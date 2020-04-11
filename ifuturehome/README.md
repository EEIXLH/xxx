#------------------------------- History--------------------------------

#### 2020/03/27 V.2.2.6实现功能如下：
1.将组件修改成配置启动模式，加载、控制设备也修改完成。

#### 2020/03/26 V.2.2.5_实现功能如下：
1.将组件修改成配置启动模式，目前加载设备还有问题

#### 2020/03/25 V.2.2.4_实现功能如下：
1.将码库文件的缓存路径改到.homeassistant/下


#### 2019/12/3 V.2.2.3_实现功能如下：
1.修改检索请求的headers的Authorization的值增加转换成str处理。


#### 2019/11/12 实现功能如下：
1.将设备的available永远身为TURE
2.更新设备属性时，不更新设备名和设备在线的属性


#### 2019/10/29 实现功能如下：
1.艾拉设备状态改变后无法同步更新的bug。
2.修复Google控制空调风速模式失败的bug。



#### 2019/9/30 实现功能如下：
1.对所有请求增加超时时间6秒，,timeout=6。
2.修改请求捕获异常的打印。
3.清除和修改部分打印信息，和打印级别。


#### 2019/9/27 实现功能如下：
1.对所有请求捕获异常，try except。
2.优化定时5分钟刷新设备列表，将每次全部加载所有类型的platform，修改为：只加载增加的设备的platform。


#### 2019/9/23 实现功能如下：
1.注释updatting设备状态时查询设备名的请求
2.打印updatting设备状态时查询设备属性的请求时间


#### 2019/9/11 实现功能如下：
1.修复token刷新的问题
2.清除多余代码，整理代码格式


#### 2019/9/10 实现功能如下：
1.更新查询红外本地缓存码库
2.只在查询的设备的时候会更新码库，如若用户切换码库，会出现不一致或控制异常的情况（隐患问题）


#### 2019/9/9 实现功能如下：
1.支持色温
2.取消轮询空调和TV，其他设备依然采用轮询更新设备状态
3.增加控制设备时间的打印


#### 2019/9/6 实现功能如下：
1.实现空调的状态同步


#### 2019/9/5 实现功能如下：
1.修复token刷新失败的问题
2.将红外设备的码库存在本地，修改所有红外设备控制直接请求ayla。


#### 2019/9/4 实现功能如下：
1.修复刷新token失败的问题


#### 2019/9/2 实现功能如下：
1.修改HA日志设置，调试级别为：发布级别为：INFO。调试级别为：DEBUG
2.修改ifuturehome组件日志设置，调试级别为：发布级别为：ERROR。调试级别为：DEBUG
3.增加打印内容


#### 2019/8/31 实现功能如下：
1.增加打印日志，设置日志级别。发布级别为：CRITICAL。调试级别为：DEBUG


#### 2019/8/31 实现功能如下：
1.修复加湿器state显示异常问题
2.修改空调控制模式后发失败的bug（当请求红外码返回为空时做容错处理）
3.实现控制TV频道的服务（通过频道的数字/名字设置频道）
4.实现加湿器设置定时的服务


#### 2019/8/28 实现功能如下：
1.修改climate控制模式的处理逻辑


#### 2019/8/23 实现功能如下：
1.修复requests库提示警告问题


#### 2019/8/22 实现功能如下：
1.修改设置TV静音的方法
2.清除打印
3.版本号为V.1.1


#### 2019/8/21 实现功能如下：
1.修改entityID
2.刷新设备状态是采用轮询方式、实时获取设备信息。目标优化成使用ayla的DSS来同步状态。(待优化)


#### 2019/8/20实现功能如下：
1.支持加湿器的湿度、工作模式、雾模式（类型为气候）
2.版本号为V.1.0


#### 2019/8/19 实现功能如下：
1.支持加湿器的开关（类型也为开关）


#### 2019/8/14 实现功能如下：
1.支持电视的开关、音量、频道（前后调）
2.支持AYLA的空调、灯、插座


#### 2019/8/8 实现功能如下：
1.修改设备名不同步的问题
2.支持AYLA的空调、灯、插座
