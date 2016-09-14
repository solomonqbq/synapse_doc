# 产品相关接口:编辑接口

## 接口地址

[http://emkt.sfaessentials.com/aj/product/edit](http://emkt.sfaessentials.com/aj/product/edit)

## 接口描述

> 产品编辑接口

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
|product_id| true| 无| 产品唯一ID|
| cn_name | false | 无 | 中文名 | 
| en_name | false | 无  | 英文名 |
| general_name | true | 无 | 通用名 |
| image | | false | 无 | 产品图片地址 |
| ingredient | false | 无 | 成分 |
| adaptation | false | 无 | 适应症/治疗领域 |
| usage | false | 无 | 用法用量 |
| reactions | false | 无 | 不良反应 |
| taboos | false | 无 | 禁忌 |
| matters | false | 无 | 注意事项 |
| classification | false | 无 | 药物分类|
| department | false | 无 | 科室id，通过","隔开 | 
| listing_time | false | 无 | 上市日期 |
| price | false | 无 | 价格 |
| status | false | 无 | 0:禁用，1:启用 |
| insurance_type | false | 无 | 医保类型 |
| otc | false | 无 | 状态(0:处方药, 1:非处方药) |


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
    error:"新建产品失败",
    data:false
}
```