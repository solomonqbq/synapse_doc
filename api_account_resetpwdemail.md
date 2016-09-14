# 用户相关接口:找回密码

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/account/findpassword](http://emkt.sfaessentials.com/aj/account/findpassword)

## 接口描述

> 通过邮箱找回密码，发送找回密码邮件

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
    msg:"验证失败",
    data:{}
}
```
