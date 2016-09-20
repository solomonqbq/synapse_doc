# 领域相关接口:领域详情接口

## 接口地址

[http://emkt.sfaessentials.com/aj/ta/info](http://emkt.sfaessentials.com/aj/ta/info)

## 接口描述

> 领域详情接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| ta_id | true | 无 | 产品id | 


## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        id: "47",
        name: "丁林美",
        description: "Clindamycin Phosphate Injection",
        create_user: "0",
        create_time: "2016-01-18 20:32:49",
        insert_time: "2016-01-04 17:34:13",
        update_time: "0000-00-00 00:00:00"
    }
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"获取领域详情失败",
    data:false
}
```
