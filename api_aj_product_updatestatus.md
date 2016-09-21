# 产品相关接口:产品状态修改

## 接口地址

[http://emkt.sfaessentials.com/aj/product/updatestatus](http://emkt.sfaessentials.com/aj/product/updatestatus)

## 接口描述

> 产品状态修改接口(支持批量)

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| product_ids | true | 无 | 药品id，支持批量通过","分隔 | 
| status | true | 无 | 状态(0:禁用, 1:启用) | 


## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "Success",
   data: true
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"禁用产品失败",
    data:false
}
```
