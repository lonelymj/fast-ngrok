### Fast-Ngrok

Java版本Ngrok客户端,集成spring-boot随应用启动快速映射应用端口

由于原版本支持Sprintboot的版本为1.5.6.RELEASE,而本人需要目标版本为2.1.1.RELEASE,所以fork了一份进行修改，分支为2.1.1

感谢大神分享！

### 使用方法

1. 添加POM依赖: 


##### springboot:1.5.6.RELEASE
```
<dependency>
    <groupId>cn.cyejing</groupId>
    <artifactId>fast-ngrok-starter</artifactId>
    <version>1.0.1</version>
</dependency>
```

##### springboot:2.1.1.RELEASE
```
<dependency>
    <groupId>cn.cyejing</groupId>
    <artifactId>fast-ngrok-starter</artifactId>
    <version>2.1.1</version>
</dependency>
```

2. 启动spring-boot应用可以在日志看到映射的地址.

### 默认配置
可以不用填写配置启动项目,如果想修改默认配置,有以下配置项:
1. 简单配置项
```
ngrok.serevr-address=b.cyejing.cn ngrok的服务地址
ngrok.server-port=4443 ngrok的服务端口
ngrok.subdomain=自定义子域名,不填则是随机
```
2. 增强配置项
```
ngrok.enabled=true 打开ngrok映射
ngrok.hostname=自定义域名,如:yourdomain.com
ngrok.httpAuth=访问授权,如:user:password
```

``ngrok``,``spring``,``spring boot``,``spring-boot``,``springboot``,``内网映射``,``内网穿透``,``微信开发``,``接口回调``