# 用户相关接口:验证激活链接参数是否合法

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/account/validatereglink](http://emkt.sfaessentials.com/v2/aj/account/validatereglink)

## 接口描述

> 验证激活中间中链接参数是否合法:，激活邮件中激活链接地址形如 http://123.56.178.15:8080/account/active?k=Nj12LM%2Buftixn%2FdfiDYPOTHGh7NNC2WX6oXoQ%2B4S0hB%2BpNzH4nFnrq8Igdo23ebBkGy5nI4azE1peGU1qZHyiw%3D%3D （最终链接地址前端定，其中k参数是关键参数，跳转到激活页时，前端用此接口来验证参数是否合法

## 认证方式

> 无

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| k | true | 无 | 验证信息 | 


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
    error_code:10001,
    error:"激活链接已过期",
    data:[]
}
```
