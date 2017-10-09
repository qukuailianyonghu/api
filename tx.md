# 交易接口列表

> 1. ### 获取服务端版本信息(server_version)
> * 请求地址 （{ "method": "server_version", "params": [], "id": 1}）
> * 请求方式 （POST）
> * 请求参数 

| 名称        | 必填           | 类型  | 说明 |
| ------------- |:-------------:| -----:| :-----|
|    无  |  |  |       |
> * 返回结果(JSON实例) 

  {
    "id" : "1",
    "jsonprc" : "2.0",
    "result" : "Ask-core/v0.1-stable-ea093f3/linux/jdk1.8.0_141-b15"
  }
  
 > * 错误代码
 
| code        | msg           | 说明     |
| ------------- |:-------------:| -----:|
|  -32601  | method_not_found | The method does not exist or is not available |

***

> 2. ### 获取节点相关信息(node_info)
> * 请求地址 （{ "method": "node_info", "params": [], "id": 1}）
> * 请求方式 (POST)
> * 请求参数

| 名称     | 必填     | 类型      | 说明    |
| ------------- |:-------------: | ------: | :--------|
|无       |    |    |   |

> * 返回结果（JSON实例） 

{
  "error" : {
    "code" : "-32601",
    "message" : "The method does not exist or is not available"
  },
  "id" : "1",
  "jsonprc" : "2.0"
}

> * 错误代码

| code        | msg           | 说明     |
| ------------- |:-------------:| -----:|
|  -32601  | method_not_found | The method does not exist or is not available |
