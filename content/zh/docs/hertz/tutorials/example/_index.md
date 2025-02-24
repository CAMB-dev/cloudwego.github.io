---
title: "代码示例"
linkTitle: "代码示例"
weight: 1
description: >

---

Hertz 提供了一系列示例代码旨在帮助用户快速上手 Hertz 并了解 Hertz 的特性，参考 [hertz-examples](https://github.com/cloudwego/hertz-examples) 以获取更多信息。

## Bizdemo

### hertz_gorm
- [hertz_gorm](https://github.com/cloudwego/hertz-examples/tree/main/bizdemo/hertz_gorm) ：在 hertz server 中使用 gorm 的示例

### hertz_gorm_gen
- [hertz_gorm_gen](https://github.com/cloudwego/hertz-examples/tree/main/bizdemo/hertz_gorm_gen) ：在 hertz server 中使用 gorm/gen & proto IDL 的示例

### hertz_jwt
- [hertz_jwt](https://github.com/cloudwego/hertz-examples/tree/main/bizdemo/hertz_jwt) ：在 hertz server 中使用 jwt 的示例

### hertz_session
- [hertz_session](https://github.com/cloudwego/hertz-examples/tree/main/bizdemo/hertz_session) ：在 hertz server 中使用分布式 session 和 csrf 的示例


## Server

### 启动 Hertz
- [hello](https://github.com/cloudwego/hertz-examples/tree/main/hello) ：启动对于 hertz 来说相当于 "hello world" 的示例

### 配置
- [config](https://github.com/cloudwego/hertz-examples/tree/main/config) ：配置 hertz server 的示例

### 协议
- [Protocol](https://github.com/cloudwego/hertz-examples/tree/main/protocol) ：hertz 使用 HTTP1、TLS 等协议的示例

### 路由
- [Route](https://github.com/cloudwego/hertz-examples/tree/main/route) ：注册路由、使用路由组、参数路由的示例

### 中间件
- [basic_auth](https://github.com/cloudwego/hertz-examples/tree/main/middleware/basicauth) ：使用 basic auth 中间件的示例
- [CORS](https://github.com/cloudwego/hertz-examples/tree/main/middleware/CORS) ：使用 CORS 中间件的示例
- [custom](https://github.com/cloudwego/hertz-examples/tree/main/middleware/custom) ：自定义中间件的示例
- [pprof](https://github.com/cloudwego/hertz-examples/tree/main/middleware/pprof) ：使用 pprof 中间件的示例
- [requestid](https://github.com/cloudwego/hertz-examples/tree/main/middleware/requestid) ：使用 RequestID 中间件的示例
- [gzip](https://github.com/cloudwego/hertz-examples/tree/main/gzip) ：在 hertz server 中使用 gzip 中间件的示例

### 参数绑定及验证
- [binding](https://github.com/cloudwego/hertz-examples/tree/main/binding) ：参数绑定及验证的示例

### 获取参数
- [parameters](https://github.com/cloudwego/hertz-examples/tree/main/parameter) ：获取 query、form、cookie 等参数的示例

### 文件
- [file](https://github.com/cloudwego/hertz-examples/tree/main/file) ：关于如何上传，下载文件和搭建静态文件服务的示例

### 渲染
- [render](https://github.com/cloudwego/hertz-examples/tree/main/render) ：渲染 json, html, protobuf 的示例

### 重定向
- [redirect](https://github.com/cloudwego/hertz-examples/tree/main/redirect) ：重定向到内部/外部 URI 的示例

### 流式读/写
- [streaming](https://github.com/cloudwego/hertz-examples/tree/main/streaming) ：使用 hertz server 流式读/写的示例

### 优雅退出
- [graceful_shutdown](https://github.com/cloudwego/hertz-examples/tree/main/graceful_shutdown) ：hertz server 优雅退出的示例

### 单元测试
- [unit_test](https://github.com/cloudwego/hertz-examples/tree/main/unit_test) ：使用 hertz 提供的接口不经过网络传输编写单元测试的示例

### 链路追踪
- [tracer](https://github.com/cloudwego/hertz-examples/tree/main/tracer) ：hertz 使用 Jaeger 进行链路追踪的示例

### 监控
- [monitoring](https://github.com/cloudwego/hertz-examples/tree/main/monitoring) ：hertz 使用 Prometheus 进行指标监控的示例

### 多端口服务
- [multiple_service](https://github.com/cloudwego/hertz-examples/tree/main/multiple_service) ：使用 Hertz 启动多端口服务的示例

### 适配器
- [adaptor](https://github.com/cloudwego/hertz-examples/tree/main/adaptor) ：使用 adaptor 集成基于 `http.Handler` 接口开发的工具, 包含使用 [jade](https://github.com/Joker/jade) 作为模版引擎的示例

### Sentinel
- [sentinel:](https://github.com/cloudwego/hertz-examples/tree/main/sentinel) ：sentinel-golang 结合 hertz 使用的示例

### 反向代理
- [reverseproxy](https://github.com/cloudwego/hertz-examples/tree/main/reverseproxy) ：在 hertz server 中使用反向代理的示例

### Hlog
- [hlog:](https://github.com/cloudwego/hertz-examples/tree/main/hlog) ：使用 hlog 以及其日志拓展的示例


## Client

### 发送请求
- [send_request](https://github.com/cloudwego/hertz-examples/tree/main/client/send_request) ：使用 hertz client 发送 http 请求的示例

### 配置
- [client_config](https://github.com/cloudwego/hertz-examples/tree/main/client/config) ：配置 hertz client 的示例

### TLS
- [tls](https://github.com/cloudwego/hertz-examples/tree/main/protocol/tls) ：hertz client 发送 tls 请求的示例

### 添加请求内容
- [add_parameters](https://github.com/cloudwego/hertz-examples/tree/main/client/add_parameters) ：使用 hertz client 添加请求参数的示例

### 上传文件
- [upload_file](https://github.com/cloudwego/hertz-examples/tree/main/client/upload_file) ：使用 hertz client 上传文件的示例

### 中间件
- [middleware](https://github.com/cloudwego/hertz-examples/tree/main/client/middleware) ：使用 hertz client middleware 的示例

### 流式读响应
- [streaming_read](https://github.com/cloudwego/hertz-examples/tree/main/client/streaming_read) ：使用 hertz client 流式读响应的示例

### 正向代理
- [forward_proxy](https://github.com/cloudwego/hertz-examples/tree/main/client/forward_proxy) ：使用 hertz client 配置正向代理的示例
