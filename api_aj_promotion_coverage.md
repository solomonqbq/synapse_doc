# 推广相关接口:推广覆盖接口

## 接口地址

[http://emkt.sfaessentials.com/aj/promotion/coverage](http://emkt.sfaessentials.com/aj/promotion/coverage)

## 接口描述

> 推广覆盖接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| type | integer | true | 无 | 1:区域，2:医院等级，3:科室, 4:医生等级 |


## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        list: [
            {
                id: "0",
                index: "",
                name: "全部区域"
            },
            {
                id: "1001",
                index: "R1001",
                name: "华东地区"
            },
            {
                id: "1002",
                index: "R1002",
                name: "华南地区"
            },
            {
                id: "1003",
                index: "R1003",
                name: "华中地区"
            },
            {
                id: "1004",
                index: "R1004",
                name: "华北地区"
            },
            {
                id: "1005",
                index: "R1005",
                name: "西北地区"
            },
            {
                id: "1006",
                index: "R1006",
                name: "西南地区"
            },
            {
                id: "1007",
                index: "R1007",
                name: "东北地区"
            },
            {
                id: "1008",
                index: "R1008",
                name: "台港澳地区"
            }
        ],
        total: 9
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