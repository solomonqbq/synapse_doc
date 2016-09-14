# 直播相关接口:根据科室查询直播

## 接口地址

[http://emkt.sfaessentials.com/v2/api/subject/lvb/list](http://emkt.sfaessentials.com/v2/api/subject/lvb/list)

## 接口描述

> 根据科室查询内容

## 认证方式

> false



## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| idb_department_id | true| 无 | IDB系统的科室ID | 
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
                "author": "呗意义",
                "author_title": "教授",
                "end_time": 1470303536000,
                "description": "",
                "begin_time": 1470217136000,
                "title": "测试直播0802",
                "meeting_end_time": "`2016-08-03 09:38:56`",
                "type": 4,
                "author_image": "http://emkt.sfaessentials.com/images/upload/20160802/14701309732981.png",
                "tags": "测试直播，测试，测试001，二尺四，",
                "uptime": 1470326702000,
                "id": 13,
                "qcloud_channel_id": 16093425727656288000,
                "meeting_start_time": "`2016-08-02 10:00:56`"
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