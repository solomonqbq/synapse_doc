# 用户资产相关:增加用户资产

## 接口地址

[http://emkt.sfaessentials.com/aj/assets/rechargelist]
(http://emkt.sfaessentials.com/aj/assets/rechargelist)

## 接口描述

> 获取用户充值记录

## 认证方式

> 登录认证

## 请求参数(Get):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| uid | true | 无| 公司uid|
|page | true| 无|页数|
| count | true| 无 |条数 |

##请求接口样例
curl "http://10.90.0.15/v2/aj/assets/rechargelist?uid=1001&page=1&count=10"

## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "success",
    "data": {
        "list":[
          {
             "id":"1",
             "company_id":"1001",//充值id
             "adminemail":"aaa",//b端操作人
             "cash":"141.00",  //充值金额
             "ctime":"2016-06-02 21:33:52",//充值时间
             "desc":""//充值备注
            },  
           ],
         "total":30 //用于前端分页展示       
    }   
}
```
> 失败 

```javascript
{
   code: 10001,
   msg: "输入输出错误",
   data: false
}        
```