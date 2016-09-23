# 产品相关接口:点击播放请求接口

## 接口地址

[http://emkt.sfaessentials.com/v2/api/subject/vod/play](http://emkt.sfaessentials.com/v2/api/subject/vod/play)

## 接口描述

> 点击播放请求接口，用于记录播放人数，扣除费用。

## 认证方式

> false

## 测试接口

> http://123.56.178.15:8088/v2/api/subject/vod/play?vod_id=1&&request_id=59


## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| vod_id | true | 无 |  资讯id|
| request_id| true | 无 | uid|



## 响应数据(JSON):
> 成功

```javascript

{
    code: 10000,
    msg: "success",
    data:true
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"error",
    data:false
}
```

