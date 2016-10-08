# 点播相关接口:通过fileId获取播放地址接口

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/vod/vodUrlInfo](http://emkt.sfaessentials.com/v2/aj/vod/vod/vodUrlInfo)

## 接口描述

> 列表接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| fileId | string| true | |fileId  | 


## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "info",
    data: {
        playSet: [
            {
                url: "http://200019300.vod.myqcloud.com/200019300_050b84d24f1111e6bc5753e1116a4f8c.f0.mp4",
                definition: 0,
                vbitrate: 0,
                vheight: 0,
                vwidth: 0
            },
            {
                url: "http://200019300.vod.myqcloud.com/200019300_050b84d24f1111e6bc5753e1116a4f8c.f20.mp4",
                definition: 20,
                vbitrate: 45640,
                vheight: 362,
                vwidth: 640
            }
        ]
    }
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"操作失败",
    data:false
}
```