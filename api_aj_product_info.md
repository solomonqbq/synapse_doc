# 产品相关接口:产品详情接口

## 接口地址

[http://emkt.sfaessentials.com/aj/product/info](http://emkt.sfaessentials.com/aj/product/info)

## 接口描述

> 产品详情接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| product_id | true | 无 | 产品id | 


## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        id: "47",
        cn_name: "丁林美",
        en_name: "Clindamycin Phosphate Injection",
        general_name: "克林霉素磷酸酯注射液",
        ingredient: "克林霉素磷酸酯<br/> ",
        adaptation: "革兰氏阳性菌引起的下列各种感染性疾病：1．扁桃体炎、化脓性中耳炎、鼻窦炎等。2．急性支气管炎、慢性支气管炎急性发作、肺脓肿和支气管扩张合并感染等。3．皮肤和软组织感染：疖、痈、脓肿、蜂窝组织炎、创伤、烧伤和手术后感染等。4．泌尿系统感染：急 ...",
        usage: "成人：深部肌肉注射或静脉滴注给药：中度感染：0.6－1.2g日，分2、3、4等剂量，每12、8、6小时一次。严重感染：1.2－2",
        reactions: "国外文献显示，克林霉素磷酸酯注射剂不良反应情况如下：1．胃肠道反应：常见恶心、呕吐、腹痛、腹泻等；严重者有腹绞痛、腹部压痛、严重",
        taboos: "本品与林可霉素、克林霉素有交叉耐药性，对克林霉素或林可霉素有过敏史者禁用。<br/> ",
        matters: "和青霉素、头孢菌素类抗生素无交叉过敏反应，可用于对青霉素过敏者。 <br/> 与氨苄青霉素、苯妥英、巴比妥盐酸盐、氨茶碱、葡萄糖",
        price: "0",
        insurance_type: "0",
        status: "1",
        otc: "0",
        corporation: "",
        department: "",
        folder_id: "0",
        group_id: "0",
        create_user: "0",
        listing_time: "2016-01-18 20:32:49",
        insert_time: "2016-01-04 17:34:13",
        update_time: "0000-00-00 00:00:00"
    }
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"新建产品失败",
    data:false
}
```
