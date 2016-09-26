# 信息点相关接口:信息点状态修改

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/keyword/updatestatus](http://emkt.sfaessentials.com/v2/aj/keyword/updatestatus)

## 接口描述

> 信息点状态修改接口(支持批量)

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| keyword_ids | true | 无 |信息点id，支持批量通过","分隔 | 
| status| true| 无| 1：启动，0：禁用|


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
    code:10001,
    msg:"修改信息点状态失败",
    data:false
}
```
