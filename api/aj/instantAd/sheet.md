# 直通车相关接口:形式列表接口

## 接口地址

[http://emkt.sfaessentials.com/aj/instantad/sheet](http://emkt.sfaessentials.com/aj/instantad/sheet)

## 接口描述

> 形式列表接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 


## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        list: [
            {
                id: "1",
                category: "1",
                name: "推广至 App Loading Page",
                desc: "推广至 App Loading Page",
                image: "",
                price: "999"
            },
            {
                id: "2",
                category: "2",
                name: "推广至应用内轮播图",
                desc: "推广至应用内轮播图",
                image: "",
                price: "999"
            },
            {
                id: "3",
                category: "3",
                name: "推广至应用 Feeds",
                desc: "推广至应用 Feeds",
                image: "",
                price: "999"
            }
        ],
        total: 3
    }
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