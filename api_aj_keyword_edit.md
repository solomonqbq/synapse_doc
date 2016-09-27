# 信息点相关接口:编辑接口

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/keyword/edit](http://emkt.sfaessentials.com/v2/aj/keyword/edit)

## 接口描述

> 信息点编辑接口

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
|id| true| 无| 信息点唯一ID|
| keyword | false | 无 | 中文名 | 
| description | false | 无  | 英文名 |
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
   data:  true,
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"修改信息点失败",
    data:{}
}
```