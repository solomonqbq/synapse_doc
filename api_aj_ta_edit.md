# 领域相关接口:编辑接口

## 接口地址

[http://emkt.sfaessentials.com/aj/ta/edit](http://emkt.sfaessentials.com/aj/ta/edit)

## 接口描述

> 领域编辑接口

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
|ta_id| true| 无| 领域唯一ID|
| name | true| 无 | 领域名称 | 
| description | false | 无  | 领域描述 |



## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "Success",
   data:  true,
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"修改领域信息失败",
    data:false
}
```