# 合作方获取广告资源接口:获取要展示的广告资源

## 接口地址

[http://emkt.sfaessentials.com/v2/api/subject/lvb/detail](http://emkt.sfaessentials.com/v2/api/subject/lvb/detail)

## 接口描述

>合作方获取广告直通车相关广告资源
（包括数据流、banner、开机广告）

## 认证方式

>channelId:合作方的渠道id （由synapse平台生成）



## 请求参数(post,json字符串):

| 参数| 数据类型  | 是否必传 | 默认值 |  描述 | 
| ---- | -----| ----- | ----- | ----- | 
| bid | String|true | 无 |  请求的唯一id，32个字符的小写字符串|
| app| object|true | 无 | App对象，客户端APP的信息，必须真实来源于客户端|
|adspace_type|enum|true|无|广告位类型 枚举值类型 1 代表BANNER 2代表NATIVE信息流 3 代表OPENING闪屏开机广告|
|uid|String|true|无|当且仅当一个页面有多个广告请求时标识用户浏览某个页面的行为，避免用户在同一页面不同位置上较大概率地看到相同的广告。32个字符的小写字符串，由媒体	端生成。生成规则：综合设备号、所在页面、毫秒时间戳三种属性，MD5后取小写值|
|ip|String|true|无|客服端的ip|
|network_type|enum|true|无|网络类型 枚举值NET_UNKNOWN = 0; //未知 NET_WIFI = 1; //wifi NET_2G =2 ; //2G NET_3G =3 ; //3G NET_4G = 4; //4G|
|user_identity|object|true|无|当前访问用户相关属|
|user_agent|String|true|无|客户端的UserAgent|
|ext|String|false|无|扩展字段  以K-V对的形式给出 以分号分隔多个值|

## app 相关属性介绍
| 名称| 数据类型  | 是否必传 | 默认值 |  描述 | 
| ---- | -----| ----- | ----- | ----- | 
|app_name|String|true|无|c端的应用名称|
|package_name|String|true|无|应用的包名，应用的唯一标识|
|app_version|String|true|无|应用版本号|
##user_identity 相关属性介绍
| 名称| 数据类型  | 是否必传 | 默认值 |  描述 | 
| ---- | -----| ----- | ----- | ----- | 
|region_id|json|true|无|地区;用id,name 的形式以json格式请求（如：{"id":001,"name":"华北地区"}）|
|province_id|json|true|无|省 ;用id,name 的形式以json格式请求 如：{"id":1005,"name":"河北省"}|
|city_id|json|true|无|市;用id,name 的形式以json格式请求 如：{"id":01,"name":"北京市"}|
|hospital_id|json|true|无|医院，用id,name 的形式以json格式请求 如：{"id":01,"name":"协和医院"}|
|hospital_grade|json|true|无|医院级别，用id,name 的形式以json格式请求 如：{"id":101,"name":"一级甲等"}|
|department_id|json|true|无|医院科室，用id,name 的形式以json格式请求 如：{"id":321,"name":"外科"}|
|doctor_grade|json|true|无|医生级别，用id,name 的形式以json格式请求 如：{"id":321,"name":"主治医师"}|
|user_id|String|true|无|用户id|
|user_name|String|true|无|用户名称|
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
    "uid": "85e9167c065e4b14fab5711b6a1b0786", /*当且仅当一个页面有多个广告请求时 
                                                标识用户浏览某个页面的行为，避免用户在同一页面不同位置上较大概率地看到相同的广告。32个字符的小写字符串，由媒体	端生成。生成规则：综合设备号、所在页面、毫秒时间戳三种属性，MD5后取小写值*/
    "ip": "210.221.10.2",
    "network_type": 1,  /*网络类型*/
    "user_identity":{   
		  "region_id":"地区id加名称",  
		  "province_id":"省id加名称",
		  "city_id":"市id加名称",
		  "hospital_id":"医院id 加名称",
		  "hospital_grade":"医院等级id加名称",
		  "department_id":"科室id加名称",
		  "doctor_grade":"医生等级id加名称",
		  "user_id"："医生唯一标识",
                  "user_name":"医生名称"
		}
    "user_agent": "user_agent",
    "ext": "k1=v1;k2=v2"
}
```


## 响应参数（json）:

| 参数| 数据类型  | 是否必传|  描述 | 
| ---- | -----| ----- | ----- | 
| code| int|true |  响应码 10000 代表请求成功 10001代表请求失败|
|msg|String|true|响应消息|
|data|object|true|返回数据数据|

## data 返回数据说明
| 参数| 数据类型  | 是否必传|  描述 | 
| ---- | -----| ----- | ----- | 
|bid|Stirng|true|与BidRequest中的bid保持一致，32字节的字符串|
|ad|object|true|广告资源内容|
|creative|object|true|每个广告位的具体内容|
|adm_type|String|true|广告素材类型 "PIC" 代表图片|
|adm|object|true|广告素材对象|

## 响应数据示例(JSON):

> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        "bid": "7e6e7fe084d7d1af1c51eb2f315712a8",/*与BidRequest中的bid保持一致，32字节的字符串*/ 
        "ad":{
           "creative" : [{   /*每个广告位的创意 */
                          "adm_type":"PIC", /* 图片素材 （广告素材类型） 咨询 QA 点播 直播 等等  */  
                          "adm":{        /*广告素材对象* /
		                        "img":"http://synapse.com/a.jpg",
		                        "desc":"推广描述文字",
		                        "url":"http://landingpage.com" /* 打开地址或下载地址 （落地页地址，目前均会填充，须支持HTTP和HTTPS）*/
                                           }
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

