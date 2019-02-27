# wenziyun
基于echarts的自定义图像的文字云
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>WordCloud Demo</title>
    <script src='https://cdn.bootcss.com/echarts/3.7.0/echarts.simple.js'></script>
        <script src='../dist/echarts-wordcloud.js'></script>
</head>
<body>
    <div id="main" style="width: 800px; height: 600px"></div>
    <script>
        onload = function () {
            var data = {
                value: [{
                    "name": "花鸟市场",
                    "value": 1446
                },
                    {
                        "name": "汽车",
                        "value": 928
                    },
                    {
                        "name": "视频",
                        "value": 906
                    },
                    {
                        "name": "电视",
                        "value": 825
                    },
                    {
                        "name": "Lover Boy 88",
                        "value": 514
                    },
                    {
                        "name": "动漫",
                        "value": 486
                    },
                    {
                        "name": "音乐",
                        "value": 53
                    },
                    {
                        "name": "直播",
                        "value": 163
                    },
                    {
                        "name": "广播电台",
                        "value": 86
                    },
                    {
                        "name": "戏曲曲艺",
                        "value": 17
                    },
                    {
                        "name": "演出票务",
                        "value": 6
                    },
                    {
                        "name": "给陌生的你听",
                        "value": 1
                    },
                    {
                        "name": "资讯",
                        "value": 1437
                    },
                    {
                        "name": "商业财经",
                        "value": 422
                    },
                    {
                        "name": "娱乐八卦",
                        "value": 353
                    },
                    {
                        "name": "军事",
                        "value": 331
                    },
                    {
                        "name": "科技资讯",
                        "value": 313
                    },
                    {
                        "name": "社会时政",
                        "value": 307
                    },
                    {
                        "name": "时尚",
                        "value": 43
                    },
                    {
                        "name": "网络奇闻",
                        "value": 15
                    },
                    {
                        "name": "旅游出行",
                        "value": 438
                    },
                    {
                        "name": "景点类型",
                        "value": 957
                    },
                    {
                        "name": "国内游",
                        "value": 927
                    },
                    {
                        "name": "远途出行方式",
                        "value": 908
                    },
                    {
                        "name": "酒店",
                        "value": 693
                    },
                    {
                        "name": "关注景点",
                        "value": 611
                    },
                    {
                        "name": "旅游网站偏好",
                        "value": 512
                    },
                    {
                        "name": "出国游",
                        "value": 382
                    },
                    {
                        "name": "交通票务",
                        "value": 312
                    },
                    {
                        "name": "旅游方式",
                        "value": 187
                    },
                    {
                        "name": "旅游主题",
                        "value": 163
                    },
                    {
                        "name": "港澳台",
                        "value": 104
                    },
                    {
                        "name": "本地周边游",
                        "value": 3
                    },
                    {
                        "name": "小卖家",
                        "value": 1331
                    },
                    {
                        "name": "全日制学校",
                        "value": 941
                    },
                    {
                        "name": "基础教育科目",
                        "value": 585
                    },
                    {
                        "name": "考试培训",
                        "value": 473
                    },
                    {
                        "name": "语言学习",
                        "value": 358
                    },
                    {
                        "name": "留学",
                        "value": 246
                    },
                    {
                        "name": "K12课程培训",
                        "value": 207
                    },
                    {
                        "name": "艺术培训",
                        "value": 194
                    },
                    {
                        "name": "技能培训",
                        "value": 104
                    },
                    {
                        "name": "IT培训",
                        "value": 87
                    },
                    {
                        "name": "高等教育专业",
                        "value": 63
                    },
                    {
                        "name": "家教",
                        "value": 48
                    },
                    {
                        "name": "体育培训",
                        "value": 23
                    },
                    {
                        "name": "职场培训",
                        "value": 5
                    },
                    {
                        "name": "金融财经",
                        "value": 1328
                    },
                    {
                        "name": "银行",
                        "value": 765
                    },
                    {
                        "name": "股票",
                        "value": 452
                    },
                    {
                        "name": "保险",
                        "value": 415
                    },
                    {
                        "name": "贷款",
                        "value": 253
                    },
                    {
                        "name": "基金",
                        "value": 211
                    },
                    {
                        "name": "信用卡",
                        "value": 180
                    },
                    {
                        "name": "外汇",
                        "value": 138
                    },
                    {
                        "name": "P2P",
                        "value": 116
                    },
                    {
                        "name": "贵金属",
                        "value": 98
                    },
                    {
                        "name": "债券",
                        "value": 93
                    },
                    {
                        "name": "网络理财",
                        "value": 92
                    },
                    {
                        "name": "信托",
                        "value": 90
                    },
                    {
                        "name": "征信",
                        "value": 76
                    },
                    {
                        "name": "期货",
                        "value": 76
                    },
                    {
                        "name": "公积金",
                        "value": 40
                    },
                    {
                        "name": "银行理财",
                        "value": 36
                    },
                    {
                        "name": "银行业务",
                        "value": 30
                    },
                    {
                        "name": "典当",
                        "value": 7
                    },
                    {
                        "name": "海外置业",
                        "value": 1
                    },
                    {
                        "name": "汽车",
                        "value": 1309
                    },
                    {
                        "name": "汽车档次",
                        "value": 965
                    },
                    {
                        "name": "汽车品牌",
                        "value": 900
                    },
                    {
                        "name": "汽车车型",
                        "value": 727
                    },
                    {
                        "name": "购车阶段",
                        "value": 461
                    },
                    {
                        "name": "二手车",
                        "value": 309
                    },
                    {
                        "name": "汽车美容",
                        "value": 260
                    },
                    {
                        "name": "新能源汽车",
                        "value": 173
                    },
                    {
                        "name": "汽车维修",
                        "value": 155
                    },
                    {
                        "name": "租车服务",
                        "value": 136
                    },
                    {
                        "name": "车展",
                        "value": 121
                    },
                    {
                        "name": "违章查询",
                        "value": 76
                    },
                    {
                        "name": "汽车改装",
                        "value": 62
                    },
                    {
                        "name": "汽车用品",
                        "value": 37
                    },
                    {
                        "name": "路况查询",
                        "value": 32
                    },
                    {
                        "name": "汽车保险",
                        "value": 28
                    },
                    {
                        "name": "陪驾代驾",
                        "value": 4
                    },
                    {
                        "name": "网络购物",
                        "value": 1275
                    },
                    {
                        "name": "做我的猫",
                        "value": 1088
                    },
                    {
                        "name": "只想要你知道",
                        "value": 907
                    },
                    {
                        "name": "团购",
                        "value": 837
                    },
                    {
                        "name": "比价",
                        "value": 201
                    },
                    {
                        "name": "海淘",
                        "value": 195
                    },
                    {
                        "name": "移动APP购物",
                        "value": 179
                    },
                    {
                        "name": "支付方式",
                        "value": 119
                    },
                    {
                        "name": "代购",
                        "value": 43
                    },
                    {
                        "name": "体育健身",
                        "value": 1234
                    },
                    {
                        "name": "体育赛事项目",
                        "value": 802
                    },
                    {
                        "name": "运动项目",
                        "value": 405
                    },
                    {
                        "name": "体育类赛事",
                        "value": 337
                    },
                    {
                        "name": "健身项目",
                        "value": 199
                    },
                    {
                        "name": "健身房健身",
                        "value": 78
                    },
                    {
                        "name": "运动健身",
                        "value": 77
                    },
                    {
                        "name": "家庭健身",
                        "value": 36
                    },
                    {
                        "name": "健身器械",
                        "value": 29
                    },
                    {
                        "name": "办公室健身",
                        "value": 3
                    },
                    {
                        "name": "商务服务",
                        "value": 1201
                    },
                    {
                        "name": "法律咨询",
                        "value": 508
                    },
                    {
                        "name": "化工材料",
                        "value": 147
                    },
                    {
                        "name": "广告服务",
                        "value": 125
                    },
                    {
                        "name": "会计审计",
                        "value": 115
                    },
                    {
                        "name": "人员招聘",
                        "value": 101
                    },
                    {
                        "name": "印刷打印",
                        "value": 66
                    },
                    {
                        "name": "知识产权",
                        "value": 32
                    },
                    {
                        "name": "翻译",
                        "value": 22
                    },
                    {
                        "name": "安全安保",
                        "value": 9
                    },
                    {
                        "name": "公关服务",
                        "value": 8
                    },
                    {
                        "name": "商旅服务",
                        "value": 2
                    },
                    {
                        "name": "展会服务",
                        "value": 2
                    },
                    {
                        "name": "特许经营",
                        "value": 1
                    },
                    {
                        "name": "休闲爱好",
                        "value": 1169
                    },
                    {
                        "name": "收藏",
                        "value": 412
                    },
                    {
                        "name": "摄影",
                        "value": 393
                    },
                    {
                        "name": "温泉",
                        "value": 230
                    },
                    {
                        "name": "博彩彩票",
                        "value": 211
                    },
                    {
                        "name": "美术",
                        "value": 207
                    },
                    {
                        "name": "书法",
                        "value": 139
                    },
                    {
                        "name": "DIY手工",
                        "value": 75
                    },
                    {
                        "name": "舞蹈",
                        "value": 23
                    },
                    {
                        "name": "钓鱼",
                        "value": 21
                    },
                    {
                        "name": "棋牌桌游",
                        "value": 17
                    },
                    {
                        "name": "KTV",
                        "value": 6
                    },
                    {
                        "name": "密室",
                        "value": 5
                    },
                    {
                        "name": "采摘",
                        "value": 4
                    },
                    {
                        "name": "电玩",
                        "value": 1
                    },
                    {
                        "name": "真人CS",
                        "value": 1
                    },
                    {
                        "name": "轰趴",
                        "value": 1
                    },
                    {
                        "name": "家电数码",
                        "value": 1111
                    },
                    {
                        "name": "手机",
                        "value": 885
                    },
                    {
                        "name": "电脑",
                        "value": 543
                    },
                    {
                        "name": "大家电",
                        "value": 321
                    },
                    {
                        "name": "家电关注品牌",
                        "value": 253
                    },
                    {
                        "name": "网络设备",
                        "value": 162
                    },
                    {
                        "name": "摄影器材",
                        "value": 149
                    },
                    {
                        "name": "影音设备",
                        "value": 133
                    },
                    {
                        "name": "办公数码设备",
                        "value": 113
                    },
                    {
                        "name": "生活电器",
                        "value": 67
                    },
                    {
                        "name": "厨房电器",
                        "value": 54
                    },
                    {
                        "name": "智能设备",
                        "value": 45
                    },
                    {
                        "name": "个人护理电器",
                        "value": 22
                    },
                    {
                        "name": "服饰鞋包",
                        "value": 1047
                    },
                    {
                        "name": "服装",
                        "value": 566
                    },
                    {
                        "name": "饰品",
                        "value": 289
                    },
                    {
                        "name": "鞋",
                        "value": 184
                    },
                    {
                        "name": "箱包",
                        "value": 168
                    },
                    {
                        "name": "奢侈品",
                        "value": 137
                    },
                    {
                        "name": "母婴亲子",
                        "value": 1041
                    },
                    {
                        "name": "孕婴保健",
                        "value": 505
                    },
                    {
                        "name": "母婴社区",
                        "value": 299
                    },
                    {
                        "name": "早教",
                        "value": 103
                    },
                    {
                        "name": "奶粉辅食",
                        "value": 66
                    },
                    {
                        "name": "童车童床",
                        "value": 41
                    },
                    {
                        "name": "关注品牌",
                        "value": 271
                    },
                    {
                        "name": "宝宝玩乐",
                        "value": 30
                    },
                    {
                        "name": "母婴护理服务",
                        "value": 25
                    },
                    {
                        "name": "纸尿裤湿巾",
                        "value": 16
                    },
                    {
                        "name": "妈妈用品",
                        "value": 15
                    },
                    {
                        "name": "宝宝起名",
                        "value": 12
                    },
                    {
                        "name": "童装童鞋",
                        "value": 9
                    },
                    {
                        "name": "胎教",
                        "value": 8
                    },
                    {
                        "name": "宝宝安全",
                        "value": 1
                    },
                    {
                        "name": "宝宝洗护用品",
                        "value": 1
                    },
                    {
                        "name": "软件应用",
                        "value": 1018
                    },
                    {
                        "name": "系统工具",
                        "value": 896
                    },
                    {
                        "name": "理财购物",
                        "value": 440
                    },
                    {
                        "name": "生活实用",
                        "value": 365
                    },
                    {
                        "name": "影音图像",
                        "value": 256
                    },
                    {
                        "name": "社交通讯",
                        "value": 214
                    },
                    {
                        "name": "手机美化",
                        "value": 39
                    },
                    {
                        "name": "办公学习",
                        "value": 28
                    },
                    {
                        "name": "应用市场",
                        "value": 23
                    },
                    {
                        "name": "母婴育儿",
                        "value": 14
                    },
                    {
                        "name": "游戏",
                        "value": 946
                    },
                    {
                        "name": "手机游戏",
                        "value": 565
                    },
                    {
                        "name": "PC游戏",
                        "value": 353
                    },
                    {
                        "name": "网页游戏",
                        "value": 254
                    },
                    {
                        "name": "游戏机",
                        "value": 188
                    },
                    {
                        "name": "模拟辅助",
                        "value": 166
                    },
                    {
                        "name": "个护美容",
                        "value": 942
                    },
                    {
                        "name": "护肤品",
                        "value": 177
                    },
                    {
                        "name": "彩妆",
                        "value": 133
                    },
                    {
                        "name": "美发",
                        "value": 80
                    },
                    {
                        "name": "香水",
                        "value": 50
                    },
                    {
                        "name": "个人护理",
                        "value": 46
                    },
                    {
                        "name": "美甲",
                        "value": 26
                    },
                    {
                        "name": "SPA美体",
                        "value": 21
                    },
                    {
                        "name": "花鸟萌宠",
                        "value": 914
                    },
                    {
                        "name": "绿植花卉",
                        "value": 311
                    },
                    {
                        "name": "狗",
                        "value": 257
                    },
                    {
                        "name": "其他宠物",
                        "value": 131
                    },
                    {
                        "name": "水族",
                        "value": 125
                    },
                    {
                        "name": "猫",
                        "value": 122
                    },
                    {
                        "name": "动物",
                        "value": 81
                    },
                    {
                        "name": "鸟",
                        "value": 67
                    },
                    {
                        "name": "宠物用品",
                        "value": 41
                    },
                    {
                        "name": "宠物服务",
                        "value": 26
                    },
                    {
                        "name": "书籍阅读",
                        "value": 913
                    },
                    {
                        "name": "网络小说",
                        "value": 483
                    },
                    {
                        "name": "关注书籍",
                        "value": 128
                    },
                    {
                        "name": "文学",
                        "value": 105
                    },
                    {
                        "name": "报刊杂志",
                        "value": 77
                    },
                    {
                        "name": "人文社科",
                        "value": 22
                    },
                    {
                        "name": "建材家居",
                        "value": 907
                    },
                    {
                        "name": "装修建材",
                        "value": 644
                    },
                    {
                        "name": "家具",
                        "value": 273
                    },
                    {
                        "name": "家居风格",
                        "value": 187
                    },
                    {
                        "name": "家居家装关注品牌",
                        "value": 140
                    },
                    {
                        "name": "家纺",
                        "value": 107
                    },
                    {
                        "name": "厨具",
                        "value": 47
                    },
                    {
                        "name": "灯具",
                        "value": 43
                    },
                    {
                        "name": "家居饰品",
                        "value": 29
                    },
                    {
                        "name": "家居日常用品",
                        "value": 10
                    },
                    {
                        "name": "生活服务",
                        "value": 883
                    },
                    {
                        "name": "物流配送",
                        "value": 536
                    },
                    {
                        "name": "家政服务",
                        "value": 108
                    },
                    {
                        "name": "摄影服务",
                        "value": 49
                    },
                    {
                        "name": "搬家服务",
                        "value": 38
                    },
                    {
                        "name": "物业维修",
                        "value": 37
                    },
                    {
                        "name": "婚庆服务",
                        "value": 24
                    },
                    {
                        "name": "二手回收",
                        "value": 24
                    },
                    {
                        "name": "鲜花配送",
                        "value": 3
                    },
                    {
                        "name": "维修服务",
                        "value": 3
                    },
                    {
                        "name": "殡葬服务",
                        "value": 1
                    },
                    {
                        "name": "求职创业",
                        "value": 874
                    },
                    {
                        "name": "创业",
                        "value": 363
                    },
                    {
                        "name": "目标职位",
                        "value": 162
                    },
                    {
                        "name": "目标行业",
                        "value": 50
                    },
                    {
                        "name": "兼职",
                        "value": 21
                    },
                    {
                        "name": "期望年薪",
                        "value": 20
                    },
                    {
                        "name": "实习",
                        "value": 16
                    },
                    {
                        "name": "雇主类型",
                        "value": 10
                    },
                    {
                        "name": "星座运势",
                        "value": 789
                    },
                    {
                        "name": "星座",
                        "value": 316
                    },
                    {
                        "name": "算命",
                        "value": 303
                    },
                    {
                        "name": "解梦",
                        "value": 196
                    },
                    {
                        "name": "风水",
                        "value": 93
                    },
                    {
                        "name": "面相分析",
                        "value": 47
                    },
                    {
                        "name": "手相",
                        "value": 32
                    },
                    {
                        "name": "公益",
                        "value": 90
                    }
                ],
                // 自定义图形，base64格式的
                //小鸟图片----
                // image: "data:image/png;base64,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"
                // image: "data:image/png;base64,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"
                // 人形状
                image: "data:image/png;base64,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"
            }
            var myChart = echarts.init(document.getElementById('main'));
            //温馨提示：image 选取有严格要求不可过大；，否则firefox不兼容  iconfont上面的图标可以
            var maskImage = new Image();
            maskImage.src = data.image
 
            maskImage.onload = function(){
                myChart.setOption( {
                    backgroundColor:'#fff',
                    tooltip: {
                        show: false
                    },
                    series: [{
                        type: 'wordCloud',
                        gridSize: 1,
                        sizeRange: [12, 55],
                        rotationRange: [-45, 0, 45, 90],
                        maskImage: maskImage,
                        textStyle: {
                            normal: {
                                color: function() {
                                    return 'rgb(' +
                                            Math.round(Math.random() * 255) +
                                            ', ' + Math.round(Math.random() * 255) +
                                            ', ' + Math.round(Math.random() * 255) + ')'
                                }
                            }
                        },
                        left: 'center',
                        top: 'center',
                        // width: '96%',
                        // height: '100%',
                        right: null,
                        bottom: null,
                        // width: 300,
                        // height: 200,
                        // top: 20,
                        data: data.value
                    }]
                })
            }
 
        }
    </script>
</body>
</html>
