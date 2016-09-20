# 获取权限组成员列表

## 接口地址

[http://emkt.sfaessentials.com/aj/group/userlist](http://emkt.sfaessentials.com/aj/group/userlist)

## 接口描述

> 获取权限组成员列表

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
|group_id| true| 无| 权限组ID|
| page | false | 1 | 数据页数 | 
| count | false | 20 | 每页数据量 |
| order | false | 无 | 排序字段 按时间排序：ctime，按状态排序：status| 
| order_type | false | asc | 排序类型(asc,desc) | 



## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "success",
    "data": {
        "data": [
            {
                "id": "149",
                "nickname": "huasdadadada",
                "useremail": "hll870909@126.com"，
                "password": "",
                "avatar": "",
                "phone": "",
                "group_id": "45",
                "company_id": "1",
                "status": "0",
                "ctime": "2016-06-05 08:48:02",
                "utime": "2016-06-12 22:13:09"
            },
       
        ],
        "count": 2
    }
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"error",
    data:false
}
```