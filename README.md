# Spring_Boot_Sensitive_Scan
## 简介
Spring-Boot 敏感信息扫描（被动），安全测试过程中自动对请求的接口进行敏感路径的访问请求检测（如：Spring Actuator、Swagger-UI、Druid）
- 检测时会自动对请求接口的多层路径均进行拼接
- 检测时会自动进行去重（检测过的不再进行检测）
- 静态资源链接不进行检测
- 采用异步请求检测，不会影响主进程
