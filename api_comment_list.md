# 某对象的评论列表

## 接口地址

[http://emkt.sfaessentials.com/v2/api/comment/list](http://emkt.sfaessentials.com/v2/api/comment/list)

## 接口描述

> C端用户查看某对象的评论列表

## 认证方式

> C端request_id, source验证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| oid | true | 无 | 评论的对象 | 
| otype | true | 无  |评论的对象类型，1：直播，2：点播|
| page | false | 无  |翻页|
|count|false|无|翻页|


## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "Success",
    "data": {
        "data": [
            {
                "update_time": 1474598694000,
                "reply_id": 168,
                "create_time": 1471429659000,
                "reply_to": {
                    "create_time": 1471429791000,
                    "id": 168,
                    "oid": 8,
                    "otype": 4,
                    "text": "222",
                    "create_user": {
                        "doctor_grade_id": "P04",
                        "doctor_id": 59,
                        "c_doctor_id": 45692321,
                        "department_id": "10202",
                        "province_id": 440000,
                        "name": "陈羽",
                        "source_app": "医联APP",
                        "ctime": 1460010525000,
                        "source_id": "C0001",
                        "hospital_id": 31204,
                        "hospital_grade_id": "L08"
                    },
                    "status": 2
                },
                "id": 167,
                "oid": 8,
                "otype": 4,
                "text": "11",
                "create_user": {
                    "doctor_grade_id": "P04",
                    "doctor_id": 59,
                    "c_doctor_id": 45692321,
                    "department_id": "10202",
                    "province_id": 440000,
                    "name": "陈羽",
                    "source_app": "医联APP",
                    "ctime": 1460010525000,
                    "source_id": "C0001",
                    "hospital_id": 31204,
                    "hospital_grade_id": "L08"
                },
                "status": 2
            },
            {
                "create_time": 1471429791000,
                "id": 168,
                "oid": 8,
                "otype": 4,
                "text": "222",
                "create_user": {
                    "doctor_grade_id": "P04",
                    "doctor_id": 59,
                    "c_doctor_id": 45692321,
                    "department_id": "10202",
                    "province_id": 440000,
                    "name": "陈羽",
                    "source_app": "医联APP",
                    "ctime": 1460010525000,
                    "source_id": "C0001",
                    "hospital_id": 31204,
                    "hospital_grade_id": "L08"
                },
                "status": 2
            },
            {
                "create_time": 1471481782000,
                "id": 169,
                "oid": 8,
                "otype": 4,
                "text": "333",
                "create_user": {
                    "doctor_grade_id": "P04",
                    "doctor_id": 59,
                    "c_doctor_id": 45692321,
                    "department_id": "10202",
                    "province_id": 440000,
                    "name": "陈羽",
                    "source_app": "医联APP",
                    "ctime": 1460010525000,
                    "source_id": "C0001",
                    "hospital_id": 31204,
                    "hospital_grade_id": "L08"
                },
                "status": 2
            },
            {
                "create_time": 1471593280000,
                "id": 188,
                "oid": 8,
                "otype": 4,
                "text": "测试",
                "create_user": {
                    "doctor_grade_id": "P04",
                    "doctor_id": 59,
                    "c_doctor_id": 45692321,
                    "department_id": "10202",
                    "province_id": 440000,
                    "name": "陈羽",
                    "source_app": "医联APP",
                    "ctime": 1460010525000,
                    "source_id": "C0001",
                    "hospital_id": 31204,
                    "hospital_grade_id": "L08"
                },
                "status": 2
            },
            {
                "update_time": 1474537327000,
                "create_time": 1474537327000,
                "id": 248,
                "oid": 8,
                "otype": 4,
                "text": "345",
                "create_user": {
                    "doctor_grade_id": "P04",
                    "doctor_id": 59,
                    "c_doctor_id": 45692321,
                    "department_id": "10202",
                    "province_id": 440000,
                    "name": "陈羽",
                    "source_app": "医联APP",
                    "ctime": 1460010525000,
                    "source_id": "C0001",
                    "hospital_id": 31204,
                    "hospital_grade_id": "L08"
                },
                "status": 2
            },
            {
                "update_time": 1474538885000,
                "create_time": 1474538885000,
                "id": 249,
                "oid": 8,
                "otype": 4,
                "text": "345",
                "create_user": {
                    "doctor_grade_id": "P04",
                    "doctor_id": 59,
                    "c_doctor_id": 45692321,
                    "department_id": "10202",
                    "province_id": 440000,
                    "name": "陈羽",
                    "source_app": "医联APP",
                    "ctime": 1460010525000,
                    "source_id": "C0001",
                    "hospital_id": 31204,
                    "hospital_grade_id": "L08"
                },
                "status": 2
            },
            {
                "update_time": 1474539042000,
                "create_time": 1474539042000,
                "id": 252,
                "oid": 8,
                "otype": 4,
                "text": "345",
                "create_user": {
                    "doctor_grade_id": "P04",
                    "doctor_id": 59,
                    "c_doctor_id": 45692321,
                    "department_id": "10202",
                    "province_id": 440000,
                    "name": "陈羽",
                    "source_app": "医联APP",
                    "ctime": 1460010525000,
                    "source_id": "C0001",
                    "hospital_id": 31204,
                    "hospital_grade_id": "L08"
                },
                "status": 2
            },
            {
                "update_time": 1474539134000,
                "create_time": 1474539134000,
                "id": 255,
                "oid": 8,
                "otype": 4,
                "text": "345",
                "create_user": {
                    "doctor_grade_id": "P04",
                    "doctor_id": 59,
                    "c_doctor_id": 45692321,
                    "department_id": "10202",
                    "province_id": 440000,
                    "name": "陈羽",
                    "source_app": "医联APP",
                    "ctime": 1460010525000,
                    "source_id": "C0001",
                    "hospital_id": 31204,
                    "hospital_grade_id": "L08"
                },
                "status": 2
            },
            {
                "update_time": 1474539272000,
                "create_time": 1474539272000,
                "id": 258,
                "oid": 8,
                "otype": 4,
                "text": "345",
                "create_user": {
                    "doctor_grade_id": "P04",
                    "doctor_id": 59,
                    "c_doctor_id": 45692321,
                    "department_id": "10202",
                    "province_id": 440000,
                    "name": "陈羽",
                    "source_app": "医联APP",
                    "ctime": 1460010525000,
                    "source_id": "C0001",
                    "hospital_id": 31204,
                    "hospital_grade_id": "L08"
                },
                "status": 2
            },
            {
                "update_time": 1474539414000,
                "create_time": 1474539414000,
                "id": 260,
                "oid": 8,
                "otype": 4,
                "text": "345",
                "create_user": {
                    "doctor_grade_id": "P04",
                    "doctor_id": 59,
                    "c_doctor_id": 45692321,
                    "department_id": "10202",
                    "province_id": 440000,
                    "name": "陈羽",
                    "source_app": "医联APP",
                    "ctime": 1460010525000,
                    "source_id": "C0001",
                    "hospital_id": 31204,
                    "hospital_grade_id": "L08"
                },
                "status": 2
            },
            {
                "update_time": 1474540510000,
                "create_time": 1474540510000,
                "id": 261,
                "oid": 8,
                "otype": 4,
                "text": "4567890",
                "create_user": {
                    "doctor_grade_id": "0",
                    "doctor_id": 132,
                    "c_doctor_id": 0,
                    "department_id": "0",
                    "name": "系统管理员",
                    "source_app": "管理后台",
                    "ctime": 1469673189000,
                    "source_id": "B0001",
                    "hospital_id": 0,
                    "hospital_grade_id": "0"
                },
                "status": 2
            }
        ],
        "count": 11
    }
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