# 产品相关接口:H5落地页获取资讯详情内容

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
        "subject_id": 207,
        "coverage": 601164,
        "image": "http://emkt.sfaessentials.com/images/upload/20160824/1472023725300.png",
        "company_id": 39,
        "question": {
            "head": "{\"head\":\"奋斗过后是就\",\"options\":[{\"id\":\"s6wz3d23\",\"content\":\"22\",\"isRight\":true},{\"id\":\"dqk68j7s\",\"content\":\"222\",\"isRight\":false}]}",
            "type": 1,
            "stem": "\"s6wz3d23\"",
            "qa_id": 207,
            "order": 0
        },
        "relates": {
            "product": [
                {
                    "cn_name": "测试转换数据",
                    "en_name": "",
                    "id": 148945,
                    "general_name": "33"
                }
            ],
            "keyword": [
                {
                    "description": "",
                    "id": 338,
                    "keyword": "芬太尼透皮贴剂、氯雷他定片-信息点"
                }
            ],
            "ta": [
                {
                    "name": "芬太尼透皮贴剂TA",
                    "description": "",
                    "id": 57
                }
            ]
        },
        "end_time": 1472626895000,
        "begin_time": 1472022095000,
        "promotion_id": 1519,
        "threshold": 100,
        "title": "测试推广启用",
        "STATUS": 1,
        "copies": 20,
        "charge_id": 656,
        "ctime": 1472023740000,
        "template_id": 66,
        "id": 207,
        "create_user": 347,
        "desc": "法大使馆和辅导教师开发大好时机烦得很随机发单删发布的设计费报价单上班房间号多少吧分级点睡不放假的办法那倒是不方便放暑假的开发比较好的"
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