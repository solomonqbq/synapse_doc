# 获取全部用户资产

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/assets/assetslist]
(http://emkt.sfaessentials.com/v2/aj/assets/assetslist)

## 接口描述

> 获取全部公司资产列表

## 认证方式

> 登录认证

## 请求参数(Get):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
|page | true| 无|页数|
| count | true| 无 |条数 |

##请求接口样例
curl "http://10.90.0.15/v2/aj/assets/rechargelist?page=1&count=10"

## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "Success",
    "data": {
        "total": 20,
        "list": [
            {
                "freeze": 520,
                "company_id": 1111,
                "consum": 10.32,
                "company_name": "",
                "ctime": 1465211870000,
                "cash": 2179.68
            },
            {
                "freeze": 123,
                "company_id": 2,
                "consum": 1113,
                "company_name": "",
                "ctime": 1470885956000,
                "cash": 12823
            },
            {
                "freeze": 620,
                "company_id": 215,
                "consum": 7,
                "company_name": "",
                "ctime": 1466666168000,
                "cash": 21372
            },
            {
                "freeze": 0,
                "company_id": 1001,
                "consum": 0,
                "company_name": "",
                "ctime": 1476013567000,
                "cash": 200000
            },
            {
                "freeze": 210,
                "company_id": 38,
                "consum": 12,
                "company_name": "ceshi0817aa",
                "ctime": 1471510310000,
                "cash": 828,
                "status": 1
            },
            {
                "freeze": 2023,
                "company_id": 37,
                "consum": 19,
                "company_name": "ceshi0817qq",
                "ctime": 1471538766000,
                "cash": 3358,
                "status": 1
            },
            {
                "freeze": 1279,
                "company_id": 39,
                "consum": 133,
                "company_name": "ceshi0818gd",
                "ctime": 1471577621000,
                "cash": 9993,
                "status": 1
            },
            {
                "freeze": 15496,
                "company_id": 41,
                "consum": 112,
                "company_name": "ceshi0830",
                "ctime": 1472529080000,
                "cash": 99995898.99,
                "status": 1
            },
            {
                "freeze": 100,
                "company_id": 69,
                "consum": 0,
                "company_name": "ceshi0926aa",
                "ctime": 1476069586000,
                "cash": 9999900,
                "status": 1
            },
            {
                "freeze": 100,
                "company_id": 68,
                "consum": 0,
                "company_name": "ceshi0926cc",
                "ctime": 1475215100000,
                "cash": 89989822,
                "status": 1
            }
        ]
    }
}
```
> 失败 

```javascript
{
   code: 10001,
   msg: "输入输出错误",
   data: false
}        
```