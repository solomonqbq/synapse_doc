# 审核评论

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/comment/review](http://emkt.sfaessentials.com/v2/aj/comment/review)

## 接口描述

> B端审核评论

## 认证方式

> 登录验证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| comment_id | true | 无  |评论id|
|status|false|无| 1：通过，0：删除|


## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "success",
    "data": true
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"系统繁忙",
    data:false
}
```