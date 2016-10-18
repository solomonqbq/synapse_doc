# IDB向杏仁推送推广


## 接口地址
>推送的杏仁地址(正式环境)
[http://xingren.com/api/promotion/add](http://xingren.com/api/promotion/add)
>预发布环境
[http://yisheng.aihaisi.com/api/promotion/add](http://yisheng.aihaisi.com/api/promotion/add)

## 接口描述

>  IDB向杏仁推送推广


## 测试请求
>


## 认证方式

> POST（form-urlencoded）


##杏仁要求的 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| token| true| 无 | 双方约定的固定token值PIpTm4EtGe7J| 
| pic | true| 无 | Banner（640x348），Timeline（598x200），闪屏（750x1334）| 
| title| true| 无 | Banner标题 | 
| url| true| 无 |跳转链接  | 
|summary(string)| false| 无 | 推广内容概要,不填默认和title一样| 
| sourcePid| true| 无 | Synapse 平台推广id，用于标识该条推广的唯一性，用于后续统计曝光时，作为参数传递 | 
|position| true| 无 |推广位置，0-首页Timeline，1-Banner，2-闪屏 | 
| provinceIds(string)| true| 无 |C端省id | 
| hospitalIds(string)| true| 无 |C端医院id | 
| hospitalLevelIds(string)| true| 无 |C端医院等级id | 
| departmentIds(string)| true| 无 |C端科室id | 
| doctorTitleIds(string) true| 无 |C端适应症id | 


##杏仁响应数据(JSON):
> 成功

```javascript
{"success":true}
```
> 失败 

```javascript
{
    "success": false,
    "code": 100,
    "msg": "不合法的provinceIds参数"
}
```