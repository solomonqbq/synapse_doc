# 产品相关接口:产品列表接口

## 接口地址

[http://emkt.sfaessentials.com/aj/product/list](http://emkt.sfaessentials.com/aj/product/list)

## 接口描述

> 产品列表接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| page | false | 1 | 数据页数 | 
| count | false | 20 | 每页数据量 |
| order | false | 无 | 排序字段 | 
| order_type | false | asc | 排序类型(asc,desc) | 



## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        data: [
            {
                id: "35",
                cn_name: "乙酰螺旋霉素片",
                en_name: "Acetylspiramycin Tablets",
                general_name: "乙酰螺旋霉素片",
                image:"http://xxxxxx",
                ingredient: "本品为单乙酰螺旋霉素Ⅱ、单乙酰螺旋霉素Ⅲ、双乙酰螺旋霉素Ⅱ和双乙酰螺旋霉素Ⅲ四个组分为主的混合物。",
                adaptation: "适用于敏感葡萄球菌、链球菌属和肺炎链球菌所致的轻、中度感染，如咽炎、扁桃体炎、鼻窦炎、中耳炎、牙周炎、急性支气管炎、慢性支气管炎急性发作、肺炎、非淋菌性尿道炎、皮肤软组织感染，亦可用于隐孢子虫病、或作为治疗妊娠期妇女弓形体病的选用药物。",
                usage: "成人剂量：一次2-3片，一日4次，首次加倍。<br/> 小儿剂量：每日按体重20-30mg/kg，分4次服用。",
                reactions: "病人对本品耐受性良好，不良反应主要为腹痛、恶心、呕吐等胃肠道反应，常发生于大剂量用药时，程度大多轻微，停药后可自行消失。变态反应",
                taboos: "对本品、红霉素及其他大环内酯类过敏的患者禁用。",
                matters: "1. 由于肝胆系统是乙酰螺旋霉素排泄的主要途径，故严重肝功能不全患者慎用本品。<br/> 2. 轻度肾功能不全患者不需作剂量调整",
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
                update_time: "2016-01-06 19:26:14"
            },
            {
                id: "47",
                cn_name: "丁林美",
                en_name: "Clindamycin Phosphate Injection",
                general_name: "克林霉素磷酸酯注射液",
                image:"http://xxxxxx",
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
        ],
        total: 31887,
        
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