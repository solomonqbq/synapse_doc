# 资讯相关接口:新建接口

## 接口地址

[http://emkt.sfaessentials.com/aj/essay/add](http://emkt.sfaessentials.com/aj/essay/add)

## 接口描述

> 新建资讯接口

## 认证方式

> 登录认证

## 请求参数(POST):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| essay | json | true | 无 | 资讯相关信息 | 
| content | json | true | 无  | 资讯内容 |
| promotion | json | true | 无 | 资讯管理推广信息 |
| relates |  json | true | 无 | 资讯关联产品/TA/信息点 |
| includings |  json | true | 无 | 推广覆盖面 |

> 参数说明
```javascript
{
    "essay": {
        "title": "",
        "image": "",
        "periodical": "",
        "author": "",
        "status": "",
        "source": "",
        "release_time": "2016-09-12 11:43:02",
        "tags": ""
    },
    "content": {
        "content_cn": "",
        "content_en": ""
    },
    "promotion": {
        "template_id":"-1" // -1为新增模板
        "template_name":"模板名称" // 当template_id = -1 是此参数为必填，否则为选填
        "threshold": 0,
        "begin_time": "2016-09-12 11:43:02",
        "end_time": "2016-09-12 11:43:02",
        "coverage" : 1111, //覆盖人数
    },
    "relates": [
        {
            "relate_type": "",  // 关联类型(产品:1、TA:2、信息点:3)
            "relate_id": ""
        }
    ],
    "includings": [{
        "category": "", // 覆盖区域类型(区域:1, 医院等级:2 ,科室:3, 医生等级: 4)
        "subject_id":""
    }]
}
```

```HTTP
POST /aj/essay/add HTTP/1.1
Content-Type: application/x-www-form-urlencoded
Host: *
Connection: close
User-Agent: *
Content-Length: 697

essay=%7B%22title%22%3A%22%E6%B5%8B%E8%AF%95%22%2C%22image%22%3A%22www.baidu.com%22%2C%22periodical%22%3A%22%E6%B5%8B%E8%AF%95%22%2C%22author%22%3A%22wantao%22%2C%22source%22%3A%22%E6%B5%8B%E8%AF%95%22%2C%22release_time%22%3A%222015-01-01%22%2C%22tags%22%3A%22%E6%B5%8B%E8%AF%95%22%7D&content=%7B%22content_cn%22%3A%22%E6%B5%8B%E8%AF%95%22%7D&promotion=%7B%22title%22%3A%22%E6%B5%8B%E8%AF%95%E6%8E%A8%E5%B9%BF%22%2C%22image%22%3A%22www.baidu.com%22%2C%22type%22%3A1%2C%22threshold%22%3A100%2C%22begin_time%22%3A%222016-05-24%22%2C%22end_time%22%3A%222016-06-30%22%7D&relates=%5B%7B%22relate_type%22%3A1%2C%22relate_id%22%3A148911%7D%5D&includings=%5B%7B%22type%22%3A1%2C+%22subject_id%22%3A2%7D%5D

```

## 响应数据(JSON):
> 成功

```javascript
{
   code: 10000,
   msg: "Success",
   data:  [],
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"新建资讯失败",
    data:false
}
```