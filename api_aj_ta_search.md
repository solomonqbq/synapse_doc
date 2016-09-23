# 领域相关接口:领域搜索接口

## 接口地址

[http://emkt.sfaessentials.com/aj/ta/search](http://emkt.sfaessentials.com/aj/ta/search)

## 接口描述

> 领域搜索接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| type | true | 无 | 搜索类型：simple（简单搜索）senior（高级搜索） |
| key | true | 无 | 搜索关键词对象 | 
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
                "name": "测试药品测试-编辑",
                "description": "Test Product666",
                "create_user": "110",
                "create_time": "2015-12-01 00:00:00",
                
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