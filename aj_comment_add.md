# B端发表评论

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/comment/add](http://emkt.sfaessentials.com/v2/aj/comment/add)

## 接口描述

> B端发表评论，统一会以“系统管理员”的身份发出去

## 认证方式

> B端登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| oid | true | 无 | 评论的对象 | 
| otype | true | 无  |评论的对象类型，1：直播，2：点播|
| text | true | 无  |评论内容，500个字|


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
    code:10001,
    msg:"系统繁忙",
    data:false
}
```