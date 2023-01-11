# mall
mall项目学习
### 启动redis服务



### 本文主要讲解mall整合SpringTask的过程，以批量修改超时订单为例。

#### SpringTask是Spring自主研发的轻量级定时任务工具，相比于Quartz更加简单方便，且不需要引入其他依赖即可使用。

业务场景说明
用户对某商品进行下单操作；
系统需要根据用户购买的商品信息生成订单并锁定商品的库存；
系统设置了60分钟用户不付款就会取消订单；
开启一个定时任务，每隔10分钟检查下，如果有超时还未付款的订单，就取消订单并取消锁定的商品库存。
