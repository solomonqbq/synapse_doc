# 产品相关接口:根据科室查询QA

## 接口地址

[http://emkt.sfaessentials.com/v2/api/subject/qa/list](http://emkt.sfaessentials.com/v2/api/subject/qa/list)

## 接口描述

> 根据科室查询Qa

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
                "image": "http://emkt.sfaessentials.com/images/upload/20160828/14723954663955.png",
                "end_time": 1473950419000,
                "begin_time": 1472481619000,
                "id": 229,
                "title": "阿斯顿发生11111",
                "type": 2,
                "uptime": 1472395873000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160830/14725474226700.png",
                "end_time": 1475225361000,
                "begin_time": 1472546961000,
                "id": 234,
                "title": "四神丸问卷",
                "type": 2,
                "uptime": 1472547431000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160830/14725474892604.png",
                "end_time": 1475225361000,
                "begin_time": 1472546961000,
                "id": 235,
                "title": "碳酸氢钠注射液问卷",
                "type": 2,
                "uptime": 1472547605000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160830/14725476274576.png",
                "end_time": 1475138961000,
                "begin_time": 1472546961000,
                "id": 236,
                "title": "肺力咳合剂问卷",
                "type": 2,
                "uptime": 1472547747000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160830/14725478782782.png",
                "end_time": 1475225361000,
                "begin_time": 1472546961000,
                "id": 237,
                "title": "牛黄上清胶囊问卷",
                "type": 2,
                "uptime": 1472547894000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160830/14725479429272.png",
                "end_time": 1475138961000,
                "begin_time": 1472546961000,
                "id": 238,
                "title": "复方 苦参注射液",
                "type": 2,
                "uptime": 1472548102000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160831/14726315785022.png",
                "end_time": 1475127846000,
                "begin_time": 1472622246000,
                "id": 239,
                "title": "班赛问卷",
                "type": 2,
                "uptime": 1472631594000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160902/14728040118665.png",
                "end_time": 1475221761000,
                "begin_time": 1472802561000,
                "id": 240,
                "title": "测试1",
                "type": 2,
                "uptime": 1473058121000
            }
        ],
        "total": 8
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