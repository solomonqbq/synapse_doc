# 直播相关接口:新建接口

## 接口地址

[http://emkt.sfaessentials.com/aj/lvb/add](http://emkt.sfaessentials.com/aj/lvb/add)

## 接口描述

> 新建直播频道接口

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| lvb | json | true | 无 | 资讯相关信息 | 
| promotion | json | true | 无 | 资讯管理推广信息 |
| relates |  json | true | 无 | 资讯关联产品/TA/信息点 |
| includings |  json | true | 无 | 推广覆盖面 |

> 参数说明
```javascript
{
    "lvb": {
        "title": "",
        "video_name": "",
        "meeting_start_time": "",
        "meeting_end_time": "",
        "description": "",
        "address": "", // HLS推流地址
        "limit": "",
        "tags": "",
        "image": "",
        "author": "",
        "author_title": "",
        "author_hospital": "",
        "author_introduction": "",
        "author_image": "",
        "notice_email": "",
        "notice_phone": "",
        "is_vod": "",
        "status": ""
    },
    "promotion": {
        "template_id":"-1" // -1为新增模板
        "template_name":"模板名称" // 当template_id = -1 是此参数为必填，否则为选填
        "threshold": "",
        "begin_time": "",
        "end_time": "",
  "coverage" : 1111, //覆盖人数
    },
    "relates": [
        {
            "relate_type": "",  // 关联类型(产品:1、TA:2、信息点:3)
            "relate_id": ""
        }
    ],
    "includings": [{
        "category": "", // 覆盖区域类型(区域:1, 医院等级:2 ,科室:3, 医生等级: 4)
        "subject_id":""
    }]
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
    error_code:10001,
    error:"新建资讯失败",
    data:false
}
```
