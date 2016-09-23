# 产品相关接口:H5落地页记录点播有效播放

## 接口地址

[http://emkt.sfaessentials.com/v2/api/subject/lvb/playtime](http://emkt.sfaessentials.com/v2/api/subject/lvb/playtime)

## 接口描述

> H5落地页记录点播有效播放

## 认证方式

> false

## 测试接口

> http://123.56.178.15:8088/v2/api/subject/lvb/playtime?id=1&&request_id=59


## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| lvb_id | true | 无 |  资讯id|
| request_id| true | 无 | c端来源id|



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
    code:10001,
    msg:"error",
    data:false
}
```
