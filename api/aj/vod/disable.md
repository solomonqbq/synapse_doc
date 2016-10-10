# 点播相关接口:禁用接口

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/vod/disable](http://emkt.sfaessentials.com/v2/aj/vod/disable)

## 接口描述

> 禁用接口

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| ids | string | true | 无 | 通过","分隔 | 


## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "Success",
   data:  [],
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"操作失败",
    data:false
}
```