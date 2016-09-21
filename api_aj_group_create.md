# 创建权限组接口

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/group/create](http://emkt.sfaessentials.com/v2/aj/group/create)

## 接口描述

> 创建权限组

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| status | false | 无 | 状态 | 
| name | true | 无 | 名称 | 
| products | false | 无  |管理的产品列表（产品id，多个用逗号分隔 ）|
| tas | false | 无  |管理的领域列表（领域id，多个用逗号分隔 ）|
| powers | false | 无  |拥有的管理权限功能（权限值id，多个用逗号分隔 ）|


## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "Success",
   data:  1,
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"新建领域失败",
    data:false
}
```