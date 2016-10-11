# 直通车相关接口:直通车内容接口

## 接口地址

[http://emkt.sfaessentials.com/aj/instantad/info](http://emkt.sfaessentials.com/aj/instantad/info)

## 接口描述

> 直通车内容接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| id | integer | true | 1 | 资讯id | 


## 响应数据(JSON):
> 成功

```javascript
{
  "code": 10000,
  "msg": "Success",
  "data": {
    "subject_id": 240,
    "image": "http://emkt.sfaessentials.com/images/upload/20161011/1476174772497.png",
    "company_id": 23,
    "relates": null,
    "subject": {
      "id": 240,
      "qcloud_channel_id": 9896587163603961979,
      "video_name": "新增会议",
      "title": "新增会议直播名称1476085222967",
      "meeting_start_time": 1476675086000,
      "meeting_end_time": 1476761486000,
      "description": "测试新增直播",
      "limit": 10,
      "tags": "测试，创建，直播，哈哈",
      "image": "http://emkt.sfaessentials.com/images/upload/20161009/14759838817846.png",
      "author": "张老师",
      "author_title": "主人",
      "author_hospital": "某某单位",
      "author_image": "http://emkt.sfaessentials.com/images/upload/20161009/14759842144755.png",
      "notice_phone": "15652237654",
      "notice_email": "wshzh@ideabinder.com",
      "is_vod": 0,
      "promotion_id": 1838,
      "status": 1,
      "comment_status": 1,
      "company_id": 23,
      "create_user": {
        "id": 279,
        "company_info": {
          "id": 23,
          "company_name": "西安杨森",
          "create_user": 279,
          "ctime": null,
          "company_licence": "http://emkt.sfaessentials.com/images/upload/20160704/14676191149418.png",
          "status": 1
        },
        "nickname": "weng test",
        "useremail": "wzeng@ideabinder.com",
        "avatar": "",
        "phone": "15901235813",
        "group_id": 157,
        "company_id": 23,
        "status": 1,
        "ctime": 1467617875000,
        "utime": 1474590619000,
        "company_manager": null
      },
      "insert_time": 1476085224000,
      "update_time": 1476150892000,
      "author_introduction": "很厉害的人",
      "type": 1,
      "subject_id": 255,
      "template_id": 45,
      "charge_id": 918,
      "threshold": 100,
      "coverage": 604452,
      "begin_time": 1475983825000,
      "end_time": 1479612625000,
      "create_time": 1476085224000,
      "uptime": 1476056425000
    },
    "end_time": 1476157606000,
    "begin_time": 1476155606000,
    "threshold": 999,
    "type": 4,
    "sheet_id": 2,
    "charge_id": 953,
    "name": "ceshi修改",
    "includings": [
      {
        "subject_id": 5,
        "name": "助理医师",
        "index": "P05",
        "promotion_id": 1838,
        "id": 8176,
        "type": 4,
        "category": 4
      },
      {
        "subject_id": 5,
        "name": "助理医师",
        "index": "P05",
        "promotion_id": 1838,
        "id": 8177,
        "type": 4,
        "category": 4
      },
      {
        "subject_id": 5,
        "name": "助理医师",
        "index": "P05",
        "promotion_id": 1838,
        "id": 8178,
        "type": 4,
        "category": 4
      },
      {
        "subject_id": 5,
        "name": "助理医师",
        "index": "P05",
        "promotion_id": 1838,
        "id": 8179,
        "type": 4,
        "category": 4
      },
      {
        "subject_id": 5,
        "name": "助理医师",
        "index": "P05",
        "promotion_id": 1838,
        "id": 8180,
        "type": 4,
        "category": 4
      },
      {
        "subject_id": 5,
        "name": "助理医师",
        "index": "P05",
        "promotion_id": 1838,
        "id": 8181,
        "type": 4,
        "category": 4
      },
      {
        "subject_id": 5,
        "name": "助理医师",
        "index": "P05",
        "promotion_id": 1838,
        "id": 8182,
        "type": 4,
        "category": 4
      }
    ],
    "ctime": 1476178115000,
    "id": 102,
    "create_user": 279,
    "status": 1,
    "desc": "ceshi"
  }
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"操作失败",
    data:false
}
```