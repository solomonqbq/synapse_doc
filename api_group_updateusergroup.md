# 修改用户权限

## 接口地址

[http://emkt.sfaessentials.com/aj/group/updateusergroup](http://emkt.sfaessentials.com/aj/group/updateusergroup)

## 接口描述

> 修改用户权限

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
|user_id| true| 无| 用户id|
| group_id | true | 无 | 权限组id | 
|name| true | 无| 用户名称|

## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data:true
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"修改失败",
    data:false
}
```
