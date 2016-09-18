# 用户相关接口:待审核用户列表

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/account/reviewlist](http://emkt.sfaessentials.com/aj/account/reviewlist)

## 接口描述

> 待审核用户列表

## 认证方式

> 无

## 请求参数(get):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| page | true | 无 | 页码 |
| count| true | 无 | 记录条数| 


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
    ode:10001,
    msg:"系统失败",
    data:{}
}
```
