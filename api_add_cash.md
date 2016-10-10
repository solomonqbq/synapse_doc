# 用户资产相关:增加用户资产

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/assets/add]
(http://emkt.sfaessentials.com/v2/aj/assets/add)

## 接口描述

> 增加用户资产

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| company_id | true | 无| 公司id|
|email | true | 无|后台操作者email|
| cash | true | 无 | 金额|


## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "success",
    "data": true
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