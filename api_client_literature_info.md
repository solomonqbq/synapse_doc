# 产品相关接口:H5落地页获取资讯详情内容

## 接口地址

[http://emkt.sfaessentials.com/v2/api/subject/essay/detail](http://emkt.sfaessentials.com/v2/api/subject/essay/detail)

## 接口描述

> H5落地页获取资讯详情内容,并进行扣费操作

## 认证方式

> false

## 测试接口

> http://123.56.178.15:8088/v2/api/subject/essay/detail?essay_id=69&request_id=111





## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| essay_id | true | 无 |  资讯id|
| request_id | true | 无 | 用户uid|



## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "Success",
    "data": {
        "id": 256,
        "title": "asdfasfdas",
        "image": "http://emkt.sfaessentials.com/images/upload/20160820/14716272015048.png",
        "periodical": "asdfasfda",
        "author": "asdfasdfas",
        "release_time": 1471626721000,
        "content_id": 306,
        "promotion_id": 1383,
        "status": 1,
        "company_id": 37,
        "create_user": 345,
        "insert_time": 1471627214000,
        "update_time": 1474158559000,
        "relates": {
            "product": [
                {
                    "cn_name": "测试花费1",
                    "en_name": "ceshi",
                    "id": 149015,
                    "general_name": "测试"
                }
            ],
            "keyword": [
                {
                    "description": "发动机号",
                    "id": 386,
                    "keyword": "测试花费1"
                }
            ],
            "ta": [
                {
                    "name": "测试花费1",
                    "description": "返回",
                    "id": 110
                }
            ]
        },
        "content_en": null,
        "content_cn": "<p>asfdasfdas</p>",
        "subject_id": 256,
        "template_id": 54,
        "charge_id": 544,
        "threshold": 111,
        "coverage": 600806,
        "begin_time": 1471626721000,
        "end_time": 1471626721000
    }
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"error",
    data:null
}
```