# IDB向医联推送推广（闪屏）


## 接口地址
###推送的医联地址
[http://app.v3.medlinker.com/rest/v1/openapi/splash/add](http://app.v3.medlinker.com/rest/v1/openapi/splash/add)
###idb接口地址

## 接口描述

> C端推广位访问记录创建（C端一次性同步多条记录）

## 测试请求
>

## 认证方式
POST

> 非登录认证

##医联要求的 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| picOne | false| 无 | 图片1 ios（640*960）| 
| picTwo| false| 无 | 图片2 ios（640*1136） | 
| picThree| false| 无 | 图片3  ios（750*1334）| 
| picFour| false| 无 | 图片4 ios（ 1242*2208 ） | 
| picFive| false| 无 | 图片5 android（720*1280 ）| 
| title| true| 无 | 闪屏标题 | 
| url| true| 无 |跳转链接  | 
| checkNum| true| 无 | 校验参数 | 
| promotion_id| true| 无 | Synapse 平台推广id，用于标识该条推广的唯一性，用于后续统计曝光时，作为参数传递 | 
| province_id| true| 无 |C端省id | 
| hospital_id| true| 无 |C端医院id | 
| hospital_grade_id| true| 无 |C端医院等级id | 
| department_id| true| 无 |C端科室id | 
| indications_id| true| 无 |C端适应症id | 
| doctor_grade_id| true| 无 |C端医生等级id| 
|source_id| true| 无 |来源id,用于区分C端来。比如C端调用接口时，source_id=C0002 | 

## 医联响应数据(JSON):
> 成功

```javascript
{"errcode":0,"msg":"success"}
```
> 失败 

```javascript
{
    errcode:2,
    msg:"系统错误 "
}
{
    errcode:4000001,
    msg:"添加失败 "
}
{
    errcode:4000002,
    msg:"图片格式有误 "
}
{
    errcode:4000003,
    msg:"校验错误 "
}
```