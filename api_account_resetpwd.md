# 用户相关接口:重置密码

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/account/resetpassword](http://emkt.sfaessentials.com/aj/account/resetpassword)

## 接口描述

> 重置密码

## 认证方式

> 无

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| email | true | 无 | 注册邮箱 | 
|user_id| true| 无| 用户id|
|sign|true|无|重置邮件中sign信息|
|password|true|无|新密码|


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
