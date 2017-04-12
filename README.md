此项目只是拆分了 商城 http://git.oschina.net/catshen/zsTrade 


- shop-admin 商城后台管理
- shop-web 商城前台 （首页 支付 等）
- shop-common 商城公共类 工具类等
- shop-order-api  订单dubbox接口
- shop-order      订单dubbox实现类 采用sharding jdbc 进行订单分库分表
- shop-member-api 会员dubbox接口
- shop-member     会员dubbox实现类 采用sharding jdbc 进行订单分库分表
- shop-goods-api  商品dubbox接口
- shop-goods      商品dubbox实现类  （商品，楼层 ，类别 品牌 等）

演示地址
http://zscat.top/
使用技术和后台同  
http://git.oschina.net/catshen/cat

### 运行部署
运行zscat-tools 下面的run.bat 同时启动zookeep redis nginx，默认配置 在app.properties修改
1.修改shop-order模块下的app.properties 的数据库链接 ，运行Bootstrap类

2.修改shop-member模块下的app.properties 的数据库链接 ，运行Bootstrap类
![输入图片说明](http://git.oschina.net/uploads/images/2017/0412/100614_d296568c_134431.png "在这里输入图片标题")

3.修改shop-goods模块下的app.properties 的数据库链接 ，运行Bootstrap类
![输入图片说明](http://git.oschina.net/uploads/images/2017/0412/100627_9374930e_134431.png "在这里输入图片标题")

4.用tomcat添加shop-admin，修改tomcat端口为4080  访问 http://localhost:4080/shop-admin/
![输入图片说明](http://git.oschina.net/uploads/images/2017/0412/101032_1320272c_134431.png "在这里输入图片标题")
商品管理
![输入图片说明](http://git.oschina.net/uploads/images/2017/0412/101314_811d498c_134431.png "在这里输入图片标题")
楼层管理
![输入图片说明](http://git.oschina.net/uploads/images/2017/0412/101322_82a87832_134431.png "在这里输入图片标题")

5.用tomcat添加shop-web， 访问 http://localhost:8080/shop-web/front
![输入图片说明](http://git.oschina.net/uploads/images/2017/0412/101020_3545076d_134431.png "在这里输入图片标题")
![输入图片说明](http://git.oschina.net/uploads/images/2017/0412/101514_9c2830ca_134431.png "在这里输入图片标题")
![输入图片说明](http://git.oschina.net/uploads/images/2017/0412/101530_73ba9328_134431.png "在这里输入图片标题")


brave-dubbo.xml 采集数据到zikpin，生成分布式调研链数据
 **_启动zipkin_** 
![输入图片说明](http://git.oschina.net/uploads/images/2017/0412/101932_4d1f56da_134431.png "在这里输入图片标题")
![输入图片说明](http://git.oschina.net/uploads/images/2017/0412/101956_c632c810_134431.png "在这里输入图片标题")
![输入图片说明](http://git.oschina.net/uploads/images/2017/0412/102006_e8778091_134431.png "在这里输入图片标题")
![输入图片说明](http://git.oschina.net/uploads/images/2017/0412/102015_2204af0a_134431.png "在这里输入图片标题")
