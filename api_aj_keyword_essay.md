# 信息点相关接口:获取引用信息点的资讯和问答
## 接口地址

[http://emkt.sfaessentials.com/v2/aj/keyword/getrelateessay](http://emkt.sfaessentials.com/v2/aj/keyword/getrelateessay)

## 接口描述

> 获取引用信息点的资讯内容

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
|keyword_id |true | 无| 信息点ID|
| page | false | 1 | 数据页数 | 
| count | false | 20 | 每页数据量 |



## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "success",
    "data": {
        "data": [
            {
                "type": "1",  // 1:资讯，2：问答
                "data": {
                    "id": "59",
                    "title": "测试01",
                    "image": "xxxxxx",
                    "periodical": "期刊测试",
                    "author": "测试工程师",
                    "source": "西安杨森11",
                    "release_time": "2016-06-01 16:48:50",
                    "tags": "测试11",
                    "content_id": "89",
                    "promotion_id": "370",
                    "status": "1",
                    "company_id": "1",
                    "create_user": "1",
                    "insert_time": "2016-06-20 17:14:16",
                    "update_time": "2016-06-20 19:12:44",
                    "content_cn": "<blockquote><ol><li><b>&nbsp;hfas</b></li><li><b>&nbsp;<br>&nbsp; &nbsp;<i> </i></b><i>蓦然回 &nbsp; </i>&nbsp; <b>&nbsp;&nbsp;</b></li><li><b>&nbsp;</b><br><u>&nbsp; 推</u></li><li>&nbsp;<br><strike>&nbsp; 预览</strike></li></ol></blockquote><p><img alt=\"Image\" src=\"https://ss0.bdstatic.com/5aV1bjqh_Q23odCf/static/superman/img/logo/bd_logo1_31bdc765.png\" width=\"540\" height=\"258\"><br></p>",
                    "content_en": null,
                    "begin_time": "2016-06-22 16:48:50",
                    "end_time": "2016-06-25 16:48:50",
                    "template_id": "10",
                    "threshold": "200000",
                    "relates": {
                        "product": [
                            {
                                "id": "148938",
                                "cn_name": "测试11",
                                "en_name": "test 01",
                                "general_name": "通用名测试11"
                            }
                        ],
                        "keyword": [
                            {
                                "id": "250",
                                "keyword": "信息点测试01",
                                "description": "信息点描述"
                            }
                        ]
                    }
                }
            }
        ],
        "count": 6
    }
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"error",
    data:false
}
```