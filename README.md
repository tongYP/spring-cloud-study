# 项目简介

SpringCloud微服务框架实战（基于Finchley版本，SpringBoot2版本实现）

内容主要包含：

| 微服务角色                 | 对应的技术选型                              |
| --------------------- | ------------------------------------ |
| 注册中心(Register Server) | Eureka                               |
| 服务提供者                 | spring mvc、spring-data-jpa、h2等       |
| 服务消费者                 | Ribbon/Feign消费服务提供者的接口               |
| 熔断器                   | Hystrix，包括Hystrix Dashboard以及Turbine |
| 配置服务                  | Spring Cloud Config Server           |
| API Gateway           | Zuul                                 |
| 服务链路追踪           | Sleuth                                 |

# 准备

## 环境准备：

| 工具    | 版本或描述                |
| ----- | -------------------- |
| JDK   | 1.8                  |
| IDE   | Eclipse 或者 IntelliJ IDEA |
| Maven | 3.x                  |

## 主机名配置：

| 主机名配置（C:\Windows\System32\drivers\etc\hosts文件） |
| ---------------------------------------- |
| 127.0.0.1 discovery config-server gateway movie user feign ribbon |

## 主机规划：

| 项目名称                                     | 端口   | 描述                     | URL             |
| ---------------------------------------- | ---- | ---------------------- | --------------- |
| microservice-api-gateway                 | 8050 | API Gateway            | 详见文章            |
| microservice-config-client               | 8041 | 配置服务的客户端               | 详见文章            |
| microservice-config-server               | 8040 | 配置服务                   | 详见文章            |
| microservice-consumer-movie-feign        | 8020 | Feign Demo             |         |
| microservice-consumer-movie-feign-with-hystrix | 8021 | Feign Hystrix Demo     |        |
| microservice-consumer-movie-feign-with-hystrix-stream | 8022 | Hystrix Dashboard Demo |        |
| microservice-consumer-movie-ribbon       | 8010 | Ribbon Demo            |        |
| microservice-consumer-movie-ribbon-with-hystrix | 8011 | Ribbon Hystrix Demo    |      |
| microservice-discovery-eureka            | 8761 | 注册中心                   |                |
| microservice-hystrix-dashboard           | 8030 | hystrix监控              |  |
| microservice-hystrix-turbine             | 8031 | turbine                |  |
| microservice-provider-user               | 8000 | 服务提供者                  |              |
| microservice-consumer-zipkin-hi               | 8988 | 服务链路追踪，服务1                 |              |
| microservice-consumer-zipkin-greet            | 8989 | 服务链路追踪，服务2                 |              |
|                                          |      |                        |                 |

[教程说明地址，旧版本文档](https://github.com/hemin1003/spring-cloud-book)

## [关于我](http://heminit.com/about/)

欢迎交流问题，可加我的个人QQ 469580884，或群号 751925591，一起探讨交流问题

[我的博客地址](http://blog.csdn.net/hemin1003)

[个人域名](http://heminit.com)

## 感谢
如果觉得内容赞，您可以请我喝杯咖啡：
<br/>
<img src="./pay/wechat.jpeg" width="240px" height="240px" />&nbsp;&nbsp;&nbsp;&nbsp;
<img src="./pay/alipay.jpeg" width="240px" height="240px" />