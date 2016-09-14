# 产品相关接口:根据科室查询文献

## 接口地址

[http://emkt.sfaessentials.com/v2/api/subject/essay/list](http://emkt.sfaessentials.com/v2/api/subject/essay/list)

## 接口描述

> 根据科室查询内容

## 认证方式

> false



## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| idb_department_id | false | 无 | IDB系统的科室ID | 
| request_id| true | 无| c端初始化请求时得到到request_id|
| page | false | 1 | 数据页数 | 
| count | false | 20 | 每页数据量 |


## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        list: [
            {
                type: "1",
                id: "60",
                title: "测试02",
                image: "http://emkt.sfaessentials.com/images/upload/20160623/14666716554948.png"
            },
            {
                type: "2",
                id: "63",
                title: "测试问答",
                image: "http://emkt.sfaessentials.com/images/upload/20160623/14666782185331.png"
            }
        ],
        total: 2
    }
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"error",
    data:null
}
```