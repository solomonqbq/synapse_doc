# 推广相关接口:推广覆盖区域接口

## 接口地址

[http://emkt.sfaessentials.com/aj/promotion/includings](http://emkt.sfaessentials.com/aj/promotion/includings)

## 接口描述

> 推广覆盖区域接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| id | integer | true | 无 | 推广id | 


## 响应数据(JSON):
> 成功

```javascript
{
code: 10000,
msg: "success",
data: [
{
id: "10",
type: "1",
subject_id: "1001",
category: "1",
promotion_id: "301",
name: "华东地区",
index: "R1001"
}
]
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