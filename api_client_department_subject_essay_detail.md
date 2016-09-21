# 产品相关接口:H5落地页获取资讯详情内容

## 接口地址

[http://emkt.sfaessentials.com/v2/api/subject/essay/detail](http://emkt.sfaessentials.com/v2/api/subject/essay/detail)

## 接口描述

> H5落地页获取资讯详情内容,并进行扣费操作

## 认证方式

> false

## 测试接口

> http://123.56.178.15:8088/v2/api/subject/essay/detail?essay_id=69&request_id=111




## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| essay_id | true | 无 |  资讯id|
| request_id| true | 无 | 用户request_id|



## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "Success",
    "data": {
        "subject_id": 272,
        "coverage": 601272,
        "image": "http://emkt.sfaessentials.com/images/upload/20160825/14721158503979.png",
        "company_id": 32,
        "content_id": 322,
        "relates": {
            "product": [
                {
                    "cn_name": "测试0825",
                    "en_name": "ceshi",
                    "id": 149033,
                    "general_name": "测试"
                }
            ],
            "keyword": [
                {
                    "description": "富家大室开发环境的康师傅还记得是否还记得看是否还记得看飞机快点发货德尚嘉咖啡得化发的是会计花费的空间十分回家的时刻发货单上飞机的花费的会计师",
                    "id": 406,
                    "keyword": "测试0825"
                }
            ],
            "ta": [
                {
                    "name": "测试0825",
                    "description": "的时间发的和富家大室开发环境的康师傅还记得是否还记得看是否还记得看飞机快点发货德尚嘉咖啡得化发的是会计花费的空间十分回家的时刻发货单上飞机的花费的会计师",
                    "id": 128
                }
            ]
        },
        "author": "丁香园",
        "end_time": 1472614808000,
        "insert_time": 1472115877000,
        "begin_time": 1472096408000,
        "promotion_id": 1542,
        "threshold": 10,
        "source": "测试",
        "title": "测试0825",
        "tags": "测试825",
        "update_time": 1472115877000,
        "content_cn": "<p>&nbsp;会使肌肤的积分地方叫对方的机房环境对方活动经费的<br></p>",
        "charge_id": 676,
        "periodical": "新闻周刊",
        "template_id": 38,
        "id": 272,
        "create_user": 308,
        "release_time": 1472096408000,
        "status": 1
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