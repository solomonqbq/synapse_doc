# 信息点相关接口:信息点详情接口

## 接口地址

[http://emkt.sfaessentials.com/v2/aj/keyword/info](http://emkt.sfaessentials.com/v2/aj/keyword/info)

## 接口描述

> 信息点详情接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| keyword_id | true | 无 | 信息点id | 


## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "success",
    "data": {
        "id": "55",
        "keyword": "kp001",
        "description": "keyword01",
        "status": "1",
        "company_id": "1",
        "create_user": "1",
        "insert_time": "2016-05-31 11:23:45",
        "update_time": "2016-05-31 11:23:45",
        "relate_product": [
            {
                "id": "148927",
                "cn_name": "产品名称11210",
                "en_name": "英文名称0",
                "general_name": "通用名",
                "image": "",
                "ingredient": "成分成分成分成分成分成分成分成分成分成分成分成分成分成分成分成分成分成分成分成分成分成分成分成分成分成分成分成分0",
                "adaptation": "治疗领域治疗领域治疗领域治疗领域治疗领域治疗领域治疗领域治疗领域治疗领域治疗领域治疗领域治疗领域治疗领域治疗领域治疗领域治疗领域治疗领域治疗领域治疗领域0",
                "usage": "用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用量用法用0",
                "reactions": "不良反应不良反应不良反应不良反应不良反应不良反应不良反应不良反应不良反应不良反应不良反应不良反应不良反应不良反应不良反应不良反应不良反应0",
                "taboos": "配方禁忌配方禁忌配方禁忌配方禁忌配方禁忌配方禁忌配方禁忌配方禁忌配方禁忌配方禁忌配方禁忌配方禁忌配方禁忌配方禁忌配方禁忌配方禁忌配方禁忌配方禁忌配方禁忌0",
                "matters": "注意事项注意事项注意事项注意事项注意事项注意事项注意事项注意事项注意事项注意事项注意事项注意事项注意事项注意事项注意事项0",
                "classification": "药物分类药物分类药物分类药物分类药物分类药物分类药物分类药物分类药物分类药物分类药物分类药物分类药物分类药物分类药物分类药物分类药物分类0",
                "price": "111110.00",
                "insurance_type": "0",
                "status": "1",
                "otc": "0",
                "corporation": "",
                "department": "",
                "company_id": "1",
                "create_user": "1",
                "listing_time": "0000-00-00 00:00:00",
                "insert_time": "2016-05-24 15:50:44",
                "update_time": "2016-05-30 15:16:18"
            },
            {
                "id": "148928",
                "cn_name": "测试产品1111",
                "en_name": "英文名",
                "general_name": "333",
                "image": "",
                "ingredient": "",
                "adaptation": "",
                "usage": "",
                "reactions": "",
                "taboos": "",
                "matters": "",
                "classification": "",
                "price": "33.00",
                "insurance_type": "1",
                "status": "1",
                "otc": "1",
                "corporation": "",
                "department": "",
                "company_id": "1",
                "create_user": "1",
                "listing_time": "0000-00-00 00:00:00",
                "insert_time": "2016-05-30 16:34:36",
                "update_time": "2016-05-30 16:34:36"
            },
            {
                "id": "148929",
                "cn_name": "产品名称1",
                "en_name": "namq",
                "general_name": "通用名0",
                "image": "",
                "ingredient": "",
                "adaptation": "",
                "usage": "",
                "reactions": "",
                "taboos": "",
                "matters": "",
                "classification": "",
                "price": "66.00",
                "insurance_type": "0",
                "status": "1",
                "otc": "1",
                "corporation": "",
                "department": "",
                "company_id": "1",
                "create_user": "1",
                "listing_time": "0000-00-00 00:00:00",
                "insert_time": "2016-05-30 16:36:02",
                "update_time": "2016-05-30 16:36:02"
            }
        ],
        "relate_ta": [
            {
                "id": "1",
                "name": "aaaaa",
                "description": "",
                "company_id": "1",
                "create_user": "1",
                "create_time": "2016-05-13 00:00:00",
                "status": "0"
            },
            {
                "id": null,
                "name": null,
                "description": null,
                "company_id": null,
                "create_user": null,
                "create_time": null,
                "status": null
            },
            {
                "id": null,
                "name": null,
                "description": null,
                "company_id": null,
                "create_user": null,
                "create_time": null,
                "status": null
            }
        ],
        "relate_essay_total": 0
    }
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"获取信息点详情失败",
    data:false
}
```
