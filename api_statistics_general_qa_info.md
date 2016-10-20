# 概况统计相关接口

## 接口地址

[http://emkt.sfaessentials.com/aj/statistics/qa/info]
(http://emkt.sfaessentials.com/aj/statistics/qa/info)

## 接口描述

> 概况统计接口


## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| company_id | true | 无| 公司id|
| qa_id | true | 无| 问答id|


## 测试url
curl "http://123.56.178.15:8088/aj/statistics/qa/info?company_id=11&qa_id=2"
## 响应参数:


## 响应数据(JSON):
> 成功

```javascript
 {
      code:10000,
      msg:"success",
      data:{
                   total_count:1000, //总份数 
                   anwser_count:10000, //已答份数 
                   total_cost:1000 //总花费
         } 
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