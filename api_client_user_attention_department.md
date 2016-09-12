# 订阅科室列表

## 接口地址

[http://emkt.sfaessentials.com/v2/api/department/subscribelist](http://emkt.sfaessentials.com/v2/api/department/subscribelist)

## 接口描述

> 订阅科室列表

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| request_id | true | 无 | 请求 id | 




## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "Success",
    "data": {
        "data": [
            {
                "create_time": "`2016-07-08 01:48:44`",
                "department_id": 101,
                "department_type": 0,
                "name": "外科"
            },
            {
                "create_time": "`2016-07-08 01:48:44`",
                "department_id": 113,
                "department_type": 1,  //1：代表用户所属的科室，0：代表订阅的科室
                "name": "麻醉科"
            },
            {
                "create_time": "`2016-07-08 01:48:44`",
                "department_id": 10101,
                "department_type": 0,
                "name": "普通外科"
            },
            {
                "create_time": "`2016-07-08 01:48:44`",
                "department_id": 10102,
                "department_type": 0,
                "name": "泌尿外科"
            },
            {
                "create_time": "`2016-07-08 01:48:44`",
                "department_id": 10103,
                "department_type": 0,
                "name": "胸外科"
            }
        ],
        "total": 5
    }
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"内部错误",
    data:null
}
```
