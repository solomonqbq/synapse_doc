# 点播相关接口:内容接口

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/vod/info](http://emkt.sfaessentials.com/v2/aj/vod/info)

## 接口描述

> 内容接口

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
       id: "1",
       qcloud_fileid: "1234354323",
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
       begin_time: null,
       end_time: null,
       template_id: null,
       threshold: null,
       charge_id: null,
       coverage: null,
       relates: [ ]
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