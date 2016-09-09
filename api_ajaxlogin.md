# 用户相关接口:登录验证

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/ajaxlogin](http://emkt.sfaessentials.com/aj/ajaxlogin)

## 接口描述

> 登录验证

## 认证方式

> 无

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| useremail | true | 无 | 注册邮箱 | 
| password | true | 无 | 密码 |


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
