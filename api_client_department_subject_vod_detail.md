# 产品相关接口:H5落地页获取点播详情内容

## 接口地址

[http://emkt.sfaessentials.com/api/subject/vod/detail](http://emkt.sfaessentials.com/api/subject/vod/detail)

## 接口描述

> H5落地页获取点播详情内容

## 认证方式

> false

## 测试接口

> http://123.56.178.15:8088/api/subject/vod/detail?essay_id=1&&request_id=59


## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| vod_id | true | 无 |  资讯id|
| request_id| true | 无 | c端来源id|



## 响应数据(JSON):
> 成功

```javascript

{
    "code": 10000,
    "msg": "Success",
    "data": {
        "subject_id": 165,
        "qcloud_fileid": "14651978969266732371",
        "relates": {
            "product": [
                {
                    "cn_name": "产品测试",
                    "en_name": "test",
                    "id": 148965,
                    "general_name": "测试产品的保存"
                }
            ],
            "keyword": [],
            "ta": [
                {
                    "name": "达克宁TA",
                    "description": "达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适",
                    "id": 63
                }
            ]
        },
        "insert_time": 1472091313000,
        "promotion_id": 1536,
        "threshold": 100,
        "title": "测试播放统计1011",
        "author_introduction": "测试播放统计1011",
        "author_image": "http://emkt.sfaessentials.com/images/upload/20160825/14720912972226.png",
        "update_time": 1474338079000,
        "charge_id": 673,
        "author_hospital": "测试播放统计1011",
        playSet: [ //点播播放地址，有两个，mp4的可以直接播放。
                [
                    {
                        url: "http://200019300.vod.myqcloud.com/200019300_baca68724a9511e696928df36f316a58.f0.mov",//
                        definition: 0,
                        vbitrate: 0,
                        vheight: 0,
                        vwidth: 0
                    },
                    {
                         url: "http://200019300.vod.myqcloud.com/200019300_baca68724a9511e696928df36f316a58.f20.mp4",
                         definition: 20,
                         vbitrate: 48351,
                         vheight: 426,
                         vwidth: 640
                    }
                ]
            ] ,
        "id": 165,
        "coverage": 601219,
        "image": "http://emkt.sfaessentials.com/images/upload/20160825/14720912857014.png",
        "desciption": "测试播放统计1011",
        "company_id": 39,
        "author": "测试播放统计1011",
        "author_title": "测试播放统计1011",
        "end_time": 1472091017000,
        "begin_time": 1472091017000,
        "comment_status": 1,
        "tags": "测试播放统计1011",
        "template_id": 51,
        "create_user": 347,
        "status": 1
    }
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

