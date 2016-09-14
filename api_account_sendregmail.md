# 用户相关接口:新建账号，发送激活邮件

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/account/sendregmail](http://emkt.sfaessentials.com/aj/account/sendregmail)

## 接口描述

> 新建账户发送账号激活邮件

## 认证方式

> 无

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| email | true | 无 | 注册邮箱 | 


## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "Success",
   data: {
      
   }
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"发送失败",
    data:{}
}
```
