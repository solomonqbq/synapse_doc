# 概况统计相关接口

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/statistics/general/info]
(http://emkt.sfaessentials.com/v2/aj/statistics/general/info)

## 接口描述

> 概况统计接口


## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| company_id | true | 无| 药厂id|
| range | true | 无| 1 当天，2 全部|

## 测试url
curl "http://123.56.178.15:8088/v2/aj/statistics/general/info?company_id=11&range=2"
## 响应参数:


## 响应数据(JSON):
> 成功

```javascript
   {
      code:10000,
      msg:"success",
      data:{
              cover_count:1000, //覆盖次数 
              total_cost:10000, //总花费 
             cover_user:1000, //覆盖用户数 
              new_user:1000 //新增用户数
} }
```
> 失败 

```javascript
{
   code: 10001,
   msg: "输入输出错误",
   data: { }
}

```