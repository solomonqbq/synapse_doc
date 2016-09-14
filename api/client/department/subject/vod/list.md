# 产品相关接口:根据科室查询QA

## 接口地址

[http://emkt.sfaessentials.com/v2/api/subject/vod/list](http://emkt.sfaessentials.com/v2/api/subject/vod/list)

## 接口描述

> 根据科室查询内容

## 认证方式

> false



## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| idb_department_id | false | 无 | IDB系统的科室ID | 
| request_id| true | 无| c端初始化请求时得到到request_id|
| page | false | 1 | 数据页数 | 
| count | false | 20 | 每页数据量 |


## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "Success",
    "data": {
        "list": [
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160905/14730573513101.png",
                "qcloud_fileid": "14651978969267976556",
                "end_time": 1473057185000,
                "begin_time": 1473057185000,
                "id": 196,
                "title": "C端用户所在科室未在H5App接口中正确返回",
                "type": 3,
                "tags": "测试,测试,测试,测试,测试,测试,测试,测试,测试,测试,测试,测试,测试,测试",
                "uptime": 1473057399000
            }
        ],
        "total": 1
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