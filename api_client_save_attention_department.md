# 产品相关接口:保存所有订阅科室

## 接口地址

[http://emkt.sfaessentials.com/v2/api/department/savesubscribelist](http://emkt.sfaessentials.com/v2/api/department/savesubscribelist)

## 接口描述

> 保存所有订阅科室

## 认证方式

> false

## 测试接口

> http://emkt.sfaessentials.com/v2/api/department/savesubscribelist



## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| department_ids | true | 无 | 科室ID,逗号分隔（用此部分数据重新覆盖用户之前的订阅数据） | 
| request_uid | true | 无 | c端口请求的用户uid | 



## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "success",
    "data":null
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"error",
    data:null
}
```