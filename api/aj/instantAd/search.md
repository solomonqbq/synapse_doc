# 直通车相关接口:直通车搜索接口

## 接口地址

[http://emkt.sfaessentials.com/aj/instantad/search](http://emkt.sfaessentials.com/aj/instantad/search)

## 接口描述

> 直通车搜索接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| type | string | true | 无 | simple:简单搜索, senior:高级搜索 | 
| key | json | true | 无 | 见下 |
| page | integer | false | 1 | 页码 | 
| count | integer | false | 10 | 每页个数 | 

> simple搜素
```javascript
key={"title":"搜索"}
``` 

> senior搜索
```javascript
key={"general_name":"产品","ta_name":"领域","keyword":"信息点","start":"2016-01-01", "end":"2017-01-01"}
```


## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "Success",
   data:  [],
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