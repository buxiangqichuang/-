# communities_manager
社团管理系统，该系统是基于B/S架构的，采用Java语言开发设计，通过面向接口的方式，进行交互。
controller层主要是接受从表单传递过来的数据，以及调用service层中的方法，实现页面的跳转。
service层是个接口层，它主要是因为前人提倡面向接口所以层与层之间的交互都是通过接口来实现。因此有一个serviceImpl层进行实现service接口层。
而且service层主要的功能是进行数据的校验以及调用dao层。
dao层，即数据访问层，该层主要是对数据进行CRUD操作。而里面使用的Dbutil框架中核心类QueryRunner能对一条数据，甚至多条数据进行结果集处理，比传统的封装要方便许多。
最后来谈谈这里面使用到的技术有servlet技术，dbutil技术，c3p0缓存技术等。
