# 产品相关接口:产品搜索接口

## 接口地址

[http://emkt.sfaessentials.com/aj/product/search](http://emkt.sfaessentials.com/aj/product/search)

## 接口描述

> 产品搜索接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| keyword | true | 无 | 搜索关键词 | 
| page | false | 1 | 数据页数 | 
| count | false | 20 | 每页数据量 |
| order | false | 无 | 排序字段 | 
| order_type | false | asc | 排序类型(asc,desc) | 


## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "success",
    "data": {
        "data": [
            {
                "id": "1",
                "cn_name": "测试药品测试-编辑",
                "en_name": "Test Product666",
                "general_name": "梅尼尔梅尼尔梅尼尔梅11111111测试测试测试测试测试测试",
                "image": "http://emkt.sfaessentials.com//images/upload/20160131/14542127629889.png",
                "ingredient": "GDFGDSGDSFGDGDG",
                "adaptation": "",
                "usage": "",
                "reactions": "",
                "taboos": "",
                "matters": "",
                "classification": "",
                "price": "7.50",
                "insurance_type": "0",
                "status": "1",
                "otc": "1",
                "corporation": "",
                "department": "",
                "folder_id": "1",
                "group_id": "0",
                "create_user": "110",
                "listing_time": "2015-12-01 00:00:00",
                "insert_time": "2016-01-10 13:54:04",
                "update_time": "2016-02-03 17:31:52"
            },
           
        "total": 29
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