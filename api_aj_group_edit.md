# 编辑权限组内容接口

## 接口地址

[http://emkt.sfaessentials.com/aj/group/edit](http://emkt.sfaessentials.com/aj/group/edit)

## 接口描述

> 编辑权限组内容

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
|group_id| true| 无| 权限组唯一id|
| name | false | 无 | 中文名 | 
| products | false | 无  |管理的产品列表（产品id，多个用逗号分隔 ）|
| tas | false | 无  |管理的领域列表（领域id，多个用逗号分隔 ）|
| powers | false | 无  |拥有的管理权限功能（权限值id，多个用逗号分隔 ）|
|status| true| 无| 权限组状态 1：启动，0禁用|



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
    error:"修改权限组信息失败",
    data:false
}
```