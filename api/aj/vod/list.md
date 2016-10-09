# 点播相关接口:列表接口

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/vod/list](http://emkt.sfaessentials.com/v2/aj/vod/list)

## 接口描述

> 列表接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| page | integer | true | 1 | 页码 | 
| count | integer | true | 20 | 每页展示数量 | 
| order | string | true | id | 排序字段 | 
| order_type | string | true | desc | 排序方式 | 
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