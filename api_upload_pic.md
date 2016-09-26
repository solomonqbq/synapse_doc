# 文件上传相关:上传图片

## 接口地址

[http://emkt.sfaessentials.com/aj/uploadpic]
(http://emkt.sfaessentials.com/aj/uploadpic)

## 接口描述

> 单张pic上传

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| fiel| true | 无| 图片文件|


## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "success",
    "data": {
        "imageurl": "http://emkt.sfaessentials.com/img/upload/20160117/1453003515869.png"
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