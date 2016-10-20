# 概况统计相关接口

## 接口地址

[http://emkt.sfaessentials.com/aj/statistics/qa/answer]
(http://emkt.sfaessentials.com/aj/statistics/qa/answer)

## 接口描述

> 概况统计接口


## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| company_id | true | 无| qaid|
| qa_id | true | 无| qaid|

## 测试url
curl "http://10.90.0.15/v2/aj/statistics/general/answer?qa_id=2&company_id=32"

## 响应数据(JSON):
> 成功

```javascript
  {
      code:10000,
      msg:"success",
      data:[
             {
                question_id:"xx",
                 header:"题目",
                 stem:"题干",
                 result:[] //由于stem为字符串,故暂不确定后台返回统计结果的数据格式
             }
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