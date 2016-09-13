# 权限组详细信息接口

## 接口地址

[http://emkt.sfaessentials.com/aj/group/info](http://emkt.sfaessentials.com/aj/group/info)

## 接口描述

> 权限组详细信息

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| group_id | true | 无 | 权限组id | 


## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        auth:
             { powers:
               products:
               tas:
  　　　　{count:
                        data:
                      }
             }
       company_id:
        id: "47",
       create_time:
       create_user:(所有AdminUser10项信息+company_manager,company_info,company_info包括6项信息)
      description:
       id:
      name:
      status:
      type: 
    }
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"获取权限组详情失败",
    data:false
}
```
