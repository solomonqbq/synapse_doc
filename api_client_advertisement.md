# 合作方获取广告资源接口:获取要展示的广告资源

![synapse移动APP广告对接流程](/uploads/2c818963aa50d2655b0a23d44528aa4a/synapse移动APP广告对接流程.jpg)

## 接口地址

[http://emkt.sfaessentials.com/v2/openapi/{companyId}/ads/fetch](#)

## 接口描述
>编码统一为UTF-8
>所有接口中涉及enum 类型，枚举具体值类型为 int
>合作方获取广告直通车相关广告资源
（包括数据流、banner、开机广告）
  其中companyId为变量，代表合作公司唯一标识 （由synapse平台提供）

## 接口说明
>编码统一为UTF-8
>所有接口中涉及enum 类型，枚举具体值类型为 int

## 认证方式

>companyId:合作方的公司id （由synapse平台生成）



## 请求参数(post,json字符串):

| 参数| 数据类型  | 是否必传 | 默认值 |  描述 | 
| ---- | -----| ----- | ----- | ----- | 
| bid | String|true | 无 |  请求的唯一id，32个字符的小写字符串|
| app| object|true | 无 | app对象，客户端APP的信息，必须真实来源于客户端,属性详细介绍参考下方[app属性介绍] (#app)</A>|
|adspace_type|enum|true|无|广告位类型 枚举值类型:  <br/> 1 :BANNER  <br/> 2:NATIVE信息流 <br/>  3 :OPENING闪屏开机广告|
|network_type|enum|true|无|网络类型 枚举值:  <br/> 0:NET_UNKNOWN未知   <br/> 1:NET_WIFI wifi   <br/>  2:NET_2G  2G  <br/> 3:NET_3G 3G  <br/>  4:NET_4G 4G|
|user_identity|object|true|无|当前访问用户相关属,属性详细介绍参考下方[user_identity属性介绍] (#user_identity)|
|device|object|true|无|访问设备对象信息,属性详细介绍参考下方[device属性介绍] (#device)|
|ext|String|false|无|扩展字段  以K-V对的形式给出 以分号分隔多个值|
## app 相关属性介绍    <a name="app" />
| 名称| 数据类型  | 是否必传 | 默认值 |  描述 | 
| ---- | -----| ----- | ----- | ----- | 
|app_name|String|true|无|c端的应用名称 如 app_name:"医疗"|
|package_name|String|true|无|应用的包名，应用的唯一标识 如 package_name:"com.yilian.com"| 
|app_version|String|true|无|应用版本号   如 app_version:"1.1"|

## user_identity 相关属性介绍（所有id均为合作方与synapse同步后，合作方自己的id） <a name="user_identity" />
| 名称| 数据类型  | 是否必传 | 默认值 |  描述 | 
| ---- | -----| ----- | ----- | ----- | 
|province_id|String|true|无|省 id|
|city_id|String|true|无|市id|
|hospital_id|String|true|无|医院id|
|hospital_grade|String|false|无|医院级别id|
|department_id|String|true|无|医院科室id|
|doctor_grade|String|true|无|医生级别id|
|user_id|String|true|无|医生id|
|user_name|String|true|无|医生名称|

## device 相关属性介绍  <a name="device" />
| 名称| 数据类型  | 是否必传 | 默认值 |  描述 | 
| ---- | -----| ----- | ----- | ----- | 
|device_id|String|true|无|设备id值，小写的原始值或小写的MD5值，MD5前请先转成小写字符串|
|hash_type|enum|true|无|设备id值哈希类型  <br/> 0 ：原始值  <br/>  1 ：MD5值|
|os_type|enum|true|无|系统类型  <br/> 1 : OS_IOS  <br/>  2 :OS_ANDOROID|
|device_id_type|enum|true|无|设备id类型 枚举值:  <br/> 0:UNKNOWN 未知  <br/> 1:IMEI imei <br/>  2:IDFA idfa <br/>  3:AAID android id  <br/>  4:MAC mac    <br/> 5:IDFV idfv  <br/> 6:M2ID  <br/>   7:SERIALID   <br/>  8:IMSI imsi   <br/>目前Android支持类型1,3,4,7,8     <br/>          如果不能保证客户端能取到，请传IMEI 目前iOS支持类型2,5 <br/> 推荐传IFDA,IDFV |

## 请求数据(JSON):

> 示例

```javascript
{
    "bid": "7e6e7fe084d7d1af1c51eb2f315712a8",
    "app": {/*客户端信息*/
        "app_name": "测试DEMO",
        "package_name": "com.mediav.ads",
        "app_version": "1.0"
    },
    "adspace_type": 4,//广告位类型 1 代表BANNER横幅;  2 代表NATIVE信息流 ;3 代表OPENING开屏 
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
		},
     "device":[{
              "device_id":"md5值或原始值",
              "device_id_type":0,
              "hash_type":0,
              "os_type" :1
     }],
     "ext": "k1=v1;k2=v2"
}
```


## 响应参数（json）:

| 参数| 数据类型  | 是否必传|  描述 | 
| ---- | -----| ----- | ----- | 
| code| int|true |  响应码  <br/> 10000 :请求成功  <br/> 10001:请求失败|
|msg|String|true|响应消息|
|data|object|true|返回数据对象,具体介绍请参考下方 [data 属性介绍](#data)|

## data 返回数据说明 <a name="data" />
| 参数| 数据类型  | 是否必传|  描述 | 
| ---- | -----| ----- | ----- | 
|bid|Stirng|true|与Request请求中的bid保持一致，32字节的字符串|
|ad|object|true|广告资源内容,对象具体属性请查看下方[ ad属性介绍](#ad)|


## ad 对象属性说明 <a name="ad" />
| 参数| 数据类型  | 是否必传|  描述 | 
| ---- | -----| ----- | ----- | 
|creative|object|true|每个广告位的具体内容,对象具体属性请查看下方[ creative属性介绍](#creative)|
|event_track|list of object|true|检测对象 ,对象具体属性请查看下方[ event_track属性介绍](#event_track)|

## creative 对象属性说明  <a name="creative" />
| 名称| 数据类型  | 是否必传|  描述 | 
| ---- | -----| ----- | ----- | 
|adm_type|String|true|广告素材类型  <br/> "PIC"指图片  <br/> "IMG_TEXT" 指图文混编|
|adm|object|true|广告素材内容具体对象|
|img|String|true|图片素材路径|
|desc|String|true|推广描述文字|
|url|String|true|推广访问链接|

## event_track对象属性说明  <a name="event_track" />
| 名称| 数据类型  | 是否必传|  描述 | 
| ---- | -----| ----- | ----- | 
|event_type|String|true|检测类型  <br/>  “SHOW”代表报告检测   <br/>“CLICK”代表点击检测|
|notify_url|String|srue|检测回调链接|

## 响应数据示例(JSON):

> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        "bid": "7e6e7fe084d7d1af1c51eb2f315712a8",//与BidRequest中的bid保持一致，32字节的字符串
        "ad":{
           "creative" : [{   //广告内容集合 
                          "adm_type":"PIC", //图片素材 （广告素材类型）
                          "adm":{        //广告素材对象
		                        "img":"http://synapse.com/a.jpg",
		                        "desc":"推广描述文字",
		                        "url":"http://landingpage.com" // 打开地址或下载地址 （落地页地址，须支持HTTP和HTTPS）
                                          },
                         "event_track":[{ //广告监测对象
                                          "event_type": "SHOW",  // 展示监测 
                                          "notify_url":"http://show_notify_url_1"//检测回调地址
                                         },
                                         {
                                           "event_type": "CLICK",  //点击监测
                                           "notify_url":"http://click_notify_url_1"
                                      }]
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

