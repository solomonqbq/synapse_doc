# 推广相关接口:推广历史列表接口

## 接口地址

[http://emkt.sfaessentials.com/aj/promotion/history](http://emkt.sfaessentials.com/aj/promotion/history)

## 接口描述

> 推广列表接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| id | integer | true | 无 | 资讯或者QA的ID | 
| type | string | true | 无 | essay or qa |


## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        list: [
            {
                id: "302",
                title: "测试推广",
                type: "2",
                subject_id: "1",
                company_id: "1",
                threshold: "100",
                coverage:"100",
                image: "www.baidu.com",
                create_user: "1",
                begin_time: "2016-05-24 00:00:00",
                end_time: "2016-06-30 00:00:00",
                create_time: "2016-05-25 00:23:08",
                status: "0",
                includings: [
                    {
                        id: "11",
                        type: "2",
                        subject_id: "1",
                        category: null,
                        promotion_id: "302"
                    }
                ]
            }
        ],
        total: 1
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