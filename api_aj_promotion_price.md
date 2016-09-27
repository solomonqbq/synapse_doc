# 推广相关接口:推广价目列表接口

## 接口地址

[http://emkt.sfaessentials.com/aj/promotion/price](http://emkt.sfaessentials.com/aj/promotion/price)

## 接口描述

> 推广价目表

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| type | integer | true | 1 | 资讯推广:1, QA推广:2 ,点播:3, 直播:4|

## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: [
        {
            id: "1",
            name: "三级主任医师",
            type: "0",
            cpc: "6"
        },
        {
            id: "2",
            name: "二级主任医师",
            type: "0",
            cpc: "6"
        },
        {
            id: "3",
            name: "三级主治医师",
            type: "0",
            cpc: "6"
        },
        {
            id: "4",
            name: "二级主治医师",
            type: "0",
            cpc: "6"
        },
        {
            id: "5",
            name: "三级医师",
            type: "0",
            cpc: "6"
        },
        {
            id: "6",
            name: "二级医师",
            type: "0",
            cpc: "6"
        },
        {
            id: "7",
            name: "其他",
            type: "0",
            cpc: "6"
        }
    ]
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"操作失败",
    data:false
}
```