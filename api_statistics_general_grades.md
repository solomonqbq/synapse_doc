# 概况统计相关接口

## 接口地址
 
[http://emkt.sfaessentials.com/aj/statistics/general/grades]
(http://emkt.sfaessentials.com/aj/statistics/general/grades)

## 接口描述

> 概况统计接口


## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| company_id | true | 无| 药厂id|
| type | true | 无| 1  医院分级，2医生分级 |
## 测试url
curl "http://123.56.178.15:8088/aj/statistics/general/grades?company_id=11&type=1"
## 响应参数:


## 响应数据(JSON):
> 成功

```javascript
 {
      code:10000,
      msg:"success",
      data:[
         {id:"1",name:"产品1",value:120}, //后台返回数值即可(无需百分比) {id:"2",name:"产品2",value:223},
         {id:"3",name:"产品3",value:334},
         {id:"4",name:"产品4",value:443},
          {id:"5",name:"产品5",value:133} ]
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