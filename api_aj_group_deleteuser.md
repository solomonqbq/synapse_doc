# 删除权限组成员接口

## 接口地址

[http://emkt.sfaessentials.com/aj/group/deleteuser](http://emkt.sfaessentials.com/aj/group/deleteuser)

## 接口描述

> 删除权限组成员

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| user_ids | true | 无  | 用户id列表，多个用逗号分隔 | 


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
    error:"删除失败",
    data:false
}
```
