#pushServer
##一、简介：<br>
     PushServer是使用`Netty`实现的简单的推送服务器。
     目前服务端应用之间使用暴露提供RMI的接口实现RPC调用，客户端使用TCP长连接到推送服务器。
			（接入MQ实现消息共享，web端可使用websocket，或Servlet3.0实现短长连接）

##二、结构说明:<br>
* 部署结构：
	* bin(class和启动脚本)
		* com<br>
		* startup.sh
		* shutdown.sh
	* conf(配置文件)
		* p12file<br>
		* xxxx.xml<br>
		* sys.properties
		* log4j.properties
	* lib(依赖的jar)
	* logs(日志输出)
<br>　　　
* 启动/关闭服务：
	1. 启动：/bin/startup.sh
	2. 关闭：/bin/shutdown.sh
	
##三、调用时序图：
![](https://github.com/Aresyi/pushServer/raw/master/doc/use.png) 

##四、后续：
			进一步达到可扩展、高可用
