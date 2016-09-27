# 删除权限组接口

## 接口地址

[http://emkt.sfaessentials.com/aj/group/delete](http://emkt.sfaessentials.com/aj/group/delete)

## 接口描述

> 删除权限组

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| group_ids | true | 无  | 权限id列表，多个用逗号分隔，权限组成员不为空时不允许删除，返回“该管理员创建过历史数据,不允许删除!” | 


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
