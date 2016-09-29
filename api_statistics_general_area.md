# 概况统计相关接口

## 接口地址
 
[http://emkt.sfaessentials.com/aj/statistics/general/area]
(http://emkt.sfaessentials.com/aj/statistics/general/area)

## 接口描述

> 概况统计接口


## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| company_id | true | 无| 药厂id|
| range | true | 无| 1 当天，2 昨天，3 过去7天，4 过去30天|
| type | true | 无| 1 pv， 2 uv 单选|
## 测试url
curl "http://123.56.178.15:8088/aj/statistics/general/area?company_id=11&range=2"
## 响应参数:


## 响应数据(JSON):
> 成功

```javascript
{
    code:10000,
    msg:"success",
    data:[
           {id:"1",name:"北京",value:23390}, 
           {id:"2",name:"天津",value:23390},
   ]

 }

```
> 失败 

```javascript
{
   code: 10001,
   msg: "输入输出错误",
   data: { }
}

```