# 搜索权限组接口

## 接口地址

[http://emkt.sfaessentials.com/aj/group/search](http://emkt.sfaessentials.com/aj/group/search)

## 接口描述

> 搜索创建的权限组

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| key | false | 无 | 搜索关键字 | 
| page | false | 1 | 数据页数 | 
| count | false | 20 | 每页数据量 |
| order | false | 无 | 排序字段 | 
| order_type | false | asc | 排序类型(asc,desc) | 



## 响应数据(JSON):
> 成功

```javascript
{
   "code":10000,
    "msg":"Success",
    "data":{
        "data":[
            {
                "company_id":39,
                "create_time":1471845004000,
                "user_count":0,
                "auth":"{"products":"149020,149019,149018","tas":"114,113,112","powers":"10001,10002,10003,10004,10005,10006,10007,10008"}",
                "name":"chhtest2",
                "description":"",
                "id":100,
                "create_user":347,
                "type":0,
                "status":1
            },
            {
                "company_id":39,
                "create_time":1471844257000,
                "user_count":0,
                "auth":"{"products":"149019","tas":"113,114","powers":"10002,10001"}",
                "name":"chhtest1",
                "description":"",
                "id":98,
                "create_user":347,
                "type":0,
                "status":1
            }
        ],
        "total":2
    }
}
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"error",
    data:false
}
```