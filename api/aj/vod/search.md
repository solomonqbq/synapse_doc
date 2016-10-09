# 点播相关接口:搜索接口

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/vod/search](http://emkt.sfaessentials.com/v2/aj/vod/search)

## 接口描述

> 列表接口

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
               id:'1'
               title: "test",
               description: "test",
               tags: "test",
               image: "test",
               author: "test",
               author_title: "test",
               author_hospital: "test",
               author_introduction: " 阿迪设法加快了速度",
               author_image: "特特",
               promotion_id: "0",
               status: "0",
               company_id: "22",
               create_user: "22",
               insert_time: "2016-07-16 18:38:43",
               update_time: "2016-07-16 18:45:08",
            },
          ],
        total: 1
    }
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"操作失败",
    data:false
}
```