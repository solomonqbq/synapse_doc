# 点播相关接口:编辑接口

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/vod/modify](http://emkt.sfaessentials.com/v2/aj/vod/modify)

## 接口描述

> 编辑接口

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| id | integer | true | 无 | id |  
|is_promotion_ch|Integer|true|无|is_promotion_ch|
|is_relates_ch|Integer|true|无|is_relates_ch|
|is_relates_ch|Integer|true|无|is_relates_ch|
| vod | json | true | 无 | 相关信息 | 
| promotion | json | true | 无 | 管理推广信息 |
| relates |  json | true | 无 | 关联产品/TA/信息点 |
| includings |  json | true | 无 | 推广覆盖面 |

> 参数说明
```javascript
{  
    "id":"221",
    "is_promotion_ch":"1",
    "is_relates_ch":"1",
    "is_includings_ch":"1",
    "vod": {
        "qcloud_fileid": "14651978969302274763",
        "status": "1",
        "title": "testtes1t",
        "desciption": "describle",
        "tags": "1234",
        "image": "http://emkt.sfaessentials.com/images/upload/20160929/1475135734275.png",
        "author": "heiheihie",
        "author_title": "heiheihie",
        "author_hospital": "heiheihie",
        "author_introduction": "heiheihie",
        "author_image": "http://emkt.sfaessentials.com/images/upload/20160929/14751357434239.png"
    },
    "relates": [
        {
            "relate_type": "1",
            "relate_id": "148972"
        },
        {
            "relate_type": "2",
            "relate_id": "69"
        },
        {
            "relate_type": "3",
            "relate_id": "373"
        },
        {
            "relate_type": "3",
            "relate_id": "437"
        }
    ],
    "promotion": {
        "template_id": "-1",
        "template_name": "52525",
        "threshold": 100,
        "begin_time": "1475204405",
        "end_time": "1475201000",
        "coverage": 604134
    },
    "includings": [
        {
            "category": "1",
            "subject_id": "1002"
        },
        {
            "category": "1",
            "subject_id": "1003"
        },
        {
            "category": "3",
            "subject_id": "10202"
        },
        {
            "category": "3",
            "subject_id": "10203"
        },
        {
            "category": "2",
            "subject_id": "3"
        },
        {
            "category": "2",
            "subject_id": "5"
        },
        {
            "category": "4",
            "subject_id": "3"
        }
    ]
}
```
## 响应数据(JSON):
> 成功
```javascript
{
   code: 10000,
   msg: "Success",
   data:  [],
}
```
> 失败 
```javascript
{
    code:10001,
    error:"新建资讯失败",
    data:false
}
```