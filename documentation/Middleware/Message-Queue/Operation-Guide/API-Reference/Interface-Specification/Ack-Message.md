# 确认消息

- 请求行

```
POST {Http接入点}/v1/ack HTTP/1.1
```

- 请求headers参数

请求公共参数请参考[公共参数](../Call-Method/Common-parameters.md)及[签名算法](../Call-Method/Signature-Algorithm.md)章节。

- Request Body
  Request Body为JSON格式，包含参数如下：

| 字段名          | 字段类型 | 必填     | 说明                                     |
| :-------------- | :------- | :------- | :--------------------------------------- |
| topic           | string   | Required |                                          |
| consumerGroupId | string   | Required |                                          |
| ackAction       | string   | Required | SUCCESS, CONSUME_FAILED, RESEND, DISCARD |
| ackIndex        | int64    | Required |                                          |

- Response Body

1.请求成功

|  字段名   | 字段类型 | 说明                                |
| :------- | :------ | :---------------------------------- |
| requestId |  string  | 本次请求的requestId，用于搜索调用链 |
|  result   |   null   | `null`|

2.请求失败

|  字段名   | 字段类型 | 说明                                                         |
| :------- | :------ | :------------------------------------------------------------ |
| requestId |  string  | 本次请求的requestId，用于搜索调用链                          |
|   error   |   map    | 返回格式为：`{"code":500,"message":"Ack message failure","status":"INTERNAL"}`|
