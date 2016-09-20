# 领域相关接口:领域状态修改

## 接口地址

[http://emkt.sfaessentials.com/aj/ta/updatestatus](http://emkt.sfaessentials.com/aj/ta/updatestatus)

## 接口描述

> 领域状态修改接口(支持批量)

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| ta_ids | true | 无 |领域id，支持批量通过","分隔 | 


## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "Success",
   data: true
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"修改领域状态失败",
    data:false
}
```
