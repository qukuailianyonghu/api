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
    "id" : "1",
     "jsonprc" : "2.0",
     "result" : {
    "ask_node_pair" :"asknode://@[::]:13131",
    "id" :"8f087309fb0168d07ac8c6fdbed3f2ed6463c9d79757ecadb59a47307d6aea14006ec77d58ad80b43070cfdbfe70",
        "ip" : "192.168.1.155",
        "listenAddr" : "192.168.1.155:13131",
        "name" : "Ask-core/v0.1-stable-ea093f3/linux/jdk1.8.0_141-b15",
        "port" : {
         "discovery" : "13131",
         "listener" : "15180"
     },
     "protocol" : {
         "ask" : {
         "network" : "1",
          "version" : "1"
        }
        }
    }
    }

> * 错误代码

| code        | msg           | 说明     |
| ------------- |:-------------:| -----:|
|  -32601  | method_not_found | The method does not exist or is not available |
