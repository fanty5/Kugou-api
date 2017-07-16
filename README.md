## 酷狗音乐API接口整理

>基于酷狗音乐整理的音乐API接口数据

### 音乐新歌榜

__说明:__ 获取新歌曲榜单

__必选参数:__
`page`: json

__接口地址:__ `http://m.kugou.com/?json=true`



###  音乐排行榜

__说明:__ 获取音乐排行榜

__必选参数:__

__接口地址:__ `http://m.kugou.com/rank/list&json=true`

__返回数据__


###  排行版分类歌曲列表

__说明:__ 获取音乐排行榜

__必选参数:__
`rankid` 排行榜分类下id
`json` 返回类型


__接口地址:__ `http://m.kugou.com/rank/info/?rankid=8888&page=1&json=true`

__返回数据__


###  音乐歌单

__说明:__ 获取音乐排行榜

__必选参数:__


__接口地址:__ `http://m.kugou.com/plist/index&json=true`

__返回数据__

###  歌单下的音乐列表

__说明:__ 获取 歌单下的音乐列表，需要添加  `specialid`


__必选参数:__
`specialid` 125032

__接口地址:__ `http://m.kugou.com/plist/list/125032?json=true`

__返回数据__


### 歌手分类

__说明:__ 获取 歌手分类


__必选参数:__

`无`
__接口地址:__ `http://m.kugou.com/singer/class&json=true`


### 歌手分类下面的歌手列表

__说明:__ 获取 歌手分类

__必选参数:__

`classid` 

__接口地址:__ `http://m.kugou.com/singer/list/88?json=true`


### 歌手信息

__说明:__ 获取 歌手分类

__必选参数:__

`singerid` : 歌手id  3060 

__接口地址:__ `http://m.kugou.com/singer/info/3060&json=true`

### 歌曲音乐详情

__说明:__ 获取 歌曲音乐详情信息

__必选参数:__

`hash` : 音乐列表下的 音乐id 

__接口地址:__ `http://m.kugou.com/app/i/getSongInfo.php?cmd=playInfo&hash=CB7EE97F4CC11C4EA7A1FA4B516A5D97`
__返回数据__
```
{
    "fileHead": 100,
    "q": 0,
    "extra": {
        "320filesize": 7998693,
        "sqfilesize": 23222557,
        "sqhash": "CAC59E48D58853BF40BB6158F2F5B0C5",
        "128hash": "CB7EE97F4CC11C4EA7A1FA4B516A5D97",
        "320hash": "47F63F15A7C048829FA796BC7F74E62B",
        "128filesize": 3198974
    },
    "fileSize": 3198974,
    "hash": "CB7EE97F4CC11C4EA7A1FA4B516A5D97",
    "choricSinger": "李玉刚",
    "error": "",
    "topic_remark": "",
    "url": "http://fs.open.kugou.com/9a44695c75d81312dbdf8ed950039390/596b5b03/G078/M08/18/17/jg0DAFgi6G-AKqsqADDP_nSW5F4051.mp3",
    "time": 1500209038,
    "bitRate": 128,
    "imgUrl": "http://singerimg.kugou.com/uploadpic/softhead/{size}/20140304/20140304154338526832.jpg",
    "songName": "刚好遇见你",
    "errcode": 0,
    "singerHead": "",
    "privilege": 0,
    "status": 1,
    "stype": 11323,
    "ctype": 1009,
    "singerName": "李玉刚",
    "fileName": "李玉刚 - 刚好遇见你",
    "singerId": 2018,
    "topic_url": "",
    "intro": "",
    "mvhash": "C4AFAEFC84A7D1B6B413288377203B38",
    "extName": "mp3",
    "req_hash": "CB7EE97F4CC11C4EA7A1FA4B516A5D97",
    "timeLength": 200
}
```

### 音乐详情-带歌词版本

__说明:__ 获取 音乐详情-带歌词版本

__必选参数:__

`hash` : 音乐列表下的 音乐id 

__接口地址:__ `http://www.kugou.com/yy/index.php?r=play/getdata&hash=CB7EE97F4CC11C4EA7A1FA4B516A5D97`
__返回数据__
```
{
    "status": 1,
    "err_code": 0,
    "data": {
        "hash": "CB7EE97F4CC11C4EA7A1FA4B516A5D97",
        "timelength": 199000,
        "filesize": 3198974,
        "audio_name": "李玉刚 - 刚好遇见你",
        "have_album": 0,
        "album_name": "未知专辑",
        "album_id": 0,
        "img": "http://singerimg.kugou.com/uploadpic/softhead/400/20140304/20140304154338526832.jpg",
        "have_mv": 1,
        "video_id": "596892",
        "author_name": "李玉刚",
        "song_name": "刚好遇见你",
        "lyrics": "[00:00.02]李玉刚 - 刚好遇见你\r\n[00:00.75]词：高进\r\n[00:00.85]曲：高进\r\n[00:00.94]编曲：关天天\r\n[00:13.13]我们哭了\r\n[00:15.79]我们笑着\r\n[00:18.83]我们抬头望天空\r\n[00:21.86]星星还亮着几颗\r\n[00:24.98]我们唱着\r\n[00:27.96]时间的歌\r\n[00:31.09]才懂得相互拥抱\r\n[00:33.98]到底是为了什么\r\n[00:37.30]因为我刚好遇见你\r\n[00:40.77]留下足迹才美丽\r\n[00:43.79]风吹花落泪如雨\r\n[00:46.80]因为不想分离\r\n[00:49.95]因为刚好遇见你\r\n[00:53.10]留下十年的期许\r\n[00:55.99]如果再相遇\r\n[00:59.21]我想我会记得你\r\n[01:14.32]我们哭了\r\n[01:17.23]我们笑着\r\n[01:20.34]我们抬头望天空\r\n[01:23.33]星星还亮着几颗\r\n[01:26.51]我们唱着\r\n[01:29.53]时间的歌\r\n[01:32.59]才懂得相互拥抱\r\n[01:35.59]到底是为了什么\r\n[01:38.73]因为我刚好遇见你\r\n[01:42.23]留下足迹才美丽\r\n[01:45.30]风吹花落泪如雨\r\n[01:48.39]因为不想分离\r\n[01:51.55]因为刚好遇见你\r\n[01:54.54]留下十年的期许\r\n[01:57.61]如果再相遇\r\n[02:00.81]我想我会记得你\r\n[02:03.99]因为刚好遇见你\r\n[02:06.86]留下足迹才美丽\r\n[02:09.94]风吹花落泪如雨\r\n[02:13.03]因为不想分离\r\n[02:16.06]因为刚好遇见你\r\n[02:19.16]留下十年的期许\r\n[02:22.21]如果再相遇\r\n[02:25.34]我想我会记得你\r\n[02:31.40]因为我刚好遇见你\r\n[02:34.51]留下足迹才美丽\r\n[02:37.59]风吹花落泪如雨\r\n[02:40.67]因为不想分离\r\n[02:43.77]因为刚好遇见你\r\n[02:46.84]留下十年的期许\r\n[02:49.94]如果再相遇\r\n[02:53.11]我想我会记得你\r\n",
        "author_id": "2018",
        "privilege": 0,
        "privilege2": "0",
        "play_url": "http://fs.web.kugou.com/1edd2b78f37fccb8642daf1b42a4dfb3/596b5886/G078/M08/18/17/jg0DAFgi6G-AKqsqADDP_nSW5F4051.mp3",
        "authors": [
            {
                "is_publish": "1",
                "author_id": "2018",
                "avatar": "20140304154338526832.jpg",
                "author_name": "李玉刚"
            }
        ],
        "bitrate": 128
    }
}
```

### 热门搜索列表

__说明:__ 获取 热门搜索列表

__必选参数:__
`plat` :开始数
`count` : 热门搜索关键字返回

__接口地址:__ `http://mobilecdn.kugou.com/api/v3/search/hot?format=json&plat=0&count=30`
__返回数据__

```
{
    "status": 1,
    "error": "",
    "data": {
        "timestamp": 1500209333,
        "info": [
            {
                "sort": 1,
                "keyword": "中国新歌声第二季",
                "jumpurl": ""
            },
            {
                "sort": 2,
                "keyword": "音乐故事",
                "jumpurl": "http://huodong.kugou.com/a2015/html/musicStory/index_87702.html"
            },
            {
                "sort": 3,
                "keyword": "从前慢",
                "jumpurl": ""
            },
            {
                "sort": 4,
                "keyword": "菊花台",
                "jumpurl": ""
            },
            {
                "sort": 5,
                "keyword": "李白",
                "jumpurl": ""
            },
            {
                "sort": 6,
                "keyword": "追光者",
                "jumpurl": ""
            },
            {
                "sort": 7,
                "keyword": "薛之谦",
                "jumpurl": ""
            },
            {
                "sort": 8,
                "keyword": "淘汰",
                "jumpurl": ""
            },
            {
                "sort": 9,
                "keyword": "鹿晗",
                "jumpurl": ""
            },
            {
                "sort": 10,
                "keyword": "金志文",
                "jumpurl": ""
            },
            {
                "sort": 11,
                "keyword": "TFBOYS",
                "jumpurl": ""
            },
            {
                "sort": 12,
                "keyword": "成都",
                "jumpurl": ""
            },
            {
                "sort": 13,
                "keyword": "无条件",
                "jumpurl": ""
            },
            {
                "sort": 14,
                "keyword": "楚乔传",
                "jumpurl": ""
            },
            {
                "sort": 15,
                "keyword": "双世宠妃",
                "jumpurl": ""
            },
            {
                "sort": 16,
                "keyword": "爱河",
                "jumpurl": ""
            }
        ]
    },
    "errcode": 0
}
```

### 音乐搜索

__说明:__ 获取 音乐搜索结果

__必选参数:__

`keyword` : 关键字

__接口地址:__ `http://mobilecdn.kugou.com/api/v3/search/song?format=json&keyword=%E7%8E%8B%E5%8A%9B%E5%AE%8F&page=1&pagesize=20&showtype=1`
__返回数据__
```
{
    "status": 1,
    "error": "",
    "data": {
        "aggregation": [
            {
                "key": "DJ",
                "count": 0
            },
            {
                "key": "现场",
                "count": 0
            },
            {
                "key": "广场舞",
                "count": 0
            },
            {
                "key": "伴奏",
                "count": 0
            },
            {
                "key": "铃声",
                "count": 0
            }
        ],
        "tab": "全部",
        "info": [
            {
                "pay_type_320": 0,
                "m4afilesize": 1258783,
                "price_sq": 0,
                "filesize": 4910601,
                "source": "",
                "bitrate": 128,
                "topic": "《非常幸运》电影主题曲",
                "price": 0,
                "Accompany": 1,
                "old_cpy": 1,
                "fail_process_sq": 0,
                "singername": "王力宏、章子怡",
                "pay_type": 0,
                "sourceid": 0,
                "topic_url": "",
                "fail_process_320": 0,
                "pkg_price": 0,
                "feetype": 0,
                "filename": "王力宏、章子怡 - 爱一点【《非常幸运》电影主题曲】",
                "price_320": 0,
                "extname": "mp3",
                "320hash": "4dc9da16dff397ed2695e164b612cab1",
                "mvhash": "2ebddad8d64878f893dd68ea7d92d095",
                "privilege": 0,
                "group": [
                    {
                        "pay_type_320": 0,
                        "m4afilesize": 1258783,
                        "price_sq": 0,
                        "filesize": 4910601,
                        "source": "",
                        "bitrate": 128,
                        "topic": "",
                        "price": 0,
                        "Accompany": 1,
                        "old_cpy": 1,
                        "fail_process_sq": 0,
                        "singername": "王力宏、章子怡",
                        "pay_type": 0,
                        "sourceid": 0,
                        "topic_url": "",
                        "fail_process_320": 0,
                        "pkg_price": 0,
                        "feetype": 0,
                        "filename": "王力宏、章子怡 - 爱一点",
                        "price_320": 0,
                        "extname": "mp3",
                        "320hash": "4dc9da16dff397ed2695e164b612cab1",
                        "mvhash": "2ebddad8d64878f893dd68ea7d92d095",
                        "privilege": 0,
                        "album_audio_id": 32243892,
                        "album_id": "982717",
                        "ownercount": 142934,
                        "rp_publish": 1,
                        "rp_type": "audio",
                        "audio_id": 8692118,
                        "320filesize": 12274416,
                        "isnew": 0,
                        "duration": 306,
                        "pkg_price_sq": 0,
                        "pkg_price_320": 0,
                        "srctype": 1,
                        "songname": "爱一点",
                        "fail_process": 0,
                        "sqhash": "dddf0263dc58a5f301093db3682532fc",
                        "album_name": "你的爱。",
                        "hash": "32dec5bb5e07be73689860aecf75ceb1",
                        "pay_type_sq": 0,
                        "320privilege": 0,
                        "sqprivilege": 0,
                        "sqfilesize": 36150153,
                        "othername": ""
                    },
                    {
                        "pay_type_320": 0,
                        "m4afilesize": 1258783,
                        "price_sq": 0,
                        "filesize": 4910601,
                        "source": "",
                        "bitrate": 128,
                        "topic": "",
                        "price": 0,
                        "Accompany": 1,
                        "old_cpy": 1,
                        "fail_process_sq": 0,
                        "singername": "王力宏、章子怡",
                        "pay_type": 0,
                        "sourceid": 0,
                        "topic_url": "",
                        "fail_process_320": 0,
                        "pkg_price": 0,
                        "feetype": 0,
                        "filename": "王力宏、章子怡 - 爱一点",
                        "price_320": 0,
                        "extname": "mp3",
                        "320hash": "4dc9da16dff397ed2695e164b612cab1",
                        "mvhash": "2ebddad8d64878f893dd68ea7d92d095",
                        "privilege": 0,
                        "album_audio_id": 32586923,
                        "album_id": "939374",
                        "ownercount": 142934,
                        "rp_publish": 1,
                        "rp_type": "audio",
                        "audio_id": 8692118,
                        "320filesize": 12274416,
                        "isnew": 0,
                        "duration": 306,
                        "pkg_price_sq": 0,
                        "pkg_price_320": 0,
                        "srctype": 1,
                        "songname": "爱一点",
                        "fail_process": 0,
                        "sqhash": "dddf0263dc58a5f301093db3682532fc",
                        "album_name": "CCTV音乐频道中国音乐电视合辑",
                        "hash": "32dec5bb5e07be73689860aecf75ceb1",
                        "pay_type_sq": 0,
                        "320privilege": 0,
                        "sqprivilege": 0,
                        "sqfilesize": 36150153,
                        "othername": ""
                    },
                    
             
            {
                "pay_type_320": 0,
                "m4afilesize": 873506,
                "price_sq": 0,
                "filesize": 3321482,
                "source": "",
                "bitrate": 128,
                "topic": "",
                "price": 0,
                "Accompany": 1,
                "old_cpy": 1,
                "fail_process_sq": 0,
                "singername": "王力宏",
                "pay_type": 0,
                "sourceid": 0,
                "topic_url": "",
                "fail_process_320": 0,
                "pkg_price": 0,
                "feetype": 0,
                "filename": "王力宏 - 十二生肖",
                "price_320": 0,
                "extname": "mp3",
                "320hash": "8735bf5b9ab8886d0cada629199f3140",
                "mvhash": "97a3b1be73fac647d8daf0a264bb09e9",
                "privilege": 0,
                "group": [],
                "album_audio_id": 0,
                "album_id": "",
                "ownercount": 67443,
                "rp_publish": 1,
                "rp_type": "audio",
                "audio_id": 906549,
                "320filesize": 8301908,
                "isnew": 0,
                "duration": 207,
                "pkg_price_sq": 0,
                "pkg_price_320": 0,
                "srctype": 1,
                "songname": "十二生肖",
                "fail_process": 0,
                "sqhash": "",
                "album_name": "",
                "hash": "07f85687459ba0741ada28063f429c6c",
                "pay_type_sq": 0,
                "320privilege": 0,
                "sqprivilege": 0,
                "sqfilesize": 0,
                "othername": ""
            },
            {
                "pay_type_320": 0,
                "m4afilesize": 1168947,
                "price_sq": 0,
                "filesize": 4560312,
                "source": "",
                "bitrate": 128,
                "topic": "",
                "price": 0,
                "Accompany": 1,
                "old_cpy": 1,
                "fail_process_sq": 0,
                "singername": "王力宏",
                "pay_type": 0,
                "sourceid": 0,
                "topic_url": "",
                "fail_process_320": 0,
                "pkg_price": 0,
                "feetype": 0,
                "filename": "王力宏 - 龙的传人 - 现场版2",
                "price_320": 0,
                "extname": "mp3",
                "320hash": "",
                "mvhash": "",
                "privilege": 0,
                "group": [],
                "album_audio_id": 0,
                "album_id": "",
                "ownercount": 41101,
                "rp_publish": 1,
                "rp_type": "audio",
                "audio_id": 24673134,
                "320filesize": 0,
                "isnew": 0,
                "duration": 285,
                "pkg_price_sq": 0,
                "pkg_price_320": 0,
                "srctype": 1,
                "songname": "龙的传人",
                "fail_process": 0,
                "sqhash": "",
                "album_name": "",
                "hash": "0b349cac7abae38480a20337eb9d5b6a",
                "pay_type_sq": 0,
                "320privilege": 0,
                "sqprivilege": 0,
                "sqfilesize": 0,
                "othername": "现场版2"
            },
            {
                "pay_type_320": 0,
                "m4afilesize": 343932,
                "price_sq": 0,
                "filesize": 1330250,
                "source": "",
                "bitrate": 128,
                "topic": "",
                "price": 0,
                "Accompany": 0,
                "old_cpy": 1,
                "fail_process_sq": 0,
                "singername": "王力宏、鹿晗",
                "pay_type": 0,
                "sourceid": 0,
                "topic_url": "",
                "fail_process_320": 0,
                "pkg_price": 0,
                "feetype": 0,
                "filename": "王力宏、鹿晗 - 大城小爱",
                "price_320": 0,
                "extname": "mp3",
                "320hash": "",
                "mvhash": "",
                "privilege": 0,
                "group": [],
                "album_audio_id": 66382768,
                "album_id": "1965578",
                "ownercount": 33397,
                "rp_publish": 1,
                "rp_type": "audio",
                "audio_id": 26979930,
                "320filesize": 0,
                "isnew": 0,
                "duration": 83,
                "pkg_price_sq": 0,
                "pkg_price_320": 0,
                "srctype": 1,
                "songname": "大城小爱",
                "fail_process": 0,
                "sqhash": "",
                "album_name": "在线热搜(华语)系列Ⅳ",
                "hash": "3f3ccb11cef7bebbcc01251f5276bf59",
                "pay_type_sq": 0,
                "320privilege": 0,
                "sqprivilege": 0,
                "sqfilesize": 0,
                "othername": ""
            },
            {
                "pay_type_320": 0,
                "m4afilesize": 1112368,
                "price_sq": 0,
                "filesize": 4331728,
                "source": "",
                "bitrate": 128,
                "topic": "",
                "price": 0,
                "Accompany": 1,
                "old_cpy": 1,
                "fail_process_sq": 0,
                "singername": "王力宏",
                "pay_type": 0,
                "sourceid": 0,
                "topic_url": "",
                "fail_process_320": 0,
                "pkg_price": 0,
                "feetype": 0,
                "filename": "王力宏 - 就是现在",
                "price_320": 0,
                "extname": "mp3",
                "320hash": "e0ff60d5a0d4de63128e2b1e5494dcfd",
                "mvhash": "b4d46c0e1f4614cfb87d48680b0f9a3e",
                "privilege": 0,
                "group": [],
                "album_audio_id": 32243886,
                "album_id": "982717",
                "ownercount": 31406,
                "rp_publish": 1,
                "rp_type": "audio",
                "audio_id": 7713683,
                "320filesize": 10826385,
                "isnew": 0,
                "duration": 270,
                "pkg_price_sq": 0,
                "pkg_price_320": 0,
                "srctype": 1,
                "songname": "就是现在",
                "fail_process": 0,
                "sqhash": "f2af18c892359e4d914fe780d787d658",
                "album_name": "你的爱。",
                "hash": "8bac223717951f0c2184f4aa03abf682",
                "pay_type_sq": 0,
                "320privilege": 0,
                "sqprivilege": 0,
                "sqfilesize": 32733224,
                "othername": ""
            },
            {
                "pay_type_320": 0,
                "m4afilesize": 1017892,
                "price_sq": 0,
                "filesize": 3963133,
                "source": "",
                "bitrate": 128,
                "topic": "",
                "price": 0,
                "Accompany": 0,
                "old_cpy": 1,
                "fail_process_sq": 0,
                "singername": "孙楠、容祖儿、王力宏、余翠芝",
                "pay_type": 0,
                "sourceid": 0,
                "topic_url": "",
                "fail_process_320": 0,
                "pkg_price": 0,
                "feetype": 0,
                "filename": "孙楠、容祖儿、王力宏、余翠芝 - 相亲相爱",
                "price_320": 0,
                "extname": "mp3",
                "320hash": "81e5f68b4c63ac5d3d5aab2102e23293",
                "mvhash": "",
                "privilege": 0,
                "group": [],
                "album_audio_id": 32586467,
                "album_id": "939265",
                "ownercount": 30576,
                "rp_publish": 1,
                "rp_type": "audio",
                "audio_id": 20567692,
                "320filesize": 9907766,
                "isnew": 0,
                "duration": 247,
                "pkg_price_sq": 0,
                "pkg_price_320": 0,
                "srctype": 1,
                "songname": "相亲相爱",
                "fail_process": 0,
                "sqhash": "116cf6bcd161629404178f83a6811a6e",
                "album_name": "CCTV音乐频道精彩音乐汇合辑",
                "hash": "441a03733122a12f1a95801078715b75",
                "pay_type_sq": 0,
                "320privilege": 0,
                "sqprivilege": 0,
                "sqfilesize": 13738566,
                "othername": ""
            },
            {
                "pay_type_320": 0,
                "m4afilesize": 1327102,
                "price_sq": 0,
                "filesize": 6643045,
                "source": "",
                "bitrate": 129,
                "topic": "",
                "price": 0,
                "Accompany": 0,
                "old_cpy": 1,
                "fail_process_sq": 0,
                "singername": "王力宏",
                "pay_type": 0,
                "sourceid": 0,
                "topic_url": "",
                "fail_process_320": 0,
                "pkg_price": 0,
                "feetype": 0,
                "filename": "王力宏 - 火力全开+龙的传人",
                "price_320": 0,
                "extname": "mp3",
                "320hash": "",
                "mvhash": "",
                "privilege": 0,
                "group": [],
                "album_audio_id": 0,
                "album_id": "",
                "ownercount": 20231,
                "rp_publish": 1,
                "rp_type": "audio",
                "audio_id": 3285166,
                "320filesize": 0,
                "isnew": 0,
                "duration": 415,
                "pkg_price_sq": 0,
                "pkg_price_320": 0,
                "srctype": 1,
                "songname": "火力全开+龙的传人",
                "fail_process": 0,
                "sqhash": "",
                "album_name": "",
                "hash": "e3aef101f1fd2726f84dd09cddc9d132",
                "pay_type_sq": 0,
                "320privilege": 0,
                "sqprivilege": 0,
                "sqfilesize": 0,
                "othername": ""
            },
            {
                "pay_type_320": 0,
                "m4afilesize": 1468053,
                "price_sq": 0,
                "filesize": 5730347,
                "source": "",
                "bitrate": 128,
                "topic": "",
                "price": 0,
                "Accompany": 1,
                "old_cpy": 1,
                "fail_process_sq": 0,
                "singername": "王力宏",
                "pay_type": 0,
                "sourceid": 0,
                "topic_url": "",
                "fail_process_320": 0,
                "pkg_price": 0,
                "feetype": 0,
                "filename": "王力宏 - 改变自己 - DJ版",
                "price_320": 0,
                "extname": "mp3",
                "320hash": "da96a026e1545f12c69dc1a5a0b4c661",
                "mvhash": "",
                "privilege": 0,
                "group": [],
                "album_audio_id": 0,
                "album_id": "",
                "ownercount": 15988,
                "rp_publish": 1,
                "rp_type": "audio",
                "audio_id": 322994,
                "320filesize": 14305656,
                "isnew": 0,
                "duration": 358,
                "pkg_price_sq": 0,
                "pkg_price_320": 0,
                "srctype": 1,
                "songname": "改变自己",
                "fail_process": 0,
                "sqhash": "",
                "album_name": "",
                "hash": "4be8f3c7498b96f3842f2b3d522f6a2a",
                "pay_type_sq": 0,
                "320privilege": 0,
                "sqprivilege": 0,
                "sqfilesize": 0,
                "othername": "DJ版"
            },
            {
                "pay_type_320": 0,
                "m4afilesize": 801030,
                "price_sq": 0,
                "filesize": 3114246,
                "source": "",
                "bitrate": 128,
                "topic": "",
                "price": 0,
                "Accompany": 1,
                "old_cpy": 1,
                "fail_process_sq": 0,
                "singername": "王力宏",
                "pay_type": 0,
                "sourceid": 0,
                "topic_url": "",
                "fail_process_320": 0,
                "pkg_price": 0,
                "feetype": 0,
                "filename": "王力宏 - 改变自己 - 2014-2015浙江卫视跨年演唱会",
                "price_320": 0,
                "extname": "mp3",
                "320hash": "405bdac1c558278bebc6e2c0510fc568",
                "mvhash": "40ea92c2ac8aa94a0d4c67b10e7638bf",
                "privilege": 0,
                "group": [],
                "album_audio_id": 32049530,
                "album_id": "961157",
                "ownercount": 15504,
                "rp_publish": 1,
                "rp_type": "audio",
                "audio_id": 7550238,
                "320filesize": 7786612,
                "isnew": 0,
                "duration": 194,
                "pkg_price_sq": 0,
                "pkg_price_320": 0,
                "srctype": 1,
                "songname": "改变自己",
                "fail_process": 0,
                "sqhash": "",
                "album_name": "2015浙江卫视跨年演唱会",
                "hash": "34ec176b3481c6edad6ba88a2631d23a",
                "pay_type_sq": 0,
                "320privilege": 0,
                "sqprivilege": 0,
                "sqfilesize": 0,
                "othername": "2014-2015浙江卫视跨年演唱会"
            },
            {
                "pay_type_320": 0,
                "m4afilesize": 1551727,
                "price_sq": 0,
                "filesize": 6050380,
                "source": "",
                "bitrate": 128,
                "topic": "",
                "price": 0,
                "Accompany": 1,
                "old_cpy": 1,
                "fail_process_sq": 0,
                "singername": "卢巧音、王力宏",
                "pay_type": 0,
                "sourceid": 0,
                "topic_url": "",
                "fail_process_320": 0,
                "pkg_price": 0,
                "feetype": 0,
                "filename": "卢巧音、王力宏 - 好心分手 - DJ Candy版",
                "price_320": 0,
                "extname": "mp3",
                "320hash": "af741e796d56d2a57b48b0b865c476bb",
                "mvhash": "",
                "privilege": 0,
                "group": [],
                "album_audio_id": 0,
                "album_id": "",
                "ownercount": 14624,
                "rp_publish": 1,
                "rp_type": "audio",
                "audio_id": 245951,
                "320filesize": 15122935,
                "isnew": 0,
                "duration": 378,
                "pkg_price_sq": 0,
                "pkg_price_320": 0,
                "srctype": 1,
                "songname": "好心分手",
                "fail_process": 0,
                "sqhash": "",
                "album_name": "",
                "hash": "4900975fc55915c460360f8bbff6e62b",
                "pay_type_sq": 0,
                "320privilege": 0,
                "sqprivilege": 0,
                "sqfilesize": 0,
                "othername": "DJ Candy版"
            },
            {
                "pay_type_320": 0,
                "m4afilesize": 1109190,
                "price_sq": 0,
                "filesize": 4328384,
                "source": "",
                "bitrate": 128,
                "topic": "",
                "price": 0,
                "Accompany": 1,
                "old_cpy": 1,
                "fail_process_sq": 0,
                "singername": "黄明志、王力宏",
                "pay_type": 0,
                "sourceid": 0,
                "topic_url": "",
                "fail_process_320": 0,
                "pkg_price": 0,
                "feetype": 0,
                "filename": "黄明志、王力宏 - 飘向北方",
                "price_320": 0,
                "extname": "mp3",
                "320hash": "d2bb1ee2952b8ec60eaafbe129190101",
                "mvhash": "6d191e99a4463be484f2bee4fdf47bcc",
                "privilege": 0,
                "group": [],
                "album_audio_id": 54097544,
                "album_id": "1976223",
                "ownercount": 13455,
                "rp_publish": 1,
                "rp_type": "audio",
                "audio_id": 25275642,
                "320filesize": 10821177,
                "isnew": 0,
                "duration": 270,
                "pkg_price_sq": 0,
                "pkg_price_320": 0,
                "srctype": 1,
                "songname": "飘向北方",
                "fail_process": 0,
                "sqhash": "03811eefb04aceec0ed220bfaa3911f2",
                "album_name": "亚洲通车",
                "hash": "d353b69a3b7f1a250000c5daabb8a4f1",
                "pay_type_sq": 0,
                "320privilege": 0,
                "sqprivilege": 0,
                "sqfilesize": 31532562,
                "othername": ""
            },
            {
                "pay_type_320": 0,
                "m4afilesize": 812429,
                "price_sq": 0,
                "filesize": 3092524,
                "source": "",
                "bitrate": 128,
                "topic": "",
                "price": 0,
                "Accompany": 1,
                "old_cpy": 1,
                "fail_process_sq": 0,
                "singername": "王力宏",
                "pay_type": 0,
                "sourceid": 0,
                "topic_url": "",
                "fail_process_320": 0,
                "pkg_price": 0,
                "feetype": 0,
                "filename": "王力宏 - 改变自己 - KTV版伴奏",
                "price_320": 0,
                "extname": "mp3",
                "320hash": "",
                "mvhash": "",
                "privilege": 0,
                "group": [],
                "album_audio_id": 0,
                "album_id": "",
                "ownercount": 11854,
                "rp_publish": 1,
                "rp_type": "audio",
                "audio_id": 322932,
                "320filesize": 0,
                "isnew": 0,
                "duration": 193,
                "pkg_price_sq": 0,
                "pkg_price_320": 0,
                "srctype": 1,
                "songname": "改变自己",
                "fail_process": 0,
                "sqhash": "",
                "album_name": "",
                "hash": "aaaf2fb02c62ff16dfc38a49a34187c8",
                "pay_type_sq": 0,
                "320privilege": 0,
                "sqprivilege": 0,
                "sqfilesize": 0,
                "othername": "KTV版伴奏"
            },
           
            {
                "pay_type_320": 0,
                "m4afilesize": 700851,
                "price_sq": 0,
                "filesize": 2735326,
                "source": "",
                "bitrate": 128,
                "topic": "",
                "price": 0,
                "Accompany": 1,
                "old_cpy": 1,
                "fail_process_sq": 0,
                "singername": "王力宏",
                "pay_type": 0,
                "sourceid": 0,
                "topic_url": "",
                "fail_process_320": 0,
                "pkg_price": 0,
                "feetype": 0,
                "filename": "王力宏 - 依然爱你 - Live",
                "price_320": 0,
                "extname": "mp3",
                "320hash": "",
                "mvhash": "",
                "privilege": 0,
                "group": [],
                "album_audio_id": 0,
                "album_id": "",
                "ownercount": 7298,
                "rp_publish": 1,
                "rp_type": "audio",
                "audio_id": 16733526,
                "320filesize": 0,
                "isnew": 0,
                "duration": 171,
                "pkg_price_sq": 0,
                "pkg_price_320": 0,
                "srctype": 1,
                "songname": "依然爱你",
                "fail_process": 0,
                "sqhash": "",
                "album_name": "",
                "hash": "eaaa967a9af1ada1af52713a457d9aca",
                "pay_type_sq": 0,
                "320privilege": 0,
                "sqprivilege": 0,
                "sqfilesize": 0,
                "othername": "Live"
            }
        ],
        "correctiontype": 0,
        "timestamp": 1500209418,
        "allowerr": 0,
        "total": 480,
        "istag": 0,
        "istagresult": 0,
        "forcecorrection": 0,
        "correctiontip": ""
    },
    "errcode": 0
}

```






