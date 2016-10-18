# 直播相关接口:直播列表接口

## 接口地址

[http://emkt.sfaessentials.com/aj/lvb/list](http://emkt.sfaessentials.com/aj/lvb/list)

## 接口描述

> 资讯列表接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| page | integer | true | 1 | 页码 | 
| count | integer | true | 20 | 每页展示数量 | 
| order | string | true | id | 排序字段 | 
| order_type | string | true | desc | 排序方式 | 
| extra | integer | false | 0 | 是否返回扩展字段，否:0, 是:1 | 
| status | integer | false | 0 | 资讯状态，禁用:0, 激活:1, 2:过期，3:草稿，不传返回所有 | 

## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        list: [
            {
                id: "3",
                qcloud_channel_id: "16093425727655894615",
                video_name: "test_video",
                title: "测试",
                meeting_time: "2016-07-22 00:00:00",
                description: "这是一个测试直播",
                limit: "500",
                tags: "医疗",
                image: "www.baidu.com",
                author: "jealone",
                author_title: "医生",
                author_hospital: "协和医院",
                author_introduction: "医疗专家",
                author_image: "www.baidu.com",
                promotion_id: "734",
                status: "0",
                company_id: "23",
                create_user: "279",
                insert_time: "2016-07-22 16:54:03",
                update_time: "2016-07-22 16:54:03",
                begin_time: "2016-07-22 00:00:00",
                end_time: "2016-07-23 00:00:00",
                template_id: "0",
                threshold: "1000",
                charge_id: "0",
                coverage: "0"
            },
            {
                id: "2",
                qcloud_channel_id: "4294967295",
                video_name: "test_video",
                title: "测试",
                meeting_time: "2016-07-22 00:00:00",
                description: "这是一个测试直播",
                limit: "500",
                tags: "医疗",
                image: "www.baidu.com",
                author: "jealone",
                author_title: "医生",
                author_hospital: "协和医院",
                author_introduction: "医疗专家",
                author_image: "www.baidu.com",
                promotion_id: "733",
                status: "0",
                company_id: "23",
                create_user: "279",
                insert_time: "2016-07-22 16:36:40",
                update_time: "2016-07-22 16:36:40",
                begin_time: "2016-07-22 00:00:00",
                end_time: "2016-07-23 00:00:00",
                template_id: "0",
                threshold: "1000",
                charge_id: "0",
                coverage: "0"
            },
            {
                id: "1",
                qcloud_channel_id: "4294967295",
                video_name: "test_video",
                title: "测试",
                meeting_time: "2016-07-22 00:00:00",
                description: "这是一个测试直播",
                limit: "500",
                tags: "医疗",
                image: "www.baidu.com",
                author: "jealone",
                author_title: "医生",
                author_hospital: "协和医院",
                author_introduction: "医疗专家",
                author_image: "www.baidu.com",
                promotion_id: "732",
                status: "0",
                company_id: "23",
                create_user: "279",
                insert_time: "2016-07-22 16:20:48",
                update_time: "2016-07-22 16:20:48",
                begin_time: "2016-07-22 00:00:00",
                end_time: "2016-07-23 00:00:00",
                template_id: "0",
                threshold: "1000",
                charge_id: "0",
                coverage: "0"
            }
        ],
        total: 3
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