# 概况统计相关接口

## 接口地址

[http://emkt.sfaessentials.com/aj/statistics/general/usercount]
(http://emkt.sfaessentials.com/aj/statistics/general/usercount)

## 接口描述

> 概况统计接口


## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| company_id | true | 无| 药厂id|


## 测试url
curl "http://123.56.178.15:8088/aj/statistics/general/usercount?company_id=1"
## 响应参数:


## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "success",
    data: {
             1: {
                     id: 1,
                     name: "高",
                     count: 0
               },
            2: {
                    id: 2,
                    name: "中",
                    count: 1
               },
           3: {
                   id: 3,
                  name: "低",
                  count: 5
            }
        }
    }
```
> 失败 

```javascript
{
   code: 10001,
   msg: "输入输出错误",
   data: { }
}

```