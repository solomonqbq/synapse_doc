# 直播相关接口:删除直播接口

## 接口地址

[http://emkt.sfaessentials.com/aj/lvb/remove](http://emkt.sfaessentials.com/aj/lvb/remove)

## 接口描述

> 删除直播接口

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
    error_code:10001,
    error:"操作失败",
    data:false
}
```