# 所有的评论列表

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/comment/alllist](http://emkt.sfaessentials.com/v2/aj/comment/alllist)

## 接口描述

> B端查看最新的评论列表

## 认证方式

> 登录验证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- |
| oid| false | 无| 直播或者点播的id|
|otype|false|无|直播1，点播2| 
| page | false | 无  |翻页|
|count|false|无|翻页|


## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "success",
    "data": {
        "data": [
            {
                "id": "3",
                "oid": "121212",
                "otype": "2",
                "text": "asdafdasdfasd",
                "root_id": null,
                "reply_id": "1",
                "create_user": {
                    "doctor_id": "132",
                    "c_doctor_id": "322221122",
                    "name": "xxxxx",
                    "hospital_id": "25232",
                    "department_id": "104",
                    "doctor_grade_id": "1",
                    "hospital_grade_id": "5",
                    "region_id": null,
                    "province_id": null,
                    "city_id": null,
                    "indications_id": null,
                    "source_id": "C0001",
                    "ctime": "2016-07-06 14:06:01"
                },
                "review_user": "281",
                "review_time": "2016-07-18 00:46:23",
                "create_time": "2016-07-18 00:24:46",
                "status": "1",
                "update_time": "2016-07-18 00:46:23",
                "reply_to": {  //回复的结构体 
                    "id": "1",
                    "oid": "121212",
                    "otype": "2",
                    "text": "11adasda",
                    "root_id": null,
                    "reply_id": null,
                    "create_user": {
                        "doctor_id": "132",
                        "c_doctor_id": "322221122",
                        "name": "xxxxx",
                        "hospital_id": "25232",
                        "department_id": "104",
                        "doctor_grade_id": "1",
                        "hospital_grade_id": "5",
                        "region_id": null,
                        "province_id": null,
                        "city_id": null,
                        "indications_id": null,
                        "source_id": "C0001",
                        "ctime": "2016-07-06 14:06:01"
                    },
                    "review_user": null,
                    "review_time": null,
                    "create_time": "2016-07-17 23:52:30",
                    "status": "2",
                    "update_time": "2016-07-18 00:46:13"
                }
            }
        ],
        "count": 3
    }
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