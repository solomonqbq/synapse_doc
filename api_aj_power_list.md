# 功能权限列表

## 接口地址

[http://emkt.sfaessentials.com/aj/group/powerlist](http://emkt.sfaessentials.com/aj/group/powerlist)

## 接口描述

> 功能权限列表


## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 



## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
             {
                power_id: "35",
                power_name: "产品管理",
              
            },
       
         {
                power_id: "36",
                power_name: "咨询管理",
              
            },
    }
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"error",
    data:false
}
```