# 直通车相关接口:直通车搜索接口

## 接口地址

[http://emkt.sfaessentials.com/aj/instantad/search](http://emkt.sfaessentials.com/aj/instantad/search)

## 接口描述

> 直通车搜索接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| type | string | true | 无 | simple:简单搜索, senior:高级搜索 | 
| key | json | true | 无 | 见下 |
| page | integer | false | 1 | 页码 | 
| count | integer | false | 10 | 每页个数 | 

> simple搜素
```javascript
         {  "type":"simple",
            "key":{
                "title": "xxx",
                "cn_name": "",
                "ta_name": "",
                "start": 时间戳,
                "end": 时间戳
            },
            "page": 1,
            "count": 10,
            "order": "create_time",
            "order_type": "desc"
        }
``` 

> senior搜索
```javascript
{  "type":"senior",
            "key":{
                "title": "xxx",
                "cn_name": "",
                "ta_name": "",
                "start": 时间戳,
                "end": 时间戳
            },
            "page": 1,
            "count": 10,
            "order": "create_time",
            "order_type": "desc"
        }
```


## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "Success",
   data:  [],
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"操作失败",
    data:false
}
```