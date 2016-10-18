# 直播相关接口:直播内容接口

## 接口地址

[http://emkt.sfaessentials.com/aj/lvb/info](http://emkt.sfaessentials.com/aj/lvb/info)

## 接口描述

> 直播内容接口

## 认证方式

> 登录认证

## 请求参数(GET):

| 参数 | 类型| 是否必传 | 默认值 |  描述 | 
| ---- | ---- | ----- | ----- | ----- | 
| id | integer | true | 1 | 资讯id | 


## 响应数据(JSON):
> 成功

```javascript
{
    code: 10000,
    msg: "success",
    data: {
        id: "3",
        qcloud_channel_id: "16093425727655894615",
        video_name: "test_video",
        title: "测试",
        meeting_time: "2016-07-22 00:00:00",
        description: "这是一个测试直播",
        limit: "500",
        tags: "医疗",
        image: "www.baidu.com",
        author: "jealone",
        author_title: "医生",
        author_hospital: "协和医院",
        author_introduction: "医疗专家",
        author_image: "www.baidu.com",
        promotion_id: "734",
        status: "0",
        company_id: "23",
        create_user: {
            id: "279",
            nickname: "zeng test",
            useremail: "wzeng@ideabinder.com",
            phone: "15901235813",
            avatar: "",
            group_id: "0",
            company_id: "23",
            status: "1",
            ctime: "2016-07-04 15:37:55",
            utime: "2016-07-11 09:53:51",
            company_info: {
                id: "23",
                company_name: "西安杨森",
                create_user: "279",
                ctime: null,
                company_licence: "http://emkt.sfaessentials.com/images/upload/20160704/14676191149418.png",
                status: "1"
            },
            company_manager: 1,
            auth: null
        },
        insert_time: "2016-07-22 16:54:03",
        update_time: "2016-07-22 16:54:03",
        channel_info: [
            {
                channel_id: "16093425727655894615",
                channel_name: "测试",
                channel_describe: "这是一个测试直播",
                channel_status: "0",
                upstream_list: [
                    {
                        sourceName: "test_video",
                        sourceID: "3100_d701354d4fe911e6a2cba4dcbef5e35a",
                        sourceType: "1",
                        sourceAddress: "rtmp://3100.livepush.myqcloud.com/live/3100_d701354d4fe911e6a2cba4dcbef5e35a?bizid=3100"
                    }
                ],
                player_id: "1328",
                resolution: null,
                password: null,
                rtmp_downstream_address: "rtmp://3100.liveplay.myqcloud.com/live/3100_d701354d4fe911e6a2cba4dcbef5e35a",
                flv_downstream_address: "http://3100.liveplay.myqcloud.com/live/3100_d701354d4fe911e6a2cba4dcbef5e35a.flv"
            }
        ]
    }
}
```
> 失败 

```javascript
{
    error_code:10001,
    error:"操作失败",
    data:false
}
```