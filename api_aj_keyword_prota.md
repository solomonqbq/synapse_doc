# 信息点相关接口:获取产品/领域关联的信息点
## 接口地址

[http://emkt.sfaessentials.com/v2/aj/keyword/getrelatelist](http://emkt.sfaessentials.com/v2/aj/keyword/getrelatelist)

## 接口描述

> 获取产品/领域关联的信息点

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
|ta_id |false | 无| 领域ID|
| product_id | false | 无 | 产品id | 


## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "success",
    "data": {
        "35": {
            "id": "35",
            "keyword": "aaaaa",
            "description": "bbbbbb",
            "status": "0",
            "company_id": "1",
            "create_user": "1",
            "insert_time": "2016-05-25 10:21:54",
            "update_time": "2016-05-25 10:21:54"
        },
        "54": {
            "id": "54",
            "keyword": "keypoint1111asd",
            "description": "dataasda",
            "status": "0",
            "company_id": "1",
            "create_user": "1",
            "insert_time": "2016-05-30 15:23:51",
            "update_time": "2016-05-30 15:23:51"
        }
    }
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"error",
    data:false
}
```