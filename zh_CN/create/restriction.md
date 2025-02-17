# 配额和限制

EMQX Cloud 对每一种部署都设置了默认配额（或限制），其中某些配额的默认值可以调整。您可以通过下面的表格按部署查看配额的默认值以及是否可以调整。如果您需要调整配额，请[联系我们](../feature/tickets.md)。

## Serverless
| **配额名称**         | **默认值**                | **是否可调整**     |
| --------------------| ----------------------- | ------------------|
| 内部认证鉴权最大条目数     | 2000                | 不可调整                  |
| 内部访问控制最大条目数     | 2000                | 不可调整                   |
| 匿名访问     | 不可匿名访问      | 不可调整                   |
| 消息队列最大长度     | 1000                | 不可调整                   |
| 消息大小上限     | 1 MB                | 不可调整                   |
| 会话保持时间（MQTT 3.x）     | 2小时                | 不可调整                   |
| 保留消息最大条目数     | 2000                | 不可调整                   |
| 保留消息单条大小上限     | 1 MB                | 不可调整                   |
| 保留消息超期时间     | 永不超期                | 不可调整                   |
| Client ID 最大长度（MQTT 3.x）     | 23                | 不可调整                   |
| Client ID 最大长度（MQTT 5.0）     | 256                | 不可调整                   |
| 单个客户端最大订阅数     | 10                | 不可调整                   |
| TCP 报文发送超时最大时间     | 10s                | 不可调整                   |
| 部署个数最大配额     | 1个                | 可调整                   |
| 子账号个数最大配额     | 20个                | 不可调整                   |


## 专有版和BYOC

| **配额名称**         | **默认值**                | **是否可调整**           |**是否需要重启部署** |
| --------------------| ----------------------- | ------------------|------------------|
| 内部认证鉴权最大条目数     | 部署连接规格 * 2      | 不可调整                  |-|
| 内部访问控制最大条目数     | 部署连接规格 * 2      | 不可调整                   |-|
| 同时支持的外部扩展认证     | 2种      | 不可调整                   |-|
| 匿名访问     | 不可匿名访问      | 可调整                   |不需重启|
| 消息队列最大长度     | 1000                | 可调整                   |不需重启|
| 消息大小上限     | 1 MB                | 可调整                   |不需重启|
| 会话保持时间（MQTT 3.x）     | 2小时                | 不可调整                   |不需重启|
| 保留消息最大条目数     | 部署连接规格 * 10    | 可调整                   |不需重启|
| 保留消息单条大小上限     | 1 MB                | 可调整                   |不需重启|
| 保留消息超期时间     | 永不超期                | 可调整                   |不需重启|
| Client ID 最大长度（MQTT 3.x）     | 23                | 可调整                   |需要重启|
| Client ID 最大长度（MQTT 5.0）     | 256                | 可调整                   |需要重启|
| API HTTP QPS     | 100/s                | 不可调整                   |-|
| TCP 报文发送超时最大时间     | 10s                | 可调整                   |需要重启|
| 数据集成中可创建的最大资源数     | 10个               | 不可调整                   |-|
| 数据集成中可创建的最大规则数     | 50条               | 不可调整                   |-|
| 部署个数最大配额     | 3个                | 可调整                   |不需重启|
| 子账号个数最大配额     | 20个                | 不可调整                   |-|