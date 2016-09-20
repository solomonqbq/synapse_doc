# 添加权限组成员

## 接口地址

[http://emkt.sfaessentials.com/aj/group/adduser](http://emkt.sfaessentials.com/aj/group/adduser)

## 接口描述

> 添加权限组成员

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| group_id | true | 无 | 权限组id | 
| company_id| true| 无| 用户所属公司_id,可从group/info中获得|
|email| true| 无| 用户邮箱|
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
    error:"添加失败",
    data:false
}
```
