# 修改权限组状态接口

## 接口地址

[http://emkt.sfaessentials.com/aj/group/updatestatus](http://emkt.sfaessentials.com/aj/group/updatestatus)

## 接口描述

> 修改权限组状态，支持批量

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| group_ids | true | 无 |权限组id列表，多个用逗号分隔 |
|status| true|无|修改状态：1启动，0禁用| 


## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: true
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"修改状态失败",
    data:false
}
```
