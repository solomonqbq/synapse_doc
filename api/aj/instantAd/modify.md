# 直通车相关接口:编辑接口

## 接口地址

[http://emkt.sfaessentials.com/aj/instantad/modify](http://emkt.sfaessentials.com/aj/instantad/modify)

## 接口描述

> 编辑直通车接口

## 认证方式

> 登录认证

## 请求参数(POST,JSON):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| id | integer | true | 无 | QA id | 
| type | integer | true | 无 | 类型，资讯：1，QA:2 | 
| subject_id | integer | true | 无  | 直通车推广id |
| sheet_id | integer | true | 无  |  直通车类型id，通过直通车形式列表接口获取的id |
| name | string | true | 无 | 直通车名称 |
| desc |  string | true | 无 | 直通车描述 |
| image |  string | true | 无 | 直通车图片 |
| begin_time |  string | true | 无 | 开始时间 |
| end_time |  string | true | 无 | 结束时间 |
| threshold |  integer | true | 无 | 提醒阈值 |
| status |  integer | true | 无 | 状态，全局统一 |

>示例
```javascript
  {"id":102,"type":4,"subject_id":240,"sheet_id":2,"name":"ceshi修改","desc":"ceshi","image":"http://emkt.sfaessentials.com/images/upload/20161011/1476174772497.png","begin_time":1476155606000,"end_time":1476157606000,"threshold":999,"status":1}
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
    error_code:10001,
    error:"新建资讯失败",
    data:false
}
```