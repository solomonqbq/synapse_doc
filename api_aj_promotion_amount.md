# 推广覆盖受众数（第三方接口实时获取）

## 接口地址

[http://123.56.178.15/api/promotion/amount](http://123.56.178.15/api/promotion/amount)

## 接口描述

> 推广覆盖受众数（第三方接口实时获取）

## 测试请求
>  curl -XPOST 'http://123.56.178.15/api/promotion/amount' -d 'province=[{"id":"1001","index":"R1001","name":"华东地区","selected":true}]&hospital_grade=[{"id":"2","index":"L02","name":"一级乙等","selected":true}]&department=[{"id":"0","parent_id":"0","index_id":"K00","name":"全部科室","type":"0","status":"0","selected":true}]&doctor_grade=[{"id":"6","index":"P06","grade":"教授","selected":true},{"id":"7","index":"P07","grade":"副教授","selected":true},{"id":"8","index":"P08","grade":"讲师","selected":true}]';
{"code":10000,"msg":"success","data":259}%                        


## 认证方式

> 非登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| province | true | 无 | 城市 | 
| hospital_grade | true | 无 | 医院级别 | 
| department | true | 无 | 科室 | 
| doctor_grade | true | 无 | 医生职级 | 


## 响应数据(JSON):
> 成功

```javascript
{"code":10000,"msg":"success","data":80532}
```
> 失败 

```javascript

```