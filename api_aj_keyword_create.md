# 信息点相关接口:新建接口

## 接口地址

[http://emkt.sfaessentials.com/aj/keyword/create](http://emkt.sfaessentials.com/aj/keyword/create)

## 接口描述

> 新建信息接口

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| keyword | true | 无 | 名称 | 
| description | false | 无  |描述 |
|product_ids| false | 无| 关联的产品id列表，多个用逗号分隔|
|ta_ids|false|无| 关联的领域id列表，多个用逗号分隔|
|status| false | 1 |  信息点启用状态1启用，0禁用|
|expire_time| true | 无| 过期时间|



## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "Success",
   data:  1,
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"新建信息点失败",
    data:false
}
```