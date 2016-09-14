# 用户相关接口:填写注册信息，创建账号

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/account/saveuser](http://emkt.sfaessentials.com/aj/account/saveuser)

## 接口描述

> 邮件激活后完善用户信息

## 认证方式

> 无

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| user_id | true | 无 | 用户id | 
| nickname | true | 无 | 用户昵称 |
| email | true | 无 | 注册邮箱 | 
|password | true| 无 | 用户密码|
| phone | true | 无 | 手机号 |
| phone_validatecode| true| 无 | 手机验证码| 
| company_name| true | 无 | 企业名称|
| company_licence | true | 无 | 公司营业执照照片 | 



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
