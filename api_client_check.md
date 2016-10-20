# c端点击检测接口:用于检测c端曝光情况

## 接口地址

[http://emkt.sfaessentials.com/v2/openapi/{companyId}/ads/check](http://emkt.sfaessentials.com/v2/openapi/{companyId}/ads/check)

## 接口描述

> c端点击检测接口

## 认证方式

> 登录认证

## 请求参数(get):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| ad_id| int| true | 无  | 推广资源id |
| user_id| string| true| 无  |  用户id |
| bid| string | true | 无 | 合作方请求资源唯一标识 ，与获取广告资源里的 bid一致|

>示例
```javascript
emkt.sfaessentials.com/v2/openapi/{companyId}/ads/check?ad_id=12&user_id=45e4e&bid=fewaf2

## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "Success",
   data:  true,
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"检测提交失败",
    data:false
}
```