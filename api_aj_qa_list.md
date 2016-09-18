# 资讯相关接口:QA列表接口

## 接口地址

[http://emkt.sfaessentials.com/aj/qa/list](http://emkt.sfaessentials.com/aj/qa/list)

## 接口描述

> QA列表接口

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
| status | integer | false | 0 | QA状态，禁用:0, 激活:1, 2:过期，3:草稿，不传返回所有 | 

## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        list: [
            {
                id: "10",
                title: "测试",
                desc: "测试",
                company_id: "1",
                promotion_id: "312",
                create_user: "1",
                ctime: "2016-05-25 19:38:18",
                status: "0",
                promotion_title: "测试推广",
                type: "2",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            },
            {
                id: "9",
                title: "测试",
                desc: "测试",
                company_id: "1",
                promotion_id: "311",
                create_user: "1",
                ctime: "2016-05-25 19:38:11",
                status: "0",
                promotion_title: "测试推广",
                type: "2",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            },
            {
                id: "8",
                title: "测试",
                desc: "测试",
                company_id: "1",
                promotion_id: "310",
                create_user: "1",
                ctime: "2016-05-25 19:37:40",
                status: "0",
                promotion_title: "测试推广",
                type: "2",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            },
            {
                id: "7",
                title: "测试",
                desc: "测试",
                company_id: "1",
                promotion_id: "309",
                create_user: "1",
                ctime: "2016-05-25 19:36:48",
                status: "0",
                promotion_title: "测试推广",
                type: "2",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            },
            {
                id: "6",
                title: "测试",
                desc: "测试",
                company_id: "1",
                promotion_id: "308",
                create_user: "1",
                ctime: "2016-05-25 19:36:21",
                status: "0",
                promotion_title: "测试推广",
                type: "2",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            },
            {
                id: "5",
                title: "测试",
                desc: "测试",
                company_id: "1",
                promotion_id: "307",
                create_user: "1",
                ctime: "2016-05-25 11:05:52",
                status: "0",
                promotion_title: "测试推广",
                type: "2",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            },
            {
                id: "4",
                title: "测试修改",
                desc: "测试",
                company_id: "1",
                promotion_id: "306",
                create_user: "1",
                ctime: "2016-05-25 00:28:15",
                status: "3",
                promotion_title: "测试推广",
                type: "1",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            },
            {
                id: "3",
                title: "测试",
                desc: "测试",
                company_id: "1",
                promotion_id: "304",
                create_user: "1",
                ctime: "2016-05-25 00:25:00",
                status: "0",
                promotion_title: "测试推广",
                type: "2",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            },
            {
                id: "2",
                title: "测试",
                desc: "测试",
                company_id: "1",
                promotion_id: "303",
                create_user: "1",
                ctime: "2016-05-25 00:24:09",
                status: "0",
                promotion_title: "测试推广",
                type: "2",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            },
            {
                id: "1",
                title: "测试",
                desc: "测试",
                company_id: "1",
                promotion_id: "302",
                create_user: "1",
                ctime: "2016-05-25 00:23:08",
                status: "0",
                promotion_title: "测试推广",
                type: "2",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00"
            }
        ],
        total: 10
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