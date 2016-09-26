# 回复评论

## 接口地址

[http://emkt.sfaessentials.com/v2/api/comment/reply](http://emkt.sfaessentials.com/v2/api/comment/reply)

## 接口描述

> C端用户回复某一条评论

## 认证方式

> C端request_id, source验证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
|request_id| true|无|C端request_id|
| reply_id | true | 无 | 回复的评论id | 
| text | true | 无  |评论内容，500个字|


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
    error:"系统繁忙",
    data:false
}
```