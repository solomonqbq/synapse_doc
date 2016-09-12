# 菜单

## 接口地址

[http://emkt.sfaessentials.com/v2/api/menu/list](http://emkt.sfaessentials.com/api/menu/list)

## 接口描述

> 获取菜单列表

## 认证方式

> 非登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| request_id | true | 无 | 请求 id | 




## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "Success",
    "data": {
        "data": [
            {
                "id": 1,
                "name": "医学资讯",
                "grade": 1
            },
            {
                "id": 2,
                "name": "内容专题",
                "grade": 1
            },
            {
                "id": 3,
                "name": "在线问答",
                "grade": 1
            },
            {
                "id": 4,
                "name": "线上科室会",
                "grade": 1
            },
            {
                "id": 5,
                "name": "文献检索",
                "grade": 1
            },
            {
                "id": 6,
                "name": "问卷调查",
                "grade": 1
            },
            {
                "id": 7,
                "name": "积分商城",
                "grade": 1
            },
            {
                "id": 8,
                "name": "投票抽奖",
                "grade": 1
            },
            {
                "id": 9,
                "name": "辩论台",
                "grade": 1
            },
            {
                "id": 10,
                "name": "病例分享",
                "grade": 1
            },
            {
                "id": 11,
                "name": "闯关",
                "grade": 1
            },
            {
                "id": 12,
                "name": "用药助手",
                "grade": 1
            },
            {
                "id": 13,
                "name": "计算工具",
                "grade": 1
            }
        ],
        "total": 13
    }
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"菜单数据为空",
    data:null
}
```