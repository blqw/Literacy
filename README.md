使用IL.Emit方式快速访问属性,字段和方法  
http://www.cnblogs.com/blqw/p/Literacy.html
这个项目是一个非常独立的代码库,使用.net2.0编译,不需要引用其他任何dll和别的项目
在我其他项目中,几乎都引用了这个项目,比如blqw.Core blqw.Json等

#### 更新说明  
* 2014.07.30  
为Literacy和ObjectProperty实体增加ID(自增标识,2个类共享自增序列)和UID(全球唯一标识符GUID)方便在做缓存的时候作为key使用  
增加TypeCodeEx枚举,用于扩展系统的TypeCode 会稍微影响构造Literacy的速度,但是由于Literacy本身是全局缓存,所以影响不大  
* 2014.07.29  
增加对特性的支持,现在可以从 Literacy 或 Literacy.Property 或 Literacy.Field 直接使用Attributes属性访问  
