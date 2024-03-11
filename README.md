## fanqie-novel-api

环境变量设置

- DATABASE_TYPE 可选： mysql
- DSN 填写mysql时必填

默认端口：8080

默认数据库sqlite

## 搜索

```shell
curl --location --request GET 'http://127.0.0.1:8000/book/search?name=末日全球海洋，勒索校花百万物资'

```

```json
{
    "code": 200,
    "data": [
        {
            "BookID": 7246248681131740175,
            "Name": "末日全球海洋，勒索校花百万物资",
            "Author": "田师傅",
            "Desc": "【暴雨，海洋，诺亚方舟，机甲，女神，囤物资】\n一场灭世大雨，淹没了整个世界。\n上一世的陈澈被校花带上船，本以为是救赎，却被当狗养，更被其踹进海底葬身。\n重生到末日来临七天前，陈澈绑定诺亚方舟。\n获取人口奖励：全身覆盖式机甲、重型载人机甲、生物机械体外装甲、生物初号机。\n没钱囤物资？\n直接勒索校花百万吨物资！\n不仅索物，还要索人！\n上辈子你做人，我做狗，这辈子，咱俩换换。",
            "Category": "科幻",
            "CreationStatus": "0",
            "ChaptersCount": 0,
            "FirstChapterId": 7246248906823205411,
            "LastChapterId": 7343307912736932376,
            "LastChapterTime": 1709747259,
            "Score": 8.5,
            "WordCount": 1056708,
            "ReadCount": 132286,
            "ThumbUrl": "http://p3-reading-sign.fqnovelpic.com/novel-pic/p2o344cc0bc26d0392138f24d2a9a22b326~tplv-resize:200:260.image?lk3s=8c91f0b0&x-expires=1712716529&x-signature=E3EpHlk32CyEehy2CJ62FHSbYRk%3D",
            "ID": 1,
            "CreatedAt": "2024-03-11T10:35:37.422+08:00",
            "UpdatedAt": "2024-03-11T10:35:37.422+08:00",
            "DeletedAt": null
        },
        {
            "BookID": 7294566552941382694,
            "Name": "末日全球海洋，勒索校花百万物资",
            "Author": "宁大公子",
            "Desc": "【暴雨，海洋，诺亚方舟，机甲，女神，囤物资】\n一场灭世大雨，淹没了整个世界。\n上一世的陈澈被校花带上船，本以为是救赎，却被当狗养，更被其踹进海底葬身。\n重生到末日来临七天前，陈澈绑定诺亚方舟。\n获取人口奖励：全身覆盖式机甲、重型载人机甲、生物机械体外装甲、生物初号机。\n没钱囤物资？\n直接勒索校花百万吨物资！\n不仅索物，还要索人！\n上辈子你做人，我做狗，这辈子，咱俩换换。",
            "Category": "科幻",
            "CreationStatus": "1",
            "ChaptersCount": 0,
            "FirstChapterId": 0,
            "LastChapterId": 0,
            "LastChapterTime": 0,
            "Score": 8.5,
            "WordCount": 0,
            "ReadCount": 0,
            "ThumbUrl": "",
            "ID": 2,
            "CreatedAt": "2024-03-11T10:35:37.838+08:00",
            "UpdatedAt": "2024-03-11T10:35:37.838+08:00",
            "DeletedAt": null
        }
    ],
    "msg": "success"
}
```

## 详情

```shell
curl --location --request GET 'http://127.0.0.1:8000/book/detail?book_id=7246248681131740175'
```

```json
{
    "code": 200,
    "data": {
        "BookID": 7246248681131740175,
        "Name": "末日全球海洋，勒索校花百万物资",
        "Author": "田师傅",
        "Desc": "【暴雨，海洋，诺亚方舟，机甲，女神，囤物资】\n一场灭世大雨，淹没了整个世界。\n上一世的陈澈被校花带上船，本以为是救赎，却被当狗养，更被其踹进海底葬身。\n重生到末日来临七天前，陈澈绑定诺亚方舟。\n获取人口奖励：全身覆盖式机甲、重型载人机甲、生物机械体外装甲、生物初号机。\n没钱囤物资？\n直接勒索校花百万吨物资！\n不仅索物，还要索人！\n上辈子你做人，我做狗，这辈子，咱俩换换。",
        "Category": "科幻",
        "CreationStatus": "0",
        "ChaptersCount": 0,
        "FirstChapterId": 7246248906823205411,
        "LastChapterId": 7343307912736932376,
        "LastChapterTime": 1709747259,
        "Score": 8.5,
        "WordCount": 1056708,
        "ReadCount": 132286,
        "ThumbUrl": "http://p3-reading-sign.fqnovelpic.com/novel-pic/p2o344cc0bc26d0392138f24d2a9a22b326~tplv-resize:200:260.image?lk3s=8c91f0b0&x-expires=1712716529&x-signature=E3EpHlk32CyEehy2CJ62FHSbYRk%3D",
        "ID": 1,
        "CreatedAt": "2024-03-11T10:35:37.422+08:00",
        "UpdatedAt": "2024-03-11T10:35:37.422+08:00",
        "DeletedAt": null
    },
    "msg": "success"
}
```

## 目录

```shell
curl --location --request GET 'http://127.0.0.1:8000/book/directory?book_id=7246248681131740175'
```

```json
{
  "code": 200,
  "data": [
    {
      "ChapterID": 7246248906823205411,
      "Name": "第1章 要挟校花",
      "BookId": 7246248681131740175,
      "ChapterNumber": 0,
      "WordCount": 0,
      "Content": "",
      "NextGroupID": 7246249594810860092,
      "NextItemID": 7246249594810860092,
      "PreGroupID": 0,
      "PreItemID": 0,
      "ID": 315,
      "CreatedAt": "2024-03-11T10:38:46.016+08:00",
      "UpdatedAt": "2024-03-11T10:38:46.016+08:00",
      "DeletedAt": null
    },
    {
      "ChapterID": 7246249594810860092,
      "Name": "第2章 开房还要女神付房费？",
      "BookId": 7246248681131740175,
      "ChapterNumber": 0,
      "WordCount": 0,
      "Content": "",
      "NextGroupID": 7246249925414126114,
      "NextItemID": 7246249925414126114,
      "PreGroupID": 7246248906823205411,
      "PreItemID": 7246248906823205411,
      "ID": 316,
      "CreatedAt": "2024-03-11T10:38:46.016+08:00",
      "UpdatedAt": "2024-03-11T10:38:46.016+08:00",
      "DeletedAt": null
    }
  ],
  "msg": "success"
}
```

## 正文

```shell
curl --location --request GET 'http://127.0.0.1:8000/chapter/content?chapter_id=7246248906823205411'
```

```json
{
    "code": 200,
    "data": {
        "ChapterID": 7246248906823205411,
        "Name": "第1章 要挟校花",
        "BookId": 7246248681131740175,
        "ChapterNumber": 1,
        "WordCount": 2146,
        "Content": "\n“俞栀子，我屮你个dog太阳的……”\n在一阵大骂声中，陈澈从宿舍床上猛然惊醒。\n“哈！”\n陈澈大口喘着粗气，呼吸着难得的新鲜空气，记忆仍停留在被海水侵蚀的最后一刻。\n2023年末，一场灭世大雨淹没了整个世界。\n人类迎来灭顶之灾，死伤无数。\n陈澈运气好，被同校校花俞栀子救了。\n可惜好景不长，社会秩序崩坏后，人性阴暗面无限放大，仙气飘飘的校花，也仗着背景变成黑心白莲。\n把陈澈和一众同学当狗使唤不说，还让他们下海抓那些恐怖的深海生物。\n陈澈就是在被俞栀子一脚踹下船后，死在了一只深海生物嘴里。\n只是现在……\n窗外阳光明媚，阳台上的衣服随风轻摆，将淡淡的洗衣粉味道撒进鼻息。\n眼前的一切，都像极了自己当初的大学宿舍。\n再摸出床头的手机看看时间。\n2023年12月24日。\n“我重生了！”\n重生在末日到来的七天前。\n陈澈下床，走到阳台上，不敢相信眼前的一切。\n天空蔚蓝没有一片乌云，楼下全是青春活泼，打扮干净的同学。\n远处操场的篮球不停跳动着，旁边小树林不时有狗♂♀进进出出。\n窗外的一切都美的不真实。\n“呼。”\n陈澈长出一口气，一直紧绷的神经，终于随之松懈。\n还有什么比淹死后，来一口新鲜空气更让人沉醉的。\n不过这样的宁静，也只剩下七天了。\n想到七天后那场泼天大雨，陈澈难免心头一沉。\n那场雨下的太大，太久。\n想要在这场灭世大雨里活下去，自己得在这宝贵的七天里，做好充足的准备。\n首先要做的，就是买一条足够大的船。\n想到就做，陈澈第一时间拿出手机，看了眼卡里余额。\n“637块5。”\n陈澈眯眼：“应该够买桶船漆了。”\n“我去你大爷的！”\n陈澈一把将手机摔了。\n好不容易重生再来一次，结果第一步就卡死了。\n想找人借钱，可他一个孤儿，无依无靠，顶多找身边同学再借几桶油漆钱，屁用没有。\n正纠结时，脑海里忽然响起一道电子音。\n【诺亚方舟操作系统绑定船长】\n同时一个3D船体形象，出现在陈澈的脑海里。\n“这是……”\n陈澈有点懵，想起了曾经看过的小说。\n自己也成了被系统选中的男人？\n不过这系统咋是个破船的操作系统？\n随着陈澈的意念，脑海里的3D船体不断转动，各项船体数据也随之浮现。\n“船身长度三千米？！！”\n据陈澈了解。\n现有世界上最大的船只，也才1371米，自己脑子里装了艘比这还大两倍有余的？\n【诺亚方舟一切数据经过系统反复测算，真实，有效】\n陈澈花了一个小时的时间，终于对自己脑子里突然出现的诺亚方舟有所了解。\n简单来说，船的问题解决了。\n不仅解决了，而且解决的很完美。\n方舟拥有远超现代的科技水平，能在各方面为陈澈提供巨大的帮助。\n不仅拥有超大空间的船舱可以储存物资，方舟上还有大量的武器，用以保障陈澈的安全。\n除此之外，方舟系统还有各项任务，完成后可以获得相应的奖励。\n有了这艘堪比海上移动城市的方舟，陈澈在末日里活下去的几率，将比任何人都大。\n甚至陈澈愿意的话，还可以带数十万人登船。\n唯一的限制，就是末日到来后，方舟才能具现。\n船的问题解决了，接下来就是食物的问题。\n灭世大雨后，食物异常紧缺。\n一包方便面就能引起一桩血案。\n一根火腿肠就能换个女人。\n当然，末日前偶尔也能用火腿肠换个女人。\n陈澈现在有诺亚方舟，食物的储藏完全不用担心，唯一有问题的，就是637块5。\n这么点钱，全买泡面大米也不够吃。\n“难道现在就去偷？”\n末日之后，秩序崩坏，自然没人管你偷或抢。\n但现在还不行。\n陈澈今天敢去偷，明天就得蹲牢里。\n到时候大雨给他淹了，想跑都跑不了。\n陈澈趴在阳台上，想了半天始终没想出什么好办法筹集钱和物资。\n一个一穷二白的学生，哪怕知道世界即将末日，压根也没办法搞到钱和物资。\n即便是撸高利贷，以他的条件顶多也就撸个二十万。\n杯水车薪。\n“俞栀子！”\n陈澈忽然瞥见了操场上一闪而过的身影。\n她长发披肩，穿着浅蓝色的连衣裙，露出一截白嫩的小腿，藏进白色的短袜里，所过之处回头率极高。\n抛开人性不谈，俞栀子这个校花当之无愧。\n颜值之高，就连陈澈这个上辈子的仇人，都忍不住夸赞一句。\n“长的真牛逼。”\n看着看着，陈澈忽然笑了。\n重生一世，自己不仅有机会报仇，钱的问题，似乎也能解决了。\n俞栀子家里很有钱。\n其父是国内有名的船舶大王，资产几十亿。\n这也是俞栀子末日后依然生活滋润的关键。\n而在末世里和俞栀子接触过很长一段时间的陈澈，恰好知道几个俞栀子的秘密。\n很快。\n陈澈追到了俞栀子所在的宿舍楼下。\n直接上去肯定是上不去的。\n左右看了看，恰好看见一个俞栀子的室友。\n连忙拦住：“同学，能帮我叫下俞栀子吗？”\n室友上下打量陈澈一眼，娇笑：“你两手空空的就想找咱们俞大校花表白吗？”\n陈澈愣了下，反应过来。\n以俞栀子的颜值和背景，找她表白的人不计其数。\n以至于是个男生过来找俞栀子，都会被误以为是表白。\n“我不表白。”\n陈澈摇头：“你就说王艳找她。”\n高中时的俞栀子，跋扈至极，霸凌过无数学生。\n王艳就是其中之一。\n甚至被欺负致死。\n不过几分钟，刚刚上楼的俞栀子又下来了。\n蹙着一双好看的秀眉，莲步轻移，在陈澈身前一米站定。\n朱唇轻启，清澈的嗓音响起：“你认识王艳？”\n陈澈没有反应，眼睛直勾勾的盯着那张好看的脸，情绪逐渐涌动。\n谁能想到这么漂亮的女生，心比墨都黑。\n末日到来后，他被这个女人折磨足足一个月。\n没睡过一个好觉，没吃过一顿好饭。\n印象最深的一次，是这个沙壁女人模仿动画情节。\n一边让他算数，一边拿老虎钳子拔他指甲。\n想着想着，陈澈控制不住了。\n啪！\n突如其来的一巴掌，扇懵了俞栀子，也扇灭了整栋楼的喧闹。",
        "NextGroupID": 7246249594810860092,
        "NextItemID": 7246249594810860092,
        "PreGroupID": 0,
        "PreItemID": 0,
        "ID": 0,
        "CreatedAt": "0001-01-01T00:00:00Z",
        "UpdatedAt": "0001-01-01T00:00:00Z",
        "DeletedAt": null
    },
    "msg": "success"
}
```