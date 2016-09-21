# 详情页面答卷相关接口:答卷接口

## 接口地址

[http://emkt.sfaessentials.com/v2/api/subject/qa/survey](http://emkt.sfaessentials.com/v2/api/subject/qa/survey)

## 接口描述

> 答卷接口

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| qa_id | int | true | 无 | 问卷id | 
| list | json | true | 无 |答题相关信息 | 

> 参数说明
```javascript
{
    "list":
    [ 
      {
        "question_id": "",//问题id
        "answer": "", //用户输入内容
        "user": ""，//用户id 
        }
     ],
    qa_id:165

｝
  
```

## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "Success",
   data:  [],
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"新建资讯失败",
    data:null
}
```