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
| token| true| 无 | 双方约定的固定token值| 
| pic | true| 无 | Banner（640x348），
Timeline，标准图片大小是598x200。不填则没有图片。
如果是闪屏，标准图片大小是750x1334| 
| title| true| 无 | Banner标题 | 
| url| true| 无 |跳转链接  | 
| checkNum| true| 无 | 校验参数 | 
| sourcePid| true| 无 | Synapse 平台推广id，用于标识该条推广的唯一性，用于后续统计曝光时，作为参数传递 | 
|position| true| 无 |推广位置，0-首页Timeline，1-Banner，2-闪屏 | 
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