# 概况统计相关接口

## 接口地址
 
[http://emkt.sfaessentials.com/v2/aj/statistics/general/trend]
(http://emkt.sfaessentials.com/statistics/general/trend)

## 接口描述

> 概况统计接口


## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| company_id | true | 无| 药厂id|
| range | true | 无| 1 当天，2 昨天，3 过去7天，4 过去30天|
| type | true | 无| 1 pv，2 uv|
## 测试url
curl "http://123.56.178.15:8088/v2/aj/statistics/general/trend?company_id=11&range=4&type=1"
## 响应参数:


## 响应数据(JSON):
> 成功

```javascript
{
      code:10000,
      msg:"success",
      data:[
//PV统计数据 {
                 id:"1",
                 name:"PV", //图例名称 data:[
                { "step": 0, "count": 7 }, //step对应折线图横坐标【坐标点间隔】,选今天和昨天, 间隔为1小时;过去7天和过去30天,间隔为1天
                  { "step": 1, "count": 6 },
                  { "step": 2, "count": 9 },
                  { "step": 3, "count": 14 },
                  { "step": 4, "count": 18 },
                  { "step": 5, "count": 21 },
                  { "step": 6, "count": 25 },
                  { "step": 7, "count": 26 },
                  { "step": 8, "count": 23 },
                  { "step": 9, "count": 18 },
                  { "step": 10, "count": 13 },
                  { "step": 11, "count": 9 }
] },
//UV统计数据 {
              id: "2",
              name: "UV",
              data: [
                  { "step": 0, "count": 0 },
                  { "step": 1, "count": 0 },
                  { "step": 2, "count": 5 },
                  { "step": 3, "count": 11 },
                  { "step": 4, "count": 17 },
                  { "step": 5, "count": 22 },
                  { "step": 6, "count": 24 },
                  { "step": 7, "count": 24 },
                  { "step": 8, "count": 20 },
                  { "step": 9, "count": 14 },
                  { "step": 10, "count": 8 },
                  { "step": 11, "count": 2 }
] }
] }```
> 失败 

```javascript
{
   code: 10001,
   msg: "输入输出错误",
   data: { }
}

```