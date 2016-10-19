# 合作方获取广告资源接口:获取要展示的广告资源

## 接口地址

[http://emkt.sfaessentials.com/v2/api/subject/lvb/detail](http://emkt.sfaessentials.com/v2/api/subject/lvb/detail)

## 接口描述

>合作方获取广告直通车相关广告资源
（包括数据流、banner、开机广告）

## 认证方式

>channelId:合作方的渠道id （由synapse平台生成）



## 请求参数(post,json字符串):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| bid | true | 无 |  请求的唯一id，32个字符的小写字符串|
| app| true | 无 | App对象，客户端APP的信息，必须真实来源于客户端|
|adspace_type|true|无|广告位类型|
|uid|true|无|当且仅当一个页面有多个广告请求时标识用户浏览某个页面的行为，避免用户在同一页面不同位置上较大概率地看到相同的广告。32个字符的小写字符串，由媒体	端生成。生成规则：综合设备号、所在页面、毫秒时间戳三种属性，MD5后取小写值|
|ip|true|无|客服端的ip|
|network_type|true|无|网络类型|
|user_identity|true|无|当前访问用户相关属|
|user_agent|true|无|客户端的UserAgent|
|ext|false|无|扩展字段  以K-V对的形式给出 以分号分隔多个值|

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

## 响应数据(JSON):

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

