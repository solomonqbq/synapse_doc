# 领域相关接口:获取引用领域的资讯内容
## 接口地址

[http://emkt.sfaessentials.com/aj/ta/getrelateessay](http://emkt.sfaessentials.com/aj/ta/getrelateessay)

## 接口描述

> 获取引用领域的资讯内容

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
|ta_id |true | 无| 领域ID|
| page | false | 1 | 数据页数 | 
| count | false | 20 | 每页数据量 |



## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10001,
    "msg": "获取列表失败",
    "data": {
        "data": {
            "21": {
                "id": "21",
                "title": "工作项：校验ajax提交字段信息",
                "image": "xxxx",
                "periodical": "期刊",
                "author": "作者",
                "source": "来源",
                "release_time": "2016-05-31 16:07:27",
                "tags": "关键字",
                "content_id": "51",
                "promotion_id": "314",
                "status": "0",
                "company_id": "1",
                "create_user": "1",
                "insert_time": "2016-05-31 18:08:39",
                "update_time": "2016-05-31 18:08:39"
            }
        },
        "total": 1
    }
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"error",
    data:false
}
```