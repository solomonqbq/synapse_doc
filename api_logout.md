# 用户相关接口:退出登录

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/account/logout](http://emkt.sfaessentials.com/aj/account/logout)

## 接口描述

> 退出登录

## 认证方式

> 无

## 请求参数(无):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 


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
    msg:退出失败",
    data:{}
}
```
