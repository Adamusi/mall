## mall
    mall项目学习

#### mall整合Redis实现缓存功能
    本文主要讲解mall整合Redis的过程，以短信验证码的存储验证为例。
    redis
        是用C语言开发的一个高性能键值对数据库，可用于数据缓存，主要用于处理大量数据的高访问负载 redis-server.exe redis.windows.conf。
    
#### mall整合SpringTask实现定时任务
    本文主要讲解mall整合SpringTask的过程，以批量修改超时订单为例。
    SpringTask
        是Spring自主研发的轻量级定时任务工具，相比于Quartz更加简单方便，且不需要引入其他依赖即可使用。
    业务场景说明
    用户对某商品进行下单操作；
    系统需要根据用户购买的商品信息生成订单并锁定商品的库存；
    系统设置了60分钟用户不付款就会取消订单；
    开启一个定时任务，每隔10分钟检查下，如果有超时还未付款的订单，就取消订单并取消锁定的商品库存。

#### mall整合Elasticsearch实现商品搜索
     本文主要讲解mall整合Elasticsearch的过程，以实现商品信息在Elasticsearch中的导入、查询、修改、删除为例。项目使用框架介绍：
     Elasticsearch 
            是一个分布式、可扩展、实时的搜索与数据分析引擎。 它能从项目一开始就赋予你的数据以搜索、分析和探索的能力，可用于实现全文搜索和实时数据统计。
     Spring Data Elasticsearch
            是Spring提供的一种以Spring Data风格来操作数据存储的方式，它可以避免编写大量的样板代码。
            
#### mall整合MongoDB实现文档操作
    本文主要讲解mall整合Mongodb的过程，以实现商品浏览记录在Mongodb中的添加、删除、查询为例。
    Mongodb
        是为快速开发互联网Web应用而构建的数据库系统，其数据模型和持久化策略就是为了构建高读/写吞吐量和高自动灾备伸缩性的系统
        注意权限管理员：C:\Windows\System32\cmd.exe
        D:\Program Files X86\middleware\mongodb\bin\mongod.exe --config "D:\Program Files X86\middleware\mongodb\mongod.cfg" --install
     Spring Data Mongodb
        是Spring提供的一种以Spring Data风格来操作数据存储的方式，它可以避免编写大量的样板代码。

#### mall整合RabbitMQ实现延迟消息
    本文主要讲解mall整合RabbitMQ实现延迟消息的过程，以发送延迟消息取消超时订单为例。
    RabbitMQ
    是一个被广泛使用的开源消息队列。它是轻量级且易于部署的，它能支持多种消息协议。RabbitMQ可以部署在分布式和联合配置中，以满足高规模、高可用性的需求。
  