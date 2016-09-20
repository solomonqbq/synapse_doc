# 领域相关接口:新建接口

## 接口地址

[http://emkt.sfaessentials.com/aj/ta/create](http://emkt.sfaessentials.com/aj/ta/create)

## 接口描述

> 新建领域接口

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| name | true | 无 | 名称 | 
| description | false | 无  |描述 |



## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "Success",
   data:  1,
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"新建领域失败",
    data:false
}
```