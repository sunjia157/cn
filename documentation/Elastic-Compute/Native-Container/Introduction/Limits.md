---
title:Limits

# 限制说明

 1. 目前在华北-北京、华东-上海上线。
 2. 目前仅支持基于Linux操作系统的Docker镜像。
 3. 下表是使用容器的相关限制：

|  资源   |  限制   |  例外申请方式   |
| --- | --- | --- |
|  创建容器用户身份限制  | 用户需完成实名认证| 无例外|
|  创建容器账户金额限制  |创建按配置计费容器，账户余额需大于50元 | 工单  |
|单地域容器实例配额     | 20台    |  工单   |
|单地域云硬盘配额     |  15块   | 工单     |
|单地域云硬盘快照配额     | 15个    | 工单    |
| 单VPC安全组限额    |  50个   |  工单   |
| 单地域公网IP配额    |  10个   |  工单  |
|容器系统盘类型及容量 | 高效云盘：10-100G；SSD云盘：10-100G | 不可修改 |
|容器数据盘类型及容量     |  高效云盘：20-3000G；SSD云盘：20-1000G   | 不可修改    |
|    单个安全组规则限制 |  出站与入站规则总和不超过100条   |  不可修改    |
|  单台容器可挂载的云硬盘数量   |  7块   |   不可修改   |
| 单台容器可关联的安全组数量    |  5个   |  不可修改    |
|  单台容器可绑定的公网IP数量   |  1个   | 不可修改    |
|  容器日志最大保存容量   |   10M  |  不可修改   |
| 单条容器日志最大输出字节数    |   4k  |   不可修改  |
|容器镜像使用限制     | 仅支持基于Linux操作系统的Dockerfile镜像    |不可修改 |
|  容器使用地域及地域限制   |华北-北京可用区A、华北-北京可用区B、华东-上海可用区A、华东-上海可用区B     | 不可修改      |
