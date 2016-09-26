# 权限组列表接口

## 接口地址

[http://emkt.sfaessentials.com/aj/group/list](http://emkt.sfaessentials.com/aj/group/list)

## 接口描述

> 权限组列表接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| page | false | 1 | 数据页数 | 
| count | false | 20 | 每页数据量 |
| order | false | id | 排序字段 | 
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
                name: "乙酰螺旋霉素片",
                auth:
                company_id:
                create_time:
                create_user:
                description:
                status:
                type:
                user_count:
            },
           
        ],
        total: 31887,
        
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