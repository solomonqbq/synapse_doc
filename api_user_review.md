# 用户相关接口:待审核用户列表

## 接口地址

[http://emkt.sfaessentials.com/aj/account/review](http://emkt.sfaessentials.com/aj/account/review)

## 接口描述

> 待审核用户列表

## 认证方式

> 无

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| user_id | true | 无 | 用户id |
| status| true | 无 | 审核状态，1：通过，0，驳回| 


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
    error:"系统失败",
    data:[]
}
```
