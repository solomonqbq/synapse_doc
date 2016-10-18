# 直播相关接口:直播搜索接口

## 接口地址

[http://emkt.sfaessentials.com/aj/lvb/search](http://emkt.sfaessentials.com/aj/
lvb/search)

## 接口描述

> 直播搜索接口
> 到时按需求提供相应字段

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| type | string | true | 无 | simple:简单搜索, senior:高级搜索 | 
| key | json | true | 无 | 见下 |
| page | integer | false | 1 | 页码 | 
| count | integer | false | 10 | 每页个数 | 
| extra | integer | false | 0 | 是否返回扩展字段，否:0, 是:1 | 
| status | integer | false | 0 | 资讯状态，禁用:0, 激活:1, 2:过期，3:草稿，不传返回所有 | 

> simple搜素
```javascript
key={"title":"搜索"}
``` 

> senior搜索
```javascript
key={"title":"名称","general_name":"产品","ta_name":"领域","keyword":"信息点","start":"2016-01-01", "end":"2017-01-01"}
```


## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        list: [
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
                update_time: "2016-05-24 00:13:36"
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
                update_time: "2016-05-24 23:13:29"
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
                update_time: "2016-05-25 00:03:04"
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
                update_time: "2016-05-25 00:13:31"
            },
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
                update_time: "2016-05-25 00:14:57"
            },
            {
                id: "20",
                title: "测试",
                image: "www.baidu.com",
                periodical: "测试",
                author: "wantao",
                source: "测试",
                release_time: "2015-01-01 00:00:00",
                tags: "测试",
                content_id: "32",
                promotion_id: "313",
                status: "0",
                company_id: "1",
                create_user: "1",
                insert_time: "2016-05-31 14:17:51",
                update_time: "2016-05-31 14:17:51"
            }
        ],
        total: 6
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