# 合作方获取广告资源接口:获取要展示的广告资源

## 接口地址

[http://emkt.sfaessentials.com/v2/openapi/{companyId}/ads/fetch](http://emkt.sfaessentials.com/v2/openapi/{companyId}/ads/fetch)

## 接口描述

>合作方获取广告直通车相关广告资源
（包括数据流、banner、开机广告）
  其中companyId为变量，代表合作公司唯一标识 （由synapse平台提供）

## 认证方式

>companyId:合作方的公司id （由synapse平台生成）



## 请求参数(post,json字符串):

| 参数| 数据类型  | 是否必传 | 默认值 |  描述 | 
| ---- | -----| ----- | ----- | ----- | 
| bid | String|true | 无 |  请求的唯一id，32个字符的小写字符串|
| app| object|true | 无 | App对象，客户端APP的信息，必须真实来源于客户端|
|adspace_type|enum|true|无|广告位类型 枚举值类型 1 代表BANNER 2代表NATIVE信息流 3 代表OPENING闪屏开机广告|
|network_type|enum|true|无|网络类型 枚举值NET_UNKNOWN = 0; //未知 NET_WIFI = 1; //wifi NET_2G =2 ; //2G NET_3G =3 ; //3G NET_4G = 4; //4G|
|user_identity|object|true|无|当前访问用户相关属|
|ext|String|false|无|扩展字段  以K-V对的形式给出 以分号分隔多个值|
|device|object|true|无|访问设备对象信息|

## app 相关属性介绍
| 名称| 数据类型  | 是否必传 | 默认值 |  描述 | 
| ---- | -----| ----- | ----- | ----- | 
|app_name|String|true|无|c端的应用名称|
|package_name|String|true|无|应用的包名，应用的唯一标识|
|app_version|String|true|无|应用版本号|

## user_identity 相关属性介绍
| 名称| 数据类型  | 是否必传 | 默认值 |  描述 | 
| ---- | -----| ----- | ----- | ----- | 
|province_id|String|true|无|省 id|
|city_id|String|true|无|市id|
|hospital_id|String|true|无|医院id|
|hospital_grade|String|false|无|医院级别id|
|department_id|String|true|无|医院科室id|
|doctor_grade|String|true|无|医生级别id|
|user_id|String|true|无|用户id|
|user_name|String|true|无|用户名称|

## device 相关属性介绍
| 名称| 数据类型  | 是否必传 | 默认值 |  描述 | 
| ---- | -----| ----- | ----- | ----- | 
|device_id|String|true|无|设备id值，小写的原始值或小写的MD5值，MD5前请先转成小写字符串|
|hash_type|enum|true|无|设备id值哈希类型 0 代表原始值 1 代表MD5值|
|os_type|enum|true|无|系统类型 1 代表 OS_IOS 2 代表OS_ANDOROID|
|device_id_type|enum|true|无|设备id类型 枚举值 UNKNOWN = 0; //未知 IMEI = 1; //imei IDFA = 2; //idfa AAID = 3;//android id MAC = 4; //mac IDFV = 5; //idfv M2ID = 6; // SERIALID = 7; // IMSI = 8; //imsi  目前Android支持类型1,3,4,7,8              如果不能保证客户端能取到，请传IMEI 目前iOS支持类型2,5 推荐传IFDA,IDFV |

## 请求数据(JSON):

> 示例

```javascript
{
    "bid": "7e6e7fe084d7d1af1c51eb2f315712a8",
    "companyId": "7e6e7fe084d7d1af325f5df6e9",
    "app": {/*客户端信息*/
        "app_name": "测试DEMO",
        "package_name": "com.mediav.ads",
        "app_version": "1.0"
    },
    "adspace_type": 4,//广告位类型 1 代表BANNER横幅;  2 代表NATIVE信息流 ;3 代表OPENING开屏 
    "uid": "85e9167c065e4b14fab5711b6a1b0786", /*当且仅当一个页面有多个广告请求时 
                                                标识用户浏览某个页面的行为，避免用户在同一页面不同位置上较大概率地看到相同的广告。32个字符的小写字符串，由媒体	端生成。生成规则：综合设备号、所在页面、毫秒时间戳三种属性，MD5后取小写值*/
    "ip": "210.221.10.2",
    "network_type": 1,  /*网络类型*/
    "user_identity":{   
		  "region_id":"地区id",  
		  "province_id":"省id",
		  "city_id":"市id",
		  "hospital_id":"医院id ",
		  "hospital_grade":"医院等级id",
		  "department_id":"科室id",
		  "doctor_grade":"医生等级id",
		  "user_id"："医生唯一标识",
                  "user_name":"医生名称"
		}
     "user_agent": "user_agent",
     "device":[{
             "device_id":[{
                       "device_id":"md5值或原始值",
                       "device_id_type":0,
                       "hash_type":0
              }],
             "os_type" :1
     }],
     "ext": "k1=v1;k2=v2"
}
```


## 响应参数（json）:

| 参数| 数据类型  | 是否必传|  描述 | 
| ---- | -----| ----- | ----- | 
| code| int|true |  响应码 10000 代表请求成功 10001代表请求失败|
|msg|String|true|响应消息|
|data|object|true|返回数据对象|

## data 返回数据说明
| 参数| 数据类型  | 是否必传|  描述 | 
| ---- | -----| ----- | ----- | 
|bid|Stirng|true|与BidRequest中的bid保持一致，32字节的字符串|
|ad|object|true|广告资源内容|
|creative|object|true|每个广告位的具体内容|
|event_track|list of object|true|检测对象|

## creative 对象属性说明
| 名称| 数据类型  | 是否必传|  描述 | 
| ---- | -----| ----- | ----- | 
|adm_type|String|true|广告素材类型"PIC"指图片|
|adm|object|true|广告素材内容具体对象|
|img|String|true|图片素材路径|
|desc|String|true|推广描述文字|
|url|String|true|推广访问链接|

## event_track对象属性说明
| 名称| 数据类型  | 是否必传|  描述 | 
| ---- | -----| ----- | ----- | 
|event_type|String|true|检测类型 “SHOW”代表报告检测 “CLICK”代表点击检测|
|notify_url|array|srue|检测回调链接|

## 响应数据示例(JSON):

> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        "bid": "7e6e7fe084d7d1af1c51eb2f315712a8",/*与BidRequest中的bid保持一致，32字节的字符串*/ 
        "ad":{
           "creative" : [{   //广告内容集合 
                          "adm_type":"PIC", //图片素材 （广告素材类型）
                          "adm":{        //广告素材对象
		                        "img":"http://synapse.com/a.jpg",
		                        "desc":"推广描述文字",
		                        "url":"http://landingpage.com" // 打开地址或下载地址 （落地页地址，须支持HTTP和HTTPS）
                                          }
                                 }],
              "event_track":[{
                              "event_type": "SHOW",  // 展示监测 
                               "notify_url": [//检测回调地址
                                          "http://show_notify_url_1",
                                          "http://show_notify_url_2"
                                ]
                           },
                           {
                                "event_type": "CLICK",  //点击监测
                                "notify_url": [
                                            "http://click_notify_url_1",
                                            "http://click_notify_url_2"
                                 ]
                       }]
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

