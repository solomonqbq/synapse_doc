# 资讯相关接口:资讯列表接口

## 接口地址

[http://emkt.sfaessentials.com/aj/essay/list](http://emkt.sfaessentials.com/aj/essay/list)

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
                id: "19",
                title: "测试",
                image: "www.baidu.com",
                periodical: "测试",
                author: "wantao",
                source: "测试",
                release_time: "2015-01-01 00:00:00",
                tags: "测试",
                content_id: "28",
                promotion_id: "301",
                status: "0",
                company_id: "1",
                create_user: "1",
                insert_time: "2016-05-25 00:14:57",
                update_time: "2016-05-25 00:14:57",
                promotion_title: "测试推广",
                type: "1",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            },
            {
                id: "18",
                title: "测试",
                image: "www.baidu.com",
                periodical: "测试",
                author: "wantao",
                source: "测试",
                release_time: "2015-01-01 00:00:00",
                tags: "测试",
                content_id: "27",
                promotion_id: "300",
                status: "0",
                company_id: "1",
                create_user: "1",
                insert_time: "2016-05-25 00:13:31",
                update_time: "2016-05-25 00:13:31",
                promotion_title: "测试推广",
                type: "1",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            },
            {
                id: "17",
                title: "测试",
                image: "www.baidu.com",
                periodical: "测试",
                author: "wantao",
                source: "测试",
                release_time: "2015-01-01 00:00:00",
                tags: "测试",
                content_id: "26",
                promotion_id: "299",
                status: "0",
                company_id: "1",
                create_user: "1",
                insert_time: "2016-05-25 00:03:04",
                update_time: "2016-05-25 00:03:04",
                promotion_title: "测试推广",
                type: "1",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            },
            {
                id: "16",
                title: "测试",
                image: "www.baidu.com",
                periodical: "测试",
                author: "wantao",
                source: "测试",
                release_time: "2015-01-01 00:00:00",
                tags: "测试",
                content_id: "25",
                promotion_id: "298",
                status: "0",
                company_id: "1",
                create_user: "1",
                insert_time: "2016-05-24 17:55:20",
                update_time: "2016-05-24 23:13:29",
                promotion_title: "测试推广",
                type: "1",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            },
            {
                id: "13",
                title: "测试",
                image: "www.baidu.com",
                periodical: "测试",
                author: "wantao",
                source: "测试",
                release_time: "2015-01-01 00:00:00",
                tags: "测试",
                content_id: "22",
                promotion_id: "293",
                status: "0",
                company_id: "1",
                create_user: "1",
                insert_time: "2016-05-24 17:53:25",
                update_time: "2016-05-24 23:13:27",
                promotion_title: "测试推广",
                type: "1",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            },
            {
                id: "12",
                title: "测试",
                image: "www.baidu.com",
                periodical: "测试",
                author: "wantao",
                source: "测试",
                release_time: "2015-01-01 00:00:00",
                tags: "测试",
                content_id: "21",
                promotion_id: "292",
                status: "1",
                company_id: "1",
                create_user: "1",
                insert_time: "2016-05-24 17:51:16",
                update_time: "2016-05-24 23:13:26",
                promotion_title: "测试推广",
                type: "1",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            },
            {
                id: "1",
                title: "测试",
                image: "",
                periodical: "",
                author: "",
                source: "",
                release_time: "0000-00-00 00:00:00",
                tags: "",
                content_id: "0",
                promotion_id: "1",
                status: "1",
                company_id: "0",
                create_user: "0",
                insert_time: "2016-05-15 11:49:48",
                update_time: "2016-05-24 00:13:36",
                promotion_title: "推广",
                type: "0",
                begin_time: "2016-05-16 23:53:25",
                end_time: "2016-05-16 23:53:25"
            }
        ],
        total: 7
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