# 用户:C端医生信息转换IDB用户信息

## 接口地址

[http://emkt.sfaessentials.com/api/doctor/init](http://emkt.sfaessentials.com/api/doctor/init)

## 接口描述

> C端医生信息转换IDB用户信息

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| doctor_id | true | 无 | C端医生id | 
| name | false | 无 | C端医生名称|
| city_id | true | 无 | C端定义的市id | 
| hospital_id | true | 无  | C端定义的医院id |
| department_id | true | 无 | C端定义的科室id |
| indications_id | false | 无 | C端定义的适应症id |
| doctor_grade_id | true | 无 | C端定义的医生等级 |
| hospital_grade_id | true | 无| C端定义的医院等级|
| source_id | true | 无 | C端来源id |

## 示例
 curl "http://solin.emkt.sfaessentials.com/api/doctor/init" -d "doctor_id=10011111&source_id=C0001&department_id=1018&city_id=22&doctor_grade_id=9&hospital_grade_id=32&hospital_id=111&province_id=1"

## 响应数据(JSON):
> 成功

```javascript
{"code":10000,"msg":"succ","data":"http:\/\/115.28.133.147:8080\/#!\/menu\/menu\/19"}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"error",
    data:[]
}
```