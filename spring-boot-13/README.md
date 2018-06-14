## 十三:事务管理

这里主要通过单元测试演示了如何使用`@Transactional`注解来声明一个函数需要被事务管理，
通常我们单元测试为了保证每个测试之间的数据独立，会使用`@Rollback`注解让每个单元测试
都能在结束时回滚。而真正在开发业务逻辑时，我们通常在`service`层接口中使用`@Transactional`
来对各个业务逻辑进行事务管理的配置。