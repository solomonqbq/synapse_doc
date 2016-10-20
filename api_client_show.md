# c端曝光检测接口:用于检测c端曝光情况

## 接口地址

[http://emkt.sfaessentials.com/v2/openapi/{companyId}/ads/show](http://emkt.sfaessentials.com/v2/openapi/{companyId}/ads/show)

## 接口描述

> c端曝光量检测接口

## 认证方式

> 登录认证

## 请求参数(get):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| companyId| string| true | 无 | c端的唯一标识| 
| adId| int| true | 无  | 推广资源id |
| userId| string| false| 无  |  用户id |
| bid| string | true | 无 | c端请求资源唯一标识 |

>示例
```javascript
emkt.sfaessentials.com/api/ad/show?companyId=00023&adId=12&userId=45e4e&bid=fewaf2

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
    error_code:10001,
    error:"检测提交失败",
    data:false
}
```