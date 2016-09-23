# 直播相关接口:H5落地页获取直播详情内容

## 接口地址

[http://emkt.sfaessentials.com/v2/api/subject/lvb/detail](http://emkt.sfaessentials.com/v2/api/subject/lvb/detail)

## 接口描述

> H5落地页获取直播详情内容

## 认证方式

> false



## 请求参数(GET):

| 参数 | 是否必传 | 默认值 |  描述 | 
| ---- | ----- | ----- | ----- | 
| lvb_id | true | 无 |  直播id|
| request_id| true | 无 | c端来源id|



## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        id: "8",
        qcloud_channel_id: "16093425727656115902",
        video_name: "创建直播hy1106",
        title: "创建直播hy1106",
        meeting_start_time: "2016-08-30 00:04:14",
        meeting_end_time: "2016-08-31 00:04:14",
        description: "",
        limit: "11",
        tags: "标签，标签，标签，标签",
        image: "http://emkt.sfaessentials.com/images/upload/20160729/14697219949344.png",
        author: "金晓峰，王小华",
        author_title: "讲者职称",
        author_hospital: "所属医院",
        author_introduction: "讲者介绍讲者介绍讲者介绍",
        author_image: "http://emkt.sfaessentials.com/images/upload/20160729/14697219967944.png",
        notice_phone: "13651341389",
        notice_email: "2645294577@qq.com",
        is_vod: "1",
        promotion_id: "830",
        status: "1",
        company_id: "23",
        create_user: "279",
        insert_time: "2016-07-29 00:06:40",
        update_time: "2016-07-29 17:55:48",
        begin_time: "2016-07-30 00:04:14",
        end_time: "2016-08-04 00:04:14",
        template_id: "18",
        threshold: "10",
        charge_id: "0",
        coverage: "0",
        relates: {
            product: [
                {
                    id: "148965",
                    cn_name: "产品测试",
                    en_name: "test",
                    general_name: "测试产品的保存"
                },
                {
                    id: "148963",
                    cn_name: "sdfsdf",
                    en_name: "",
                    general_name: "sdfsdf"
                }
            ],
            ta: [
                {
                    id: "63",
                    name: "达克宁TA",
                    description: "达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适达克宁适应症达克宁适"
                }
            ],
            keyword: [
                {
                    id: "345",
                    keyword: "达克宁信息点",
                    description: ""
                }
            ]
        },
        channel_info: [
            {
                channel_id: "16093425727656115902",
                channel_name: "创建直播hy1106",
                channel_describe: null,
                channel_status: "0",
                upstream_list: [
                    {
                        sourceName: "创建直播hy1106",
                        sourceID: "3100_44e80a1054dd11e6a2cba4dcbef5e35a",
                        sourceType: "1",
                        sourceAddress: "rtmp://3100.livepush.myqcloud.com/live/3100_44e80a1054dd11e6a2cba4dcbef5e35a?bizid=3100"
                    }
                ],
                player_id: "1328",
                resolution: null,
                password: null,
                rtmp_downstream_address: "rtmp://3100.liveplay.myqcloud.com/live/3100_44e80a1054dd11e6a2cba4dcbef5e35a",
                flv_downstream_address: "http://3100.liveplay.myqcloud.com/live/3100_44e80a1054dd11e6a2cba4dcbef5e35a.flv"
            }
        ]
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

