# 用户相关接口:左侧菜单

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/account/menulist](http://emkt.sfaessentials.com/aj/account/menulist)

## 接口描述

>  左侧菜单

## 认证方式

> 无

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 



## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "success",
    "data": {
        "loginuser": {
            "id": "1",
            "nickname": "aaaa",
            "useremail": "aaaaa",
            "phone": "",
            "avatar": "",
            "group_id": "1",
            "company_id": "1",
            "status": "1",
            "ctime": "0000-00-00 00:00:00",
            "utime": "2016-06-24 00:42:03",
            "company_info": {
                "id": "1",
                "name": "aaaaaa",
                "create_user": "1",
                "ctime": null,
                "licence": null,
                "status": null
            },
            "company_manager": 1,
            "auth": {
                "products": [
                    "148937"
                ],
                "tas": [
                    "19",
                    "18"
                ],
                "powers": [
                    "10002",
                    "10004",
                    "11111"
                ]
            }
        },
        "menulist": {
            "1": {
                "name": "概况",
                "url": "",
                "power": "0"
            },
            "2": {
                "name": "基础数据",
                "url": "",
                "power": "0",
                "subchild": {
                    "0": {
                        "name": "产品管理",
                        "power": "10001",
                        "url": ""
                    },
                    "1": {
                        "name": "信息点管理",
                        "power": "10002",
                        "url": ""
                    },
                    "3": {
                        "name": "治疗领域管理",
                        "power": "10003",
                        "url": ""
                    }
                }
            },
            "3": {
                "name": "推广中心",
                "url": "",
                "power": "0",
                "subchild": [
                    {
                        "name": "医学资讯",
                        "power": "10004",
                        "url": ""
                    },
                    {
                        "name": "问卷调查",
                        "power": "10005",
                        "url": ""
                    },
                    {
                        "name": "医学视频",
                        "power": "10006",
                        "url": ""
                    }
                ]
            },
            "4": {
                "name": "直通车",
                "url": "",
                "power": "0",
                "subchild": [
                    {
                        "name": "直通车管理",
                        "power": "10007",
                        "url": ""
                    }
                ]
            },
            "5": {
                "name": "设置",
                "url": "",
                "power": "0",
                "subchild": [
                    {
                        "name": "权限设置",
                        "power": "10008",
                        "url": ""
                    },
                    {
                        "name": "账户充值",
                        "power": "10009",
                        "url": ""
                    }
                ]
            }
        }
    }
}
```
> 失败 

```javascript
{
   code:10001,
    msg:"系统失败",
    data:{}
}
```
