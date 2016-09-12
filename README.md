#sharding-validate-web
项目初步暂定完成两部分内容,以后扩展 - -
第一部分:全局id生成器
主要使用mysql+java current包,完成内存队里id全局生成器--独立的web服务
用到的知识点:
1,mysql基础事务等
2,java并发库中的各种队列
3,线程池
4,rpc框架(dubbo或者其他)
5,尝试使用一致性hash维护队列集群
第二部分
主要完成分库分表路由,入参校验框架,以及限流器
用到的知识点
1,java基础,反射,注解等
2,guava常用库
3,spring动态路由
4,无侵入式修改成使用开源的hytix并发框架
5,httpclient模拟调用id生成器生成sharding主键
6,在不使用数据库中间件的情况下读写分离
