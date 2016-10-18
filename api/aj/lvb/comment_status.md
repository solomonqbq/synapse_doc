# 直播相关接口:评论状态接口

## 接口地址

[http://emkt.sfaessentials.com/aj/lvb/comment](http://emkt.sfaessentials.com/aj/lvb/comment)

## 接口描述

> 评论状态接口

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| id | int | true | 无 | | 
| comment_status | int | true | 无 | 0 可用， 1 不可用 | 


## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "Success",
   data:  [],
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"操作失败",
    data:false
}
```