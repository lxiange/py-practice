# 随机点餐

### 【解决思路】

1. 首先，你需要阅读百度糯米[api文档](http://apistore.baidu.com/apiworks/servicedetail/508.html)。显然，在使用此api接口前你需要百度apikey，好在这个apikey获取起来相对简单，只要有百度账号就行，并且是百度全平台通用的。

2. 随后是通过http协议进行调用，你可以使用Python自带的`urllib`或`httplib`包（甚至是`socket` =_=），不过更建议使用`requests`库，这个库之前我们已经介绍过。

3. 然后是阅读各个接口的请求要求。注意到，查询商铺信息时，有两个必选参数：apikey和城市id。城市id是什么呢？这时候又得调用另一个接口，获取城市的id。

4. 注意到，api提供的功能比较有限，或许并不能直接满足我们的需求，这时候就需要对任务进行分解，对不同的api组合调用，这样基本上能够应付我们的常见需求了。

5. 其中有一个参数是要求传入地理位置坐标，我们没有办法直接获得（毕竟没有定位设备），但是可以通过任意一款地图软件，获取指定位置的坐标。

6. 还有很多接口/参数可供调用，尽情探索吧！

   ​


