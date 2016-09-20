# 信息点相关接口:信息点列表接口

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/keyword/list](http://emkt.sfaessentials.com//v2aj/keyword/list)

## 接口描述

> 信息点列表接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| page | false | 1 | 数据页数 | 
| count | false | 20 | 每页数据量 |
| order | false | 无 | 排序字段 | 
| order_type | false | asc | 排序类型(asc,desc) | 



## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        data: [
            {
                id: "35",
                keyword: "乙酰螺旋霉素片",
                description: "Acetylspiramycin Tablets",
                create_user: "0",
                create_time: "2016-01-18 20:32:49",
            },
           
        ],
        total: 31887,
        
    }
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"error",
    data:{}
}
```