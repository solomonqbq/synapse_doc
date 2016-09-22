# 产品相关接口:H5落地页获取Qa详情内容

## 接口地址

[http://emkt.sfaessentials.com/v2/api/subject/qa/detail](http://emkt.sfaessentials.com/v2/api/subject/qa/detail)

## 接口描述

> H5落地页获取资讯详情内容,并进行扣费操作

## 认证方式

> false

## 测试接口

http://123.56.178.15:8088/v2/api/subject/qa/detail?qa_id=52



## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| qa_id | true | 无 | 问答id|
| request_id | true | 无 | 用户uid|



## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "Success",
    "data": {
        "subject_id": 218,
        "coverage": 601272,
        "image": "http://emkt.sfaessentials.com/images/upload/20160825/14721159228373.png",
        "company_id": 32,
        "question": [
            {
                "head": "{\"head\":\"发电设备\",\"options\":[{\"id\":\"gspt8851\",\"content\":\"1\",\"isRight\":true},{\"id\":\"sm9x0kkz\",\"content\":\"2\",\"isRight\":false}]}",
                "type": 1,
                "stem": "\"gspt8851\"",
                "qa_id": 218,
                "order": 0
            }
        ],
        "relates": {
            "product": [
                {
                    "cn_name": "测试0825",
                    "en_name": "ceshi",
                    "id": 149033,
                    "general_name": "测试"
                }
            ],
            "keyword": [
                {
                    "description": "富家大室开发环境的康师傅还记得是否还记得看是否还记得看飞机快点发货德尚嘉咖啡得化发的是会计花费的空间十分回家的时刻发货单上飞机的花费的会计师",
                    "id": 406,
                    "keyword": "测试0825"
                }
            ],
            "ta": [
                {
                    "name": "测试0825",
                    "description": "的时间发的和富家大室开发环境的康师傅还记得是否还记得看是否还记得看飞机快点发货德尚嘉咖啡得化发的是会计花费的空间十分回家的时刻发货单上飞机的花费的会计师",
                    "id": 128
                }
            ]
        },
        "end_time": 1472614808000,
        "begin_time": 1472096408000,
        "promotion_id": 1543,
        "threshold": 100,
        "title": "测试825",
        "copies": 20,
        "charge_id": 686,
        "ctime": 1472115937000,
        "template_id": 38,
        "id": 218,
        "create_user": 308,
        "desc": "放大环境的变化很放得开富家大室开发环境的康师傅还记得是否还记得看是否还记得看飞机快点发货德尚嘉咖啡得化发的是会计花费的空间十分回家的时刻发货单上飞机的花费的会计师",
        "status": 1
    }
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"error",
    data:[]
}
```