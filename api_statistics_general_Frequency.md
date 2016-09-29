# 概况统计相关接口

## 接口地址
 
[http://emkt.sfaessentials.com/aj/statistics/general/Frequency]
(http://emkt.sfaessentials.com/aj/statistics/general/Frequency)

## 接口描述

> 概况统计接口


## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| company_id | true | 无| 药厂id|
| type | true | 无| 1  产品，2 Ta|
## 测试url
curl "http://123.56.178.15:8088/aj/statistics/general/Frequency?company_id=1&type=2"
## 响应参数:


## 响应数据(JSON):
> 成功

```javascript
 {
    "code": 10000,
    "msg": "Success",
    "data": [
        {
            "name": "测试77727",
            "id": 148986,
            "value": 8
        },
        {
            "name": "对方即可7271",
            "id": 148988,
            "value": 55
        },
        {
            "name": "ceshi0801",
            "id": 148993,
            "value": 22
        },
        {
            "name": "0803",
            "id": 148995,
            "value": 48
        },
        {
            "name": "测试产品长长长长长度才踩踩踩踩踩踩踩踩踩打点踩踩踩踩踩踩踩踩才踩的踩踩踩踩踩从踩踩踩踩踩踩踩踩踩踩踩踩踩踩踩从踩踩踩踩踩踩踩踩踩踩踩踩踩从踩踩踩踩踩踩踩踩踩踩踩踩踩踩踩从",
            "id": 148999,
            "value": 65
        },
        {
            "name": "测试成分长度",
            "id": 149000,
            "value": 136
        },
        {
            "name": "测试810",
            "id": 149002,
            "value": 11
        },
        {
            "name": "测试总花费计算是否正确",
            "id": 149004,
            "value": 3
        },
        {
            "name": "测试统计总花费",
            "id": 149005,
            "value": 6
        },
        {
            "name": "测试0825",
            "id": 149033,
            "value": 29
        }
    ]
}
```
> 失败 

```javascript
{
   code: 10001,
   msg: "输入输出错误",
   data: []
}

```