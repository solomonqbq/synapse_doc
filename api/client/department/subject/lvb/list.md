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
                "author": "刘华",
                "author_title": "呼吸科副主任",
                "end_time": 1475140990000,
                "description": "活血止痛，软坚散结。用于气虚血瘀，痰湿凝滞引起的慢性盆腔炎，症见白带增多者。",
                "begin_time": 1472548990000,
                "title": "久金直播",
                "meeting_end_time": 1472556190000,
                "type": 4,
                "author_image": "http://emkt.sfaessentials.com/images/upload/20160830/14725495695580.png",
                "tags": "久金直播，久金直播，久金直播，久金直播，久金直播，久金直播，久金直播",
                "uptime": 1472549592000,
                "id": 203,
                "qcloud_channel_id": 9896587163583574000,
                "meeting_start_time": 1472552590000
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