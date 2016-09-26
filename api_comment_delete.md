# 删除评论

## 接口地址

[http://emkt.sfaessentials.com/v2/api/comment/delete](http://emkt.sfaessentials.com/v2/api/comment/delete)

## 接口描述

> C端用户删除自己的评论（只能删除自己的）

## 认证方式

> C端request_id, source验证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
|request_id| true|无|C端request_id|
| comment_id | true | 无 | 评论的id | 


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
    msg:"系统繁忙",
    data:false
}
```