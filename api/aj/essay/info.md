# 资讯相关接口:资讯内容接口

## 接口地址

[http://emkt.sfaessentials.com/aj/essay/info](http://emkt.sfaessentials.com/aj/essay/info)

## 接口描述

> 资讯内容接口

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
    code: 10000,
    msg: "success",
    data: {
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
        content_cn: "测试",
        content_en: null
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