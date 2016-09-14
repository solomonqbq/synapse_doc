# 用户相关接口:设置密码

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/account/setpassword](http://emkt.sfaessentials.com/v2/aj/account/setpassword)

## 接口描述

> 设置用户密码接口

## 认证方式

> 无

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| user_id | true | 无 | 用户id |
| password| true | 无 | 新密码| 


## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "success",
   data: {
      
   }
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"设置失败",
    data:[]
}
```
