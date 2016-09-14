# 产品相关接口:根据科室查询文献

## 接口地址

[http://emkt.sfaessentials.com/v2/api/subject/essay/list](http://emkt.sfaessentials.com/v2/api/subject/essay/list)

## 接口描述

> 根据科室查询咨询文献

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
                "image": "http://emkt.sfaessentials.com/images/upload/20160824/14720222653078.png",
                "end_time": 1472626895000,
                "begin_time": 1472022095000,
                "id": 270,
                "title": "测试推广草稿12",
                "type": 1,
                "uptime": 1472022771000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160830/14725441522665.png",
                "end_time": 1475220598000,
                "begin_time": 1472542198000,
                "id": 278,
                "title": "关注痔血胶囊引起的肝损害",
                "type": 1,
                "uptime": 1472544168000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160830/14725443752709.png",
                "end_time": 1475220598000,
                "begin_time": 1472542198000,
                "id": 279,
                "title": "血管内皮友好型药物支架研发成为新焦点",
                "type": 1,
                "uptime": 1472544391000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160830/14725451585856.png",
                "end_time": 1475220598000,
                "begin_time": 1472542198000,
                "id": 280,
                "title": "nsight：那些获批临床的独家品种（下）",
                "type": 1,
                "uptime": 1472545178000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160830/14725454346286.png",
                "end_time": 1474961398000,
                "begin_time": 1472542198000,
                "id": 281,
                "title": "想买廉价药为啥这么难？",
                "type": 1,
                "uptime": 1472545455000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160830/14725458728739.png",
                "end_time": 1475134198000,
                "begin_time": 1472542198000,
                "id": 282,
                "title": "法国暂停酮康唑 200mg 片剂的销售和上市许可一年",
                "type": 1,
                "uptime": 1472545887000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160830/1472546079567.png",
                "end_time": 1475134198000,
                "begin_time": 1472542198000,
                "id": 283,
                "title": "商业周刊：久戴智能设备成良医",
                "type": 1,
                "uptime": 1472546093000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160830/14725461187050.png",
                "end_time": 1475047798000,
                "begin_time": 1472542198000,
                "id": 284,
                "title": "施仲伟教授",
                "type": 1,
                "uptime": 1472546256000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160830/14725464245260.png",
                "end_time": 1475134198000,
                "begin_time": 1472542198000,
                "id": 285,
                "title": "苦参素注射液治疗慢性丙型肝炎肝硬化合并糖尿病",
                "type": 1,
                "uptime": 1472546439000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160830/14725468859543.png",
                "end_time": 1475047798000,
                "begin_time": 1472542198000,
                "id": 286,
                "title": "西安：门对门药店 同一种药价格相差百元",
                "type": 1,
                "uptime": 1472546906000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160901/14726985716745.png",
                "end_time": 1474512287000,
                "begin_time": 1472697887000,
                "id": 287,
                "title": "美国 CDC 对致命化合致幻新药乙酰芬太尼发布警告",
                "type": 1,
                "uptime": 1472803923000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160902/14728096761398.png",
                "end_time": 1473064919000,
                "begin_time": 1473064919000,
                "id": 289,
                "title": "氨酚那敏胶囊通用介绍",
                "type": 1,
                "uptime": 1472809693000
            },
            {
                "image": "http://emkt.sfaessentials.com/images/upload/20160830/14725437523724.png",
                "end_time": 1475047798000,
                "begin_time": 1472542198000,
                "id": 277,
                "title": "指南解读：加拿大痤疮临床管理指南（2016 年版）",
                "type": 1,
                "uptime": 1473127756000
            }
        ],
        "total": 13
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