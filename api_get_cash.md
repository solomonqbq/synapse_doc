# 用户资产相关接口:获取单个用户资产接口

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/assets/get]
(http://emkt.sfaessentials.com/v2/aj/assets/get)

## 接口描述

> 获取单个用户资产接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
|company_id | integer | true | 无 | 公司id | 

## 返回参数说明:

| 参数 |  描述 | 
| ---- | ---- |
|company_id | 用户uid | 
|cash |帐号的可用金额 | 
|freeze | 帐号的冻结金额 |
|consum | 帐号的累计消费金额 |
## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
          company_id: "302",
         cash: "3000.99",
         freeze: "1000.99"
         consum:"1876.88"
     }
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