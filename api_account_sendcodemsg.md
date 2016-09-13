# 用户相关接口:发送邮件验证短信

## 接口地址

[http://emkt.sfaessentials.com/aj/account/sendvalidatemsg](http://emkt.sfaessentials.com/aj/account/sendvalidatemsg)

## 接口描述

> 发送邮件验证短信

## 认证方式

> 无

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| phone | true | 无 | 注册邮箱 | 
| user_id | true | 无 | 用户id |

## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "success",
    "data": {
        "code": 123456
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
