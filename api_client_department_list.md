# 科室列表

## 接口地址

[http://emkt.sfaessentials.com/v2/api/department/list](http://emkt.sfaessentials.com/v2/api/department/list)

## 接口描述

> 全部科室列表

## 认证方式

> 登录认证
## 否

## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 




## 响应数据(JSON):
> 成功

```javascript
{
    "code": 10000,
    "msg": "succ",
    "data": {
        "data": [
            {
                "id": "0",
                "parent_id": "0",
                "index_id": "K00",
                "name": "全部科室",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "0",
                        "parent_id": "0",
                        "index_id": "K00",
                        "name": "全部科室",
                        "type": "0",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "101",
                "parent_id": "101",
                "index_id": "K01",
                "name": "外科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "101",
                        "parent_id": "101",
                        "index_id": "K01",
                        "name": "外科",
                        "type": "0",
                        "status": "0"
                    },
                    {
                        "id": "10101",
                        "parent_id": "101",
                        "index_id": "K0101",
                        "name": "普通外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10102",
                        "parent_id": "101",
                        "index_id": "K0102",
                        "name": "泌尿外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10103",
                        "parent_id": "101",
                        "index_id": "K0103",
                        "name": "胸外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10104",
                        "parent_id": "101",
                        "index_id": "K0104",
                        "name": "骨科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10105",
                        "parent_id": "101",
                        "index_id": "K0105",
                        "name": "甲状腺乳腺外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10106",
                        "parent_id": "101",
                        "index_id": "K0106",
                        "name": "脊柱外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10107",
                        "parent_id": "101",
                        "index_id": "K0107",
                        "name": "关节外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10108",
                        "parent_id": "101",
                        "index_id": "K0108",
                        "name": "小儿外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10109",
                        "parent_id": "101",
                        "index_id": "K0109",
                        "name": "骨肿瘤科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10110",
                        "parent_id": "101",
                        "index_id": "K0110",
                        "name": "足踝外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10111",
                        "parent_id": "101",
                        "index_id": "K0111",
                        "name": "肛肠外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10112",
                        "parent_id": "101",
                        "index_id": "K0112",
                        "name": "心脏外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10113",
                        "parent_id": "101",
                        "index_id": "K0113",
                        "name": "神经外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10114",
                        "parent_id": "101",
                        "index_id": "K0114",
                        "name": "烧伤整形科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10115",
                        "parent_id": "101",
                        "index_id": "K0115",
                        "name": "胃肠外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10116",
                        "parent_id": "101",
                        "index_id": "K0116",
                        "name": "肝脏外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10117",
                        "parent_id": "101",
                        "index_id": "K0117",
                        "name": "胆胰外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10118",
                        "parent_id": "101",
                        "index_id": "K0118",
                        "name": "血管外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10119",
                        "parent_id": "101",
                        "index_id": "K0119",
                        "name": "骨科创伤",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10120",
                        "parent_id": "101",
                        "index_id": "K0120",
                        "name": "运动医学科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10121",
                        "parent_id": "101",
                        "index_id": "K0121",
                        "name": "手外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10122",
                        "parent_id": "101",
                        "index_id": "K0122",
                        "name": "美容整形科",
                        "type": "1",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "102",
                "parent_id": "102",
                "index_id": "K02",
                "name": "内科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "102",
                        "parent_id": "102",
                        "index_id": "K02",
                        "name": "内科",
                        "type": "0",
                        "status": "0"
                    },
                    {
                        "id": "10201",
                        "parent_id": "102",
                        "index_id": "K0201",
                        "name": "神经内科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10202",
                        "parent_id": "102",
                        "index_id": "K0202",
                        "name": "消化内科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10203",
                        "parent_id": "102",
                        "index_id": "K0203",
                        "name": "风湿免疫科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10204",
                        "parent_id": "102",
                        "index_id": "K0204",
                        "name": "感染科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10205",
                        "parent_id": "102",
                        "index_id": "K0205",
                        "name": "老年医学科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10206",
                        "parent_id": "102",
                        "index_id": "K0206",
                        "name": "普通内科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10207",
                        "parent_id": "102",
                        "index_id": "K0207",
                        "name": "呼吸内科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10208",
                        "parent_id": "102",
                        "index_id": "K0208",
                        "name": "肾脏内科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10209",
                        "parent_id": "102",
                        "index_id": "K0209",
                        "name": "内分泌科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10210",
                        "parent_id": "102",
                        "index_id": "K0210",
                        "name": "血液内科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10211",
                        "parent_id": "102",
                        "index_id": "K0211",
                        "name": "心脏内科",
                        "type": "1",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "103",
                "parent_id": "103",
                "index_id": "K03",
                "name": "口腔科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "103",
                        "parent_id": "103",
                        "index_id": "K03",
                        "name": "口腔科",
                        "type": "0",
                        "status": "0"
                    },
                    {
                        "id": "10301",
                        "parent_id": "103",
                        "index_id": "K0301",
                        "name": "牙体牙髓科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10302",
                        "parent_id": "103",
                        "index_id": "K0302",
                        "name": "口腔修复科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10303",
                        "parent_id": "103",
                        "index_id": "K0303",
                        "name": "口腔黏膜科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10304",
                        "parent_id": "103",
                        "index_id": "K0304",
                        "name": "颌面外科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10305",
                        "parent_id": "103",
                        "index_id": "K0305",
                        "name": "正颌科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10306",
                        "parent_id": "103",
                        "index_id": "K0306",
                        "name": "预防口腔科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10307",
                        "parent_id": "103",
                        "index_id": "K0307",
                        "name": "口腔内科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10308",
                        "parent_id": "103",
                        "index_id": "K0308",
                        "name": "牙周科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10309",
                        "parent_id": "103",
                        "index_id": "K0309",
                        "name": "口腔种植科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10310",
                        "parent_id": "103",
                        "index_id": "K0310",
                        "name": "口腔正畸科 ",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10311",
                        "parent_id": "103",
                        "index_id": "K0311",
                        "name": "唇腭裂科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10312",
                        "parent_id": "103",
                        "index_id": "K0312",
                        "name": "颌面创伤科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10313",
                        "parent_id": "103",
                        "index_id": "K0313",
                        "name": "儿童口腔科",
                        "type": "1",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "104",
                "parent_id": "104",
                "index_id": "K04",
                "name": "肿瘤科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "104",
                        "parent_id": "104",
                        "index_id": "K04",
                        "name": "肿瘤科",
                        "type": "0",
                        "status": "0"
                    },
                    {
                        "id": "10401",
                        "parent_id": "104",
                        "index_id": "K0401",
                        "name": "腹部肿瘤科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10402",
                        "parent_id": "104",
                        "index_id": "K0402",
                        "name": "放疗化疗科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10403",
                        "parent_id": "104",
                        "index_id": "K0403",
                        "name": "头颈肿瘤科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10404",
                        "parent_id": "104",
                        "index_id": "K0404",
                        "name": "胸部肿瘤科",
                        "type": "1",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "105",
                "parent_id": "105",
                "index_id": "K05",
                "name": "急诊医学科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "105",
                        "parent_id": "105",
                        "index_id": "K05",
                        "name": "急诊医学科",
                        "type": "0",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "106",
                "parent_id": "105",
                "index_id": "K06",
                "name": "皮肤科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "106",
                        "parent_id": "105",
                        "index_id": "K06",
                        "name": "皮肤科",
                        "type": "0",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "107",
                "parent_id": "107",
                "index_id": "K07",
                "name": "妇产科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "107",
                        "parent_id": "107",
                        "index_id": "K07",
                        "name": "妇产科",
                        "type": "0",
                        "status": "0"
                    },
                    {
                        "id": "10701",
                        "parent_id": "107",
                        "index_id": "K0701",
                        "name": "产科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10702",
                        "parent_id": "107",
                        "index_id": "K0702",
                        "name": "遗传咨询科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10703",
                        "parent_id": "107",
                        "index_id": "K0703",
                        "name": "妇科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10704",
                        "parent_id": "107",
                        "index_id": "K0704",
                        "name": "生殖内分泌科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10705",
                        "parent_id": "107",
                        "index_id": "K0705",
                        "name": "产前诊断科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10706",
                        "parent_id": "107",
                        "index_id": "K0706",
                        "name": "计划生育科",
                        "type": "1",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "108",
                "parent_id": "108",
                "index_id": "K08",
                "name": "儿科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "108",
                        "parent_id": "108",
                        "index_id": "K08",
                        "name": "儿科",
                        "type": "0",
                        "status": "0"
                    },
                    {
                        "id": "10801",
                        "parent_id": "108",
                        "index_id": "K0801",
                        "name": "小儿消化科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10802",
                        "parent_id": "108",
                        "index_id": "K0802",
                        "name": "小儿神经内科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10803",
                        "parent_id": "108",
                        "index_id": "K0803",
                        "name": "小儿肾内科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10804",
                        "parent_id": "108",
                        "index_id": "K0804",
                        "name": "小儿免疫科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10805",
                        "parent_id": "108",
                        "index_id": "K0805",
                        "name": "小儿血液科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10806",
                        "parent_id": "108",
                        "index_id": "K0806",
                        "name": "小儿精神科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10807",
                        "parent_id": "108",
                        "index_id": "K0807",
                        "name": "小儿呼吸科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10808",
                        "parent_id": "108",
                        "index_id": "K0808",
                        "name": "小儿营养保健科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10809",
                        "parent_id": "108",
                        "index_id": "K0809",
                        "name": "小儿心内科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10810",
                        "parent_id": "108",
                        "index_id": "K0810",
                        "name": "小儿内分泌科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10811",
                        "parent_id": "108",
                        "index_id": "K0811",
                        "name": "小儿皮肤科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10812",
                        "parent_id": "108",
                        "index_id": "K0812",
                        "name": "小儿感染科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "10813",
                        "parent_id": "108",
                        "index_id": "K0813",
                        "name": "新生儿科",
                        "type": "1",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "109",
                "parent_id": "109",
                "index_id": "K09",
                "name": "康复理疗科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "109",
                        "parent_id": "109",
                        "index_id": "K09",
                        "name": "康复理疗科",
                        "type": "0",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "110",
                "parent_id": "110",
                "index_id": "K10",
                "name": "重症医学科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "110",
                        "parent_id": "110",
                        "index_id": "K10",
                        "name": "重症医学科",
                        "type": "0",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "111",
                "parent_id": "111",
                "index_id": "K11",
                "name": "中西医结合科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "111",
                        "parent_id": "111",
                        "index_id": "K11",
                        "name": "中西医结合科",
                        "type": "0",
                        "status": "0"
                    },
                    {
                        "id": "11101",
                        "parent_id": "111",
                        "index_id": "K1101",
                        "name": "中西医结合肿瘤内科",
                        "type": "1",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "112",
                "parent_id": "112",
                "index_id": "K12",
                "name": "中医科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "112",
                        "parent_id": "112",
                        "index_id": "K12",
                        "name": "中医科",
                        "type": "0",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "113",
                "parent_id": "113",
                "index_id": "K13",
                "name": "麻醉科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "113",
                        "parent_id": "113",
                        "index_id": "K13",
                        "name": "麻醉科",
                        "type": "0",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "114",
                "parent_id": "114",
                "index_id": "K14",
                "name": "传染科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "114",
                        "parent_id": "114",
                        "index_id": "K14",
                        "name": "传染科",
                        "type": "0",
                        "status": "0"
                    },
                    {
                        "id": "11401",
                        "parent_id": "114",
                        "index_id": "K1401",
                        "name": "肝病科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11402",
                        "parent_id": "114",
                        "index_id": "K1402",
                        "name": "结核科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11403",
                        "parent_id": "114",
                        "index_id": "K1403",
                        "name": "其他传染科",
                        "type": "1",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "115",
                "parent_id": "115",
                "index_id": "K15",
                "name": "五官科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "115",
                        "parent_id": "115",
                        "index_id": "K15",
                        "name": "五官科",
                        "type": "0",
                        "status": "0"
                    },
                    {
                        "id": "11501",
                        "parent_id": "115",
                        "index_id": "K1501",
                        "name": "眼科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11502",
                        "parent_id": "115",
                        "index_id": "K1502",
                        "name": "耳鼻咽喉头颈外科",
                        "type": "1",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "116",
                "parent_id": "116",
                "index_id": "K16",
                "name": "精神科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "116",
                        "parent_id": "116",
                        "index_id": "K16",
                        "name": "精神科",
                        "type": "0",
                        "status": "0"
                    },
                    {
                        "id": "11601",
                        "parent_id": "116",
                        "index_id": "K1601",
                        "name": "身心障碍",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11602",
                        "parent_id": "116",
                        "index_id": "K1602",
                        "name": "儿童老年",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11603",
                        "parent_id": "116",
                        "index_id": "K1603",
                        "name": "精神障碍",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11604",
                        "parent_id": "116",
                        "index_id": "K1604",
                        "name": "物质依赖",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11605",
                        "parent_id": "116",
                        "index_id": "K1605",
                        "name": "睡眠障碍科",
                        "type": "1",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "117",
                "parent_id": "117",
                "index_id": "K17",
                "name": "其他科室",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "117",
                        "parent_id": "117",
                        "index_id": "K17",
                        "name": "其他科室",
                        "type": "0",
                        "status": "0"
                    },
                    {
                        "id": "11701",
                        "parent_id": "117",
                        "index_id": "K1701",
                        "name": "全科医学",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11702",
                        "parent_id": "117",
                        "index_id": "K1702",
                        "name": "药剂科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11703",
                        "parent_id": "117",
                        "index_id": "K1703",
                        "name": "疼痛科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11704",
                        "parent_id": "117",
                        "index_id": "K1704",
                        "name": "体检中心",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11705",
                        "parent_id": "117",
                        "index_id": "K1705",
                        "name": "高压氧科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11706",
                        "parent_id": "117",
                        "index_id": "K1706",
                        "name": "职业病科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11707",
                        "parent_id": "117",
                        "index_id": "K1707",
                        "name": "影像科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11708",
                        "parent_id": "117",
                        "index_id": "K1708",
                        "name": "病理科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11709",
                        "parent_id": "117",
                        "index_id": "K1709",
                        "name": "介入科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11710",
                        "parent_id": "117",
                        "index_id": "K1710",
                        "name": "检验科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11711",
                        "parent_id": "117",
                        "index_id": "K1711",
                        "name": "营养科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11712",
                        "parent_id": "117",
                        "index_id": "K1712",
                        "name": "毒理科",
                        "type": "1",
                        "status": "0"
                    },
                    {
                        "id": "11713",
                        "parent_id": "117",
                        "index_id": "K1713",
                        "name": "胃食管反流病科",
                        "type": "1",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "118",
                "parent_id": "118",
                "index_id": "K18",
                "name": "急诊科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "118",
                        "parent_id": "118",
                        "index_id": "K18",
                        "name": "急诊科",
                        "type": "0",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "119",
                "parent_id": "118",
                "index_id": "K19",
                "name": "脑科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "119",
                        "parent_id": "118",
                        "index_id": "K19",
                        "name": "脑科",
                        "type": "0",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "120",
                "parent_id": "120",
                "index_id": "K20",
                "name": "手术室",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "120",
                        "parent_id": "120",
                        "index_id": "K20",
                        "name": "手术室",
                        "type": "0",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "121",
                "parent_id": "121",
                "index_id": "K21",
                "name": "护理科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "121",
                        "parent_id": "121",
                        "index_id": "K21",
                        "name": "护理科",
                        "type": "0",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "122",
                "parent_id": "122",
                "index_id": "K22",
                "name": "过敏科",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "122",
                        "parent_id": "122",
                        "index_id": "K22",
                        "name": "过敏科",
                        "type": "0",
                        "status": "0"
                    }
                ]
            },
            {
                "id": "123",
                "parent_id": "123",
                "index_id": "K23",
                "name": "住院部",
                "type": "0",
                "status": "0",
                "leaves": [
                    {
                        "id": "123",
                        "parent_id": "123",
                        "index_id": "K23",
                        "name": "住院部",
                        "type": "0",
                        "status": "0"
                    }
                ]
            }
        ],
        "total": 24
    }
}
```
> 失败 

```javascript
{
    code:10001,
    msg:"内部错误",
    data:null
}
```