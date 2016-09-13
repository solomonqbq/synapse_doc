# 产品相关接口:订阅科室

## 接口地址

[http://emkt.sfaessentials.com/v2/api/department/subscribe](http://emkt.sfaessentials.com/v2/api/department/subscribe)

## 接口描述

> 订阅科室

## 认证方式

> false

## 测试接口

> http://emkt.sfaessentials.com/v2/api/department/subscribe



## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| department_id | true | 无 | 科室ID | 
| request_uid | true | 无 | c端口请求的用户uid | 



## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "订阅成功",
    "data": null
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"error",
    data:[]
}
```