# 关于107.173.42[.]94 盗刷 tokens 以及这个ip后面的某位佬

Source: https://linux.do/t/topic/2852798
Version: v1
Posts: 133
Missing floors: none

## #1 慕鸢 (@user792)

Created: 2026-09-04T01:52:39.642Z
Updated: 2026-09-04T01:52:39.642Z

[6月 18 日] 有人发帖说自己的cpa被盗刷，结果这个ip把自己的80端口重定向到 [muyuan.do](http://muyuan.do)

  
    

    ![](https://linux.do/assets/mirrored/ff/ff9d9a70835c8dc6878ba6abf7beb16c6c9768f530ac52c8f0251550090d1b46.png)
    
      [cpa 被来自 racknerd 的ip 107.173.42.94 盗刷, 举报有效, 已经suspend了该server.](https://linux.do/t/topic/2426372) [
  

开发调优](https://linux.do/c/develop/4)
    

  

  
> 今早使用codex, 返回429 rate limit, 好奇怪, 上cpa面板一看, 4个账号3个账号达到5小时限制了, token还在不断地飙升. 赶紧让claude把它停了, 然后查log, 一看来自ip 107.173.42.94 在狂刷. 查了一下ip 107.173.42.94, 是racknerd, 已经向racknerd举报. 
> 没太想清楚key怎么被获得的. 以前这个cpa是安装…

[6月 23 日] 我发帖澄清

  
    

    ![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png)
    
      [舆论对立挑不起来，跟我玩栽赃是吧](https://linux.do/t/topic/2461064) [
  

搞七捻三](https://linux.do/c/gossip/11)
    

  

  
> 热更新 
> 这个ip死了，下次别陷害了 
> 
> 107.173.42.94 
> 
> 分割线 
> 从 [cpa 被来自 racknerd 的ip 107.173.42.94 盗刷, 举报有效, 已经suspend了该server. - #15，来自 cheeryman](https://linux.do/t/topic/2426372/15) 继续讨论， 
> 我的基本上所有的服务器都在ovh，都是物理机，我不至于穷到用rn，别瞎说 
> 有一点家宽和线路机 
> 具体请看，[君の守望](https://server.centos.hk/)

[6月 18 日] 一位热心佬友开始追踪，发现了一些确切的痕迹，明确这位盗刷者的身份，但是并没有公布

  
    

    ![](https://linux.do/assets/mirrored/be/bed29452f22066ece7e974e97499cfd9a998858d1ac27866006fa78f430e59ee.png)
    
      [[update]用事实证据还慕鸢【君の守望】公益站一个清白，关于 107.173.42[.]94 我所观察到的一切](https://linux.do/t/topic/2461746) [
  

搞七捻三](https://linux.do/c/gossip/11)
    

  

  
> 从[舆论对立挑不起来，跟我玩栽赃是吧](https://linux.do/t/topic/2461064)继续讨论： 
> [#p-19506427-h-1](#p-19506427-h-1)以下内容无任何臆测，数据均来自第三方网络平台。
> [#p-19506427-h-1071734294-2](#p-19506427-h-1071734294-2)107.173.42.94 到底是谁在使用？
> 严谨调查，事实说话，首先常规操作起手： 
> 
> 
> 来自微步的SSL证书 
>  [[截屏2026-06-24 00.00.07]](https://cdn3.ldstatic.com/original/4X/0/1/0/010b4e285b1ce82cff055d333566731377686a47.png) 
> 
> 
> 来自 Quake 的SSL证书 
>  [[截屏2026-06-24 00.02.01]](https://cdn3.ldstatic.com/original/4X/f/0/5/f054ca51f44cac747892e75397980bd77d4ee4e4.jpeg) 
> 
> 
> 现在所有证据都指向 744000[.]xy…

[9月 3 日]

这个ip再次盗刷tokens

  
    

    ![](https://linux.do/assets/mirrored/33/332251ae47a6d876b662752a7200858ae081cba9bd7d0054da979f7097fcd519.png)
    
      [部署的 sub2api 被偷 token 了](https://linux.do/t/topic/2849378) [
  

搞七捻三](https://linux.do/c/gossip/11)
    

  

  
> ![sweat_smile](https://linux.do/assets/mirrored/7c/7cabe38e4fbcd004aabe3211ed481ef540cca0969ad30eed19080a96eee1165f.png) 
> 肯定是站内的某位大佬干的。收收神通吧 求求了。 
> 好几周 sub2api 没升级了，突然发现所有用户都一起在请求。本来就是我自用的 用户全是我硬塞给大佬们的。都不屑来调我的。 
> 然后发现全是一个 ip在调用，坏菜了。 
> 我太菜了 我也收集不到什么信息 fofa 查了一个这个 ip。肯定是站内大佬了 ![melting_face](https://linux.do/assets/mirrored/9e/9e93fb8c3bb4ac119d8c84cb34d4024b41c1a12dc76b847b91a1f04a328705d9.png) 
>  [[image]](https://cdn3.ldstatic.com/original/4X/6/7/9/679339e386198f0cb34a156ebd37fb8c90e630c5.png) 
> 更新 这几个 ip…

[#p-22334881-ip-1](#p-22334881-ip-1)那么这个ip的强关联方是谁呢

![](https://linux.do/assets/mirrored/be/bed29452f22066ece7e974e97499cfd9a998858d1ac27866006fa78f430e59ee.png)[[update]用事实证据还慕鸢【君の守望】公益站一个清白，关于 107.173.42[.]94 我所观察到的一切](https://linux.do/t/topic/2461746/1)

> 以下内容无任何臆测，数据均来自第三方网络平台。
> 107.173.42.94 到底是谁在使用？
> 严谨调查，事实说话，首先常规操作起手：
> 
> 
> 来自微步的 SSL 证书
> [![截屏2026-06-24 00.00.07](https://linux.do/assets/mirrored/16/16eeec6b9e76c2628c7a4e8c91f5c60c1b2b193eaa7cafa1785feea7ed4c19a3.png)截屏2026-06-24 00.00.072484×1340 300 KB](https://cdn3.ldstatic.com/original/4X/0/1/0/010b4e285b1ce82cff055d333566731377686a47.png)
> 
> 
> 来自 Quake 的 SSL 证书
> [![截屏2026-06-24 00.02.01](https://linux.do/assets/mirrored/cc/cc7f4ccd66d0ce37b0d7861639623824015768eda96a8c5750358c82bb3da667.jpeg)截屏2026-06-24 00.02.011920×835 155 KB](https://cdn3.ldstatic.com/original/4X/f/0/5/f054ca51f44cac747892e75397980bd77d4ee4e4.jpeg)
> 
> 
> 现在所有证据都指向 744000[.]xyz，那么问题来了
> 这个域名又是谁在使用？
> 接下来我们打开万能的 Google 搜索引擎：
> [![截屏2026-06-24 00.03.44](https://linux.do/assets/mirrored/10/10f06b9e10dafc0f5cf7e994fc55fd799be634a349e570be6289d9bd346d9a18.jpeg)截屏2026-06-24 00.03.441920×1296 183 KB](https://cdn3.ldstatic.com/original/4X/a/6/1/a61e6c5116b235dc62c489f82db548d28d73f975.jpeg)
> 让我们打开 Threads 看看这条推在说什么：
> 
> 《AI 世界中的 “索马里之旅” 第一篇》
> 这个名为 “China VSLLM” 的 AI 盗版组织也接受条纹码（Stripe）支付方式……
> 
> 感觉他们就像霍尔木兹海峡革命卫队一样 —— 同样接受信用卡支付啊……
> 
> [![截屏2026-06-24 00.08.48](https://linux.do/assets/mirrored/8a/8abc8fd1b25b1bbb3f0e291c1b3da34d387a9abad1c458f76698b4ecd1a6bb21.jpeg)截屏2026-06-24 00.08.481252×2192 223 KB](https://cdn3.ldstatic.com/original/4X/0/9/3/093bd6c0ba2f9afe47c0a2bb64d27dbfa34e0c88.jpeg)
> 那么我们的 744000[.]xyz 又是在哪里出现的呢？
> [![截屏2026-06-24 00.09.53](https://linux.do/assets/mirrored/a2/a2a067c6d0fdc62ce6a7c0a5c191dcacea8b56e2260d766c747fa129ecaa948f.jpeg)截屏2026-06-24 00.09.531246×1062 346 KB](https://cdn3.ldstatic.com/original/4X/a/4/0/a4090325f63bbce1ff59b21f4aa5344b225a5ab1.jpeg)
> Proxy 接口被 Cloudflare 拦截跳 5 秒盾暴露了 Proxy 后端地址 ![:laughing:](https://linux.do/assets/mirrored/0d/0d46390df7858374bd26a539915193d11a6bfb5fef11ff8e7572a1d32851b126.png)
> 附上一个子站点
> [https://console.744000.xyz](https://console.744000.xyz/)
> [![截屏2026-06-24 00.42.49](https://linux.do/assets/mirrored/a0/a0a0b68907a98d3fdb167282685a7390c46c1463fefcd0a9afe86441b66a45a6.png)截屏2026-06-24 00.42.492724×1718 401 KB](https://cdn3.ldstatic.com/original/4X/a/0/1/a0153cb43c66eb3b1772a364d3cc5397ff628683.png)

[https://console.744000.xyz/](https://console.744000.xyz/) 指向 [https://linux.do/u/yeahhe](https://linux.do/u/yeahhe)

[![image](https://linux.do/assets/mirrored/d7/d774d4ffc6993344ea6118391ced6b7ead746d3f182355ad51f53595d0d8b885.png)image1956×1078 188 KB](https://cdn3.ldstatic.com/original/4X/6/e/1/6e14a96924dadbd85e1237ec9095113bf3812b2a.png)

部署的开源项目是一个前端 demo，只有 UI 没有实际的功能，这套 demo 没有开源并且不可能有第二个人会在自己的 demo 里面写别人的邮箱和 ID，拿帖子里截图的邮箱搜索出来的是开源项目，给哥们吓得把 demo 都关了

还是那句话，都是国人，别打自己人的野！薅薅openai的羊毛就得了

![](https://linux.do/assets/mirrored/04/04faa363bfffb14b547443203596867f456c71f4ebd0caeaa1124280e3a016e9.png)[【小结】不明来路的 key 大家就不要再薅了](https://linux.do/t/topic/2768044/1)

> 都是国人开发者，这都是干的啥事啊。。。

## #2 摇摆熊 (@Jojo_Coco)

Created: 2026-09-04T01:54:34.457Z
Updated: 2026-09-04T01:54:34.457Z

代理池也不用，就楞打是吗，还有这么直接的？

## #3 人间第一流 (@diyiliu)

Created: 2026-09-04T01:54:41.220Z
Updated: 2026-09-04T01:54:41.220Z

又有瓜吃啦？ 标记一下帖子  准备看后续

## #4 Ken (@Ken)

Created: 2026-09-04T01:55:30.471Z
Updated: 2026-09-04T01:55:30.471Z

前排吃瓜。不用代理直接来这样倒是好溯源了

## #5 rookiepy (@rookiepy)

Created: 2026-09-04T01:55:38.218Z
Updated: 2026-09-04T01:55:38.218Z

群众里面有坏人啊.jpg

流放吧

## #6 藕粉 (@OFlare)

Created: 2026-09-04T01:55:41.411Z
Updated: 2026-09-04T01:55:41.411Z

我站内搜到这个人了，貌似很多开源，高产？

## #7 Kevin9010 (@kevin9)

Created: 2026-09-04T01:57:26.547Z
Updated: 2026-09-04T01:57:26.547Z

这个分析得还是很透彻，一环一环的，这不比破案电视剧强？

## #8 Mirae (@Mirae)

Created: 2026-09-04T01:57:56.619Z
Updated: 2026-09-04T01:57:56.619Z

单纯好奇，@example.com 真的存在么？不是说是保留域名么

## #9 luwei (@luwei11)

Created: 2026-09-04T01:58:02.868Z
Updated: 2026-09-04T01:58:02.868Z

卧槽 还能这么破案 学到了，很宝贵的经验

## #10 SevenZxi (@SevenZxi)

Created: 2026-09-04T01:58:15.916Z
Updated: 2026-09-04T01:58:15.916Z

吃瓜吃瓜，能@出来站内这个人吗？

## #11 cata (@mengbao03)

Created: 2026-09-04T01:58:46.741Z
Updated: 2026-09-04T01:58:46.741Z

前排吃瓜，打野被抓到哇，也是站内的吗？

## #12 Theo (@jmklkj)

Created: 2026-09-04T01:58:59.382Z
Updated: 2026-09-04T01:58:59.382Z

前排出售瓜子饮料矿泉水，坐等当事人出现

## #13 小小 (@lp0826)

Created: 2026-09-04T01:59:07.737Z
Updated: 2026-09-04T01:59:07.737Z

我标记了一处地点 ![:grinning_face:](https://linux.do/assets/mirrored/9c/9cfc5ad34e89b6eebddcd5ec715c224a86c99ea5b9fad999407dee7e32f681b6.png)，然后，救救我，救救我 ![:grinning_face:](https://linux.do/assets/mirrored/9c/9cfc5ad34e89b6eebddcd5ec715c224a86c99ea5b9fad999407dee7e32f681b6.png)

## #14 Efar (@efarxs)

Created: 2026-09-04T01:59:42.872Z
Updated: 2026-09-04T02:07:58.483Z

（帖子已被作者删除）

## #15 浴皇大帝 (@ty12)

Created: 2026-09-04T01:59:45.068Z
Updated: 2026-09-04T02:00:01.100Z

吃瓜吃瓜，经典“中国人不搞中国人” ![:joy:](https://linux.do/assets/mirrored/c2/c252a58367211c11d839155e50dc5e98551826c64b8d2e8d6267124c054ceae0.png)（不搞才怪）

[![5f7c754a242e2e30da4b05139e1a135d](https://linux.do/assets/mirrored/dd/dd0e8c07ae6e6eecdfcaf02571ebdea370e38702245449c06f53e825fe6e5efe.jpeg)5f7c754a242e2e30da4b05139e1a135d828×865 121 KB](https://cdn3.ldstatic.com/original/4X/f/4/8/f48380415ca9ab786f0dfff9ef10d6d850dbf533.jpeg)

## #16 superjack (@superjack)

Created: 2026-09-04T01:59:46.809Z
Updated: 2026-09-04T02:00:14.242Z

涨知识了，确实赞同这个，A/O÷ 是因为是÷ 所以才薅的心安理得，国人还是手下留情吧

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 还是那句话，都是国人，别打自己人的野！薅薅 openai 的羊毛就得了

## #17 晨旭 (@chenxu)

Created: 2026-09-04T01:59:51.545Z
Updated: 2026-09-04T02:58:44.439Z

这应该只是巧合吧，这个id我看重名的挺多啊

邮箱后缀是@example.com，看起来就是随便瞎写的

744000.xyz这个域名，有个子域名指向了edgeone，老外用的概率太低了

[![图片](https://linux.do/assets/mirrored/e6/e664cc91a9648501d087dc511ab22c81208abf31ce29db4b209a65942448f60b.png)图片767×393 34.8 KB](https://cdn3.ldstatic.com/original/4X/a/7/0/a702a3ab42ec5e4e5aba72dd9f94ad55460fb9d7.png)

## #18 onlysuperman (@onlysuperman)

Created: 2026-09-04T02:01:21.640Z
Updated: 2026-09-04T02:01:21.640Z

话说站内有重名的情况吗？？如果要单方面封禁的话会不会封错人了？？ ![:poop:](https://linux.do/assets/mirrored/91/91f689597621d1bed4653fb69281128d46ac44cca08248e4cef1ef7f9a46b724.png)

## #19 hhnnjjcc (@hhnnjjcc)

Created: 2026-09-04T02:01:28.549Z
Updated: 2026-09-04T02:01:28.549Z

我觉得L站应该彻底杜绝打野的行为。这和偷有什么区别。

这种行为你自己偷着用也就算了，不值得提倡

## #20 是水吉啊 (@linuxhe)

Created: 2026-09-04T02:01:36.176Z
Updated: 2026-09-04T02:01:36.176Z
Reply to: #17 晨旭

能这么严谨的调查，中期跟踪后，这么长时间才发出来，你觉得会是巧合？

## #21 Mx (@Mxucc)

Created: 2026-09-04T02:01:37.264Z
Updated: 2026-09-04T02:01:37.264Z

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 给哥们吓得把 demo 都关了

当事人已经上线了，看看后续怎么说

## #22 james (@jamesfu)

Created: 2026-09-04T02:01:59.666Z
Updated: 2026-09-04T02:01:59.666Z

没点实力都不好查啊，还是厉害啊！！

## #23 cxmplex (@Sen_C)

Created: 2026-09-04T02:02:15.090Z
Updated: 2026-09-04T02:02:15.090Z
Reply to: #17 晨旭

这个人资料里挂着的git就是慕鸢佬图中的git啊

## #24 MartinMa (@MartinMa)

Created: 2026-09-04T02:02:17.438Z
Updated: 2026-09-04T02:02:17.438Z

佬太牛了，已经严肃学习破案思路。

## #25 苏夜白 (@suyebai)

Created: 2026-09-04T02:02:24.166Z
Updated: 2026-09-04T02:02:24.166Z

自己部署的CPA，会被人盗刷吗？如何防止这个情况。

## #26 白龙 (@showfor)

Created: 2026-09-04T02:02:30.085Z
Updated: 2026-09-04T02:02:30.085Z

前排来的 这个追踪能力好强 学到了![:smiling_face:](https://linux.do/assets/mirrored/6b/6ba62723e34df401cdd78478b350203278f197b7f54aae7efe77a59731a5ce23.png)

## #27 Tbot (@Tbot)

Created: 2026-09-04T02:02:55.061Z
Updated: 2026-09-04T02:02:55.061Z

WTF？？本来这个用户名不认识，但是点进主页发现是墨子？

## #28 fatcarter (@fatcarter)

Created: 2026-09-04T02:03:05.487Z
Updated: 2026-09-04T02:03:05.487Z

流放岭南！！！

[![image](https://linux.do/assets/mirrored/94/94c556e9a4d5e50afe60faef9113d6f47782f4bfefffd782dd1caea515903c79.jpeg)image248×293 17 KB](https://linux.do/assets/mirrored/94/94c556e9a4d5e50afe60faef9113d6f47782f4bfefffd782dd1caea515903c79.jpeg)

## #29 Crixs (@Crixs)

Created: 2026-09-04T02:03:23.623Z
Updated: 2026-09-04T02:03:23.623Z

[@yeahhe](https://linux.do/u/yeahhe) 大召唤术，这位也是熟人

## #30 marre (@marre)

Created: 2026-09-04T02:03:42.593Z
Updated: 2026-09-04T02:03:42.593Z

牛皮，赶上热乎的了，我喜欢福尔摩斯环节

## #31 柏川 (@b3b41020)

Created: 2026-09-04T02:04:15.665Z
Updated: 2026-09-04T02:04:15.665Z

破案神速，严肃学习！打站内的人也太坏了！！！我觉得有必要请@neo 来判决下了

## #32 RerrentLinden (@RerrentLinden)

Created: 2026-09-04T02:04:21.048Z
Updated: 2026-09-04T02:04:21.048Z

又到了周五摸鱼最喜欢的名侦探柯南环节 ![:bili_038:](https://linux.do/assets/mirrored/41/41ebf0b3357f5e93c7509ddc3998e518c8ca9aaf69e3674924f4d1e5d46429e2.png)

## #33 luwei (@luwei11)

Created: 2026-09-04T02:04:28.616Z
Updated: 2026-09-04T02:04:28.616Z

[@neo](https://linux.do/u/neo)  来吃瓜了 始皇，新鲜的

## #34 bi-o-xu (@bi-o-xu)

Created: 2026-09-04T02:04:40.245Z
Updated: 2026-09-04T02:04:40.245Z

又到了我最喜欢的对线环节,吃瓜看戏

## #35 三月七 (@March7th)

Created: 2026-09-04T02:04:47.697Z
Updated: 2026-09-04T02:04:47.697Z

这个我记得上次就已经查出来了，只不过没直说，所以没几个人知道

## #36 samuel_wyj (@samuel_wyj)

Created: 2026-09-04T02:04:57.919Z
Updated: 2026-09-04T02:04:57.919Z

吃瓜吃瓜，周五吃瓜日。这位佬不出来对线吗？

## #37 Theo (@jmklkj)

Created: 2026-09-04T02:05:34.645Z
Updated: 2026-09-04T02:05:34.645Z
Reply to: #36 samuel_wyj

当事人三分钟前已经回复过帖子了，估计在来的路上，如果不来估计直接摆了。。

## #38 木木 (@littlemumu)

Created: 2026-09-04T02:06:15.468Z
Updated: 2026-09-04T02:06:15.468Z

感觉这个网址见到好多次捏。与人斗 其乐无穷 ![:laughing:](https://linux.do/assets/mirrored/0d/0d46390df7858374bd26a539915193d11a6bfb5fef11ff8e7572a1d32851b126.png)

## #39 well (@well)

Created: 2026-09-04T02:06:20.616Z
Updated: 2026-09-04T02:06:30.954Z

正好周五不想上班,这下又有瓜吃了.等一个后续 ![:grin:](https://linux.do/assets/mirrored/ed/ed2d1ae8dcdaf6a12e9af7d7bced25db2c3e8f38e624f930d13ff697e3285e7b.png)

## #40 彭于晏 (@hongxb)

Created: 2026-09-04T02:06:52.057Z
Updated: 2026-09-04T02:06:52.057Z

这哥们也是执着，同一个ip反复调用这么多次。

## #41 Yu001 (@Yu001)

Created: 2026-09-04T02:07:31.889Z
Updated: 2026-09-04T02:07:31.889Z
Reply to: #10 SevenZxi

不用@啊，帖子里面指向那个链接就是

## #42 云书 (@2233flyme)

Created: 2026-09-04T02:09:44.160Z
Updated: 2026-09-04T02:09:44.160Z

神了还有这种事情的啊 牛逼牛逼  !

## #43 太想进步啦 (@txjbl)

Created: 2026-09-04T02:10:36.945Z
Updated: 2026-09-04T02:10:36.945Z

前排吃瓜，不愧是大佬啊，抽丝剥茧，层层递进，实在是厉害厉害

## #44 xiaoddiao (@xiaoddiao)

Created: 2026-09-04T02:11:07.657Z
Updated: 2026-09-04T02:11:07.657Z

之前有一个大佬就扒出来是他了，等当事人自己出来澄清吧

## #45 JokerChan (@JokerChan)

Created: 2026-09-04T02:12:09.498Z
Updated: 2026-09-04T02:12:09.498Z

![image](https://linux.do/assets/mirrored/4a/4aff9e47a52b5e5c170ff7f7e3f9fe72ac717740234f591b7462870f007cd5a8.png)

开始对线

## #46 xiaoyan  (@xiaoyan)

Created: 2026-09-04T02:12:16.046Z
Updated: 2026-09-04T02:12:35.733Z

后排吃瓜，这个当事人看着也是挺眼熟啊

![image](https://linux.do/assets/mirrored/44/44038eebf5250611dd3e37770aed1bf8c2fb173120e716bcb44d0ac059c86cd1.png)也在打字了

## #47 甘尼克斯 (@KIVINXU)

Created: 2026-09-04T02:12:21.617Z
Updated: 2026-09-04T02:12:21.617Z

吃瓜吃瓜，先给盗刷怪加个标签再说

## #48 Mozi (@yeahhe)

Created: 2026-09-04T02:12:26.324Z
Updated: 2026-09-04T02:14:44.768Z
Reply to: #29 Crixs

[![PixPin_2026-09-04_10-14-37](https://linux.do/assets/mirrored/78/788d45f56dcd42ce94fd543a1351bdb76b76fd8acaaa151e7e29db4073d6bc01.png)PixPin_2026-09-04_10-14-371357×1261 91.2 KB](https://cdn3.ldstatic.com/original/4X/8/6/4/864fe42fcd6e9aaf4a23229cdf24bdd02856bdce.png)

我只有这一个服务器，这个IP不匹配

而且现在也在用

## #49 想无msn (@lzz0836)

Created: 2026-09-04T02:13:31.232Z
Updated: 2026-09-04T02:13:31.232Z

cpa怎么不安全吗？直接就被盗token了，害怕

## #50 wxpLeo (@wxpLeo)

Created: 2026-09-04T02:14:13.086Z
Updated: 2026-09-04T02:14:13.086Z

来了来了 大要来 前排开始吃瓜 ![:star_struck:](https://linux.do/assets/mirrored/49/494a5d33fa83756c26384a2e7a90142bde9d8d0b4f81c7f2721b9527cf5ce684.png)

## #51 某人 (@abao)

Created: 2026-09-04T02:15:07.325Z
Updated: 2026-09-04T02:15:07.325Z

吃瓜吃瓜，好久没吃到富.kd.g以外的瓜了，观望一下看看情况。

## #52 ak7876 (@ak7876)

Created: 2026-09-04T02:15:31.814Z
Updated: 2026-09-04T02:15:31.814Z
Reply to: #49 想无msn

看前面好像是环境变量填错了，导致设置密码没有生效，相当于没设密码。知道ip就可以用

## #53 dayangda163 (@dayangda163)

Created: 2026-09-04T02:16:12.951Z
Updated: 2026-09-04T02:16:12.951Z

发生了什么事，安静的吃瓜看戏， ![:rofl:](https://linux.do/assets/mirrored/4a/4a371ef1123fee52185f3098d3d3b65dc7f695fdd574ea977ea2afedff963ad5.png)

## #54 Mozi (@yeahhe)

Created: 2026-09-04T02:16:48.728Z
Updated: 2026-09-04T02:16:48.728Z
Reply to: #48 Mozi

说实话，我现在都没怎么看懂，我是真一点都不知道这种事情

我要怎么才可以证明自己呢

## #55 xiaoddiao (@xiaoddiao)

Created: 2026-09-04T02:17:16.144Z
Updated: 2026-09-04T02:17:16.144Z

反正可以确定当事人是肯定在L站的，是不是这位佬就不知道了。无论怎么说这个人是各种意义上的坏透了，金额也是巨大，就是不好溯源，除非有服务商的配合

## #56 叮咚 (@honest)

Created: 2026-09-04T02:17:43.581Z
Updated: 2026-09-04T02:17:43.581Z
Reply to: #48 Mozi

demo有你的ID邮箱啊，别人怎么会用你的邮箱（在连代理池都不用 显然是没有刻意防备伪装的前提下）？

## #57 野王996 (@BraveCalf)

Created: 2026-09-04T02:19:48.321Z
Updated: 2026-09-04T02:19:48.321Z
Reply to: #56 叮咚

唉，不能强制收手的前提下，“凶手”对线完，又成熟了，下次作案手法又高明了

## #58 darkhandz (@darkhandz)

Created: 2026-09-04T02:19:59.119Z
Updated: 2026-09-04T02:19:59.119Z

吃瓜的，看看双方辩手怎么说的，有没有第三方

## #59 laikey.lau (@laikey.lau)

Created: 2026-09-04T02:20:54.008Z
Updated: 2026-09-04T02:20:54.008Z

这什么情况？这是什么瓜？要好好对线才行啊

## #60 undefined (@tuan2046)

Created: 2026-09-04T02:21:03.665Z
Updated: 2026-09-04T02:21:03.665Z

![:bili_040:](https://linux.do/assets/mirrored/58/58a161463a67ba070bf5bdaf761f6dc19395980fa13f0dbb8ab29f8b0b026eee.png)

各大公益站联合查一下嘛，

看看这ip是否有对应的账号

然后汇总起来就大概能定位了。

## #61 pluto233 (@pluto233)

Created: 2026-09-04T02:21:38.102Z
Updated: 2026-09-04T02:21:38.102Z

ww 好久没吃到瓜了喵~(呆

另一位也是很眼熟的佬呢(呆

## #62 小呆太帅 (@xiaodaitaishuai)

Created: 2026-09-04T02:23:03.280Z
Updated: 2026-09-04T02:23:03.280Z

反复观看,学习技术 ,佬太牛了.

## #63 coho (@coho)

Created: 2026-09-04T02:24:24.757Z
Updated: 2026-09-04T02:24:24.757Z

不是我，我再吃瓜，礼貌问一下，怎么弄tokens啊 ![:joy:](https://linux.do/assets/mirrored/c2/c252a58367211c11d839155e50dc5e98551826c64b8d2e8d6267124c054ceae0.png)

## #64 MartinMa (@MartinMa)

Created: 2026-09-04T02:26:22.476Z
Updated: 2026-09-04T02:26:22.476Z

我想到一个辩解思路，因为是yeahhe@example.com，这个明显是所有叫yeahhe的人都有可能会用的。demo中那个yeahhe@example.com 有没有可能是另一个叫yeahhe的人呢？然后碰巧也是中国人，也用linuxdo，正好也用yeahhe@example.com 这个邮箱做演示，我觉得有点扯吧。 ![:rofl:](https://linux.do/assets/mirrored/4a/4a371ef1123fee52185f3098d3d3b65dc7f695fdd574ea977ea2afedff963ad5.png)

## #65 iostream (@iostream)

Created: 2026-09-04T02:26:25.405Z
Updated: 2026-09-04T02:26:25.405Z

感觉自证好苍白无力，找neo看一下这个佬的登录ip历史有没有这个嫌疑ip不知道是否可以 ![:melting_face:](https://linux.do/assets/mirrored/9e/9e93fb8c3bb4ac119d8c84cb34d4024b41c1a12dc76b847b91a1f04a328705d9.png)

## #66 wohaokunr (@hk_w)

Created: 2026-09-04T02:29:28.870Z
Updated: 2026-09-04T02:29:28.870Z
Reply to: #65 iostream

[@neo](https://linux.do/u/neo) 先@出来试试，说不定真的来了

## #67 Mozi (@yeahhe)

Created: 2026-09-04T02:31:45.508Z
Updated: 2026-09-04T02:32:59.457Z
Reply to: #66 wohaokunr

我自己找他吧，反正我有什么信息提供什么信息，我评论的话越描越黑了

## #68 Simplef (@Simplef)

Created: 2026-09-04T02:32:00.891Z
Updated: 2026-09-04T02:32:00.891Z

话说有没有打野教学，想学习技术（手动狗头）

## #69 拼多多 (@pinduoduo)

Created: 2026-09-04T02:32:35.775Z
Updated: 2026-09-04T02:32:35.775Z
Reply to: #64 MartinMa

你仔细看看图里面还有个论坛帖子的地址，再看看发帖人是谁

## #70 Theo (@jmklkj)

Created: 2026-09-04T02:32:51.296Z
Updated: 2026-09-04T02:32:51.296Z
Reply to: #64 MartinMa

[![image](https://linux.do/assets/mirrored/3d/3da9d4150f8241a80a6daf5d352ff2953c28a8f780fa116be70c775f049b016f.png)image909×262 10.8 KB](https://linux.do/assets/mirrored/3d/3da9d4150f8241a80a6daf5d352ff2953c28a8f780fa116be70c775f049b016f.png)

巧合太多了，电影都不敢这么拍

## #71 key1 (@key5230)

Created: 2026-09-04T02:33:13.874Z
Updated: 2026-09-04T02:33:13.874Z

这就是道德问题，你只能自己气氛没啥办法，服务器也最多去举报，对当事人一点风险都没有

## #72 L (@Lilis)

Created: 2026-09-04T02:34:08.370Z
Updated: 2026-09-04T02:35:14.864Z
Reply to: #64 MartinMa

没办法，也只能一个用户名重复了。坏人之前不是栽赃慕鸢吗？也有可能是故意陷害栽赃给这个佬的，不过这位佬真是洗不清了。

## #73 ZackWill (@ZackWill)

Created: 2026-09-04T02:34:14.346Z
Updated: 2026-09-04T02:44:06.796Z

一个猜想，既然攻击者能给80端口重定向到muyuan，那他也完全可以重定向到站内任意一个佬公开的页面来栽赃吧![:thinking:](https://linux.do/assets/mirrored/51/5116f7d07677f06785887c0af23c189b541a306d6b792d605ffaf3ed9f0e912d.png)

[@iostream](https://linux.do/u/iostream) 哪里的信息有说console这个不是重定向的

## #74 MartinMa (@MartinMa)

Created: 2026-09-04T02:34:19.650Z
Updated: 2026-09-04T02:34:19.650Z
Reply to: #70 Theo

我也觉得，但是证据链上其他的部分实在是太硬了，哈哈哈，无法想象他将如何对线。

## #75 undefined (@tuan2046)

Created: 2026-09-04T02:34:55.138Z
Updated: 2026-09-04T02:34:55.138Z

要不谁指定下始皇 ![:bili_040:](https://linux.do/assets/mirrored/58/58a161463a67ba070bf5bdaf761f6dc19395980fa13f0dbb8ab29f8b0b026eee.png)

始皇来大数据来一波。

## #76 kkniu (@Kiko1)

Created: 2026-09-04T02:35:16.080Z
Updated: 2026-09-04T02:35:16.080Z

好喜欢这种东窗事发、深入摸查、意外转折、群雄涿鹿、蛛丝马迹、柳暗花明、拨云见日的剧情。

## #77 SevenZxi (@SevenZxi)

Created: 2026-09-04T02:36:01.436Z
Updated: 2026-09-04T02:36:01.436Z
Reply to: #70 Theo

这个就已经算是铁证了，怎么都无法狡辩的

## #78 wangzhen3691 (@wangzhen3691)

Created: 2026-09-04T02:36:08.581Z
Updated: 2026-09-04T02:36:08.581Z
Reply to: #73 ZackWill

别的佬不好栽赃，因为最帅的佬是搞安全的 ![:laughing:](https://linux.do/assets/mirrored/0d/0d46390df7858374bd26a539915193d11a6bfb5fef11ff8e7572a1d32851b126.png)

为了自证清白，微步溯源走了一圈

## #79 我思故我在 (@fengtang)

Created: 2026-09-04T02:37:26.615Z
Updated: 2026-09-04T02:37:26.615Z

代理池都不用吗，直接一个IP一直用啊。

## #80 陌流川 (@cavalry)

Created: 2026-09-04T02:37:38.444Z
Updated: 2026-09-04T02:37:38.444Z

刺激，有种破案的感觉了，没想到自己用的CPA还能被盗刷，太坏了

## #81 superuser (@superuser)

Created: 2026-09-04T02:38:12.692Z
Updated: 2026-09-04T02:38:27.606Z

（帖子已被作者删除）

## #82 tt (@dlouxgit)

Created: 2026-09-04T02:38:20.437Z
Updated: 2026-09-04T02:38:20.437Z

可以再隐藏或者模糊一下追溯流程吗，防止后面有人升级了这个手段让人查不出来。

因为我也被盗刷了很多，而且是 api 形式的真金白银，痛恨这群盗刷者。太恶心了。

## #83 coior (@maxsea)

Created: 2026-09-04T02:38:52.343Z
Updated: 2026-09-04T02:38:52.343Z

此处吃瓜. 其乐无穷.

期待后续情况回复

## #84 superuser (@superuser)

Created: 2026-09-04T02:39:07.042Z
Updated: 2026-09-04T02:46:32.474Z

完蛋捏。对不起了各位。貌似刨析错了，那个当事人不是目标 ![:smiling_face_with_tear:](https://linux.do/assets/mirrored/ad/ad1dcb074a55b2b3bacd1744db2a851d6ca83decb7e232e3fcb08e5c3e37357b.png)

## #85 moml (@moml)

Created: 2026-09-04T02:40:24.415Z
Updated: 2026-09-04T02:40:24.415Z

看到IP前缀心里还咯噔了一下，觉得有点眼熟，看了一下我的RN服务器，还真有一个107.173开头的，还好后面两个不对 ![:rofl:](https://linux.do/assets/mirrored/4a/4a371ef1123fee52185f3098d3d3b65dc7f695fdd574ea977ea2afedff963ad5.png)

## #86 xiewuzhiying (@xiewuzhiying)

Created: 2026-09-04T02:41:17.833Z
Updated: 2026-09-04T02:41:17.833Z
Reply to: #84 superuser

反正这家伙就是找两个论坛里眼熟的佬泼脏水。

## #87 code (@NEXT0)

Created: 2026-09-04T02:41:33.081Z
Updated: 2026-09-04T02:41:33.081Z
Reply to: #70 Theo

看着巧合的就是一个id吧，example.com这个域名后缀好像很多应用默认都是这个 ![:tieba_087:](https://linux.do/assets/mirrored/b5/b5053bbded7f95078a12bc73c8f2c462abb6d0e3e31e2b8ca95136ca9b5a2d66.png)

## #88 RyanVan (@RyanVan)

Created: 2026-09-04T02:42:05.874Z
Updated: 2026-09-04T03:02:37.833Z

看完了目前只能想到3种解释。

demo 站点是当事人的仓库，攻击者部署demo时沿用了这个邮箱。
攻击者恶意陷害当事人。
攻击者碰巧跟当事人同名。

目前看起来栽赃还是有可能的，[[update]用事实证据还慕鸢【君の守望】公益站一个清白，关于 107.173.42[.]94 我所观察到的一切](https://linux.do/t/topic/2461746) 这个帖子几个月前就公布了这个域名，攻击者完全有时间栽赃。既然能栽赃楼主，栽赃当事人也是可能的。

## #89 KSAMNI (@yancj)

Created: 2026-09-04T02:43:03.114Z
Updated: 2026-09-04T02:43:03.114Z

能在L站找到本人的搞笑程度+++++哈哈哈

## #90 undefined (@tuan2046)

Created: 2026-09-04T02:43:11.365Z
Updated: 2026-09-04T02:43:11.365Z

![:bili_040:](https://linux.do/assets/mirrored/58/58a161463a67ba070bf5bdaf761f6dc19395980fa13f0dbb8ab29f8b0b026eee.png)

那要不大家都ddos下 107.173.42.94 试试。

## #91 BoBo (@Bo666)

Created: 2026-09-04T02:43:17.669Z
Updated: 2026-09-04T02:43:17.669Z

得跟最帅的男人学下破案技术了，顺便吃下瓜

群众里总是有这种坏的

## #92 Gaze (@Gazeee)

Created: 2026-09-04T02:43:34.551Z
Updated: 2026-09-04T02:43:34.551Z
Reply to: #84 superuser

我觉得，既然ip可以302转跳栽赃muyuan佬，用户名也是可能栽赃其它佬的，所以我感觉很难算作是石锤证据 ![:thinking:](https://linux.do/assets/mirrored/51/5116f7d07677f06785887c0af23c189b541a306d6b792d605ffaf3ed9f0e912d.png)

## #93 小木公菜奈 (@WuliJonC)

Created: 2026-09-04T02:44:26.088Z
Updated: 2026-09-04T02:46:18.119Z
Reply to: #84 superuser

发帖的那个韩国人不是当事人吧，就是个碰巧无意识发了些线索的路人

那个发thread的韩国人应该是被低价中转吸引过去的，看内容是在吐槽自己买的低价api直接524报错

## #94 Gaze (@Gazeee)

Created: 2026-09-04T02:44:27.445Z
Updated: 2026-09-04T02:44:27.445Z
Reply to: #90 undefined

刚刚lo了一眼，这个ip目前处于全部超时的状态

## #95 Theo (@jmklkj)

Created: 2026-09-04T02:45:27.147Z
Updated: 2026-09-04T02:45:27.147Z
Reply to: #35 三月七

细说上次的瓜。。可以作为补充证据

## #96 RyanVan (@RyanVan)

Created: 2026-09-04T02:47:29.638Z
Updated: 2026-09-04T02:47:29.638Z
Reply to: #84 superuser

Threads 的截图不是证明韩国人是攻击者，而是这个韩国人联系过攻击者

## #97 nick_glod (@nick_y)

Created: 2026-09-04T02:47:29.904Z
Updated: 2026-09-04T02:47:29.904Z

吃瓜，在线吃瓜，居然还是之前的瓜在线，居然不换ip哈哈哈

## #98 清酒半盏 (@sivyer)

Created: 2026-09-04T02:48:20.493Z
Updated: 2026-09-04T02:49:07.440Z

前排吃瓜，不站队，纯吃瓜。

从现有证据来看，我感觉前面都还算挺有理有据的，直到最后通过名字去判断具体是某个人，这个不好评价算不算实锤。

毕竟国人那么多，重名的太多了，我就算一个大众名，经常碰到重名的 ![:rofl:](https://linux.do/assets/mirrored/4a/4a371ef1123fee52185f3098d3d3b65dc7f695fdd574ea977ea2afedff963ad5.png)

## #99 Elon Musk (@sinfor)

Created: 2026-09-04T02:48:43.009Z
Updated: 2026-09-04T02:48:43.009Z

确实是强证据，置信度很高。不过锤不死，看这位怎么回应吧

## #100 𝓵𝓸𝓿𝓮𝓛𝓾 (@usercnmd)

Created: 2026-09-04T02:48:55.221Z
Updated: 2026-09-04T02:48:55.221Z

赶上了赶上了，热乎的瓜，实在查不出来的话就召唤弗洛伊德佬吧 [@Sigmund](https://linux.do/u/sigmund)

## #101 Sunuuc (@Sunuuc)

Created: 2026-09-04T02:49:09.662Z
Updated: 2026-09-04T02:49:09.662Z
Reply to: #84 superuser

可是那个子域名也是中文的网站，没有确切的证据发出来就是打草惊蛇。但我还是希望能抓到真的

## #102 lidonga (@lidonga)

Created: 2026-09-04T02:49:18.726Z
Updated: 2026-09-04T02:49:18.726Z

[![image](https://linux.do/assets/mirrored/e9/e91e3fd2a5d24b70cd310fa761cba6584df83a7912e7af924401cf33badd57c7.png)image1760×600 75.9 KB](https://cdn3.ldstatic.com/original/4X/7/e/2/7e282a761be9de51a623e4a63c059b7193ec8d84.png)

打开一看是token大家用，罪名我来担

## #103 ProYI (@ProYI)

Created: 2026-09-04T02:49:50.079Z
Updated: 2026-09-04T02:49:50.079Z

console.744000.xyz的域名拥有者可以随意转发吧。。。这里有混淆的可能

## #104 GRaN (@GRaN)

Created: 2026-09-04T02:49:51.493Z
Updated: 2026-09-04T02:49:51.493Z

期待后续调查进展，晚点再来看看怎么个事

## #105 tianzl (@tianzl)

Created: 2026-09-04T02:50:04.488Z
Updated: 2026-09-04T02:50:04.488Z

支持大佬！非常感谢做公益的大佬，做公益本就不容易，请大家相互支持！

## #106 Cuber (@Cuber)

Created: 2026-09-04T02:51:19.081Z
Updated: 2026-09-04T02:56:00.282Z

很硬的证据了，但是当事人不承认也没办法，不好说啥，我站楼主的证据，没有这么巧的事。

很多人都说栽赃，刚好就轮到这个人吗。

后缀可以理解，前缀yeahhe就算不复杂也没这么巧刚好撞到一位L站并且刚好是活人并且刚好匹配的上ID叫这个？？？

这能洗吗？ 但凡对不上我都不想站边。 ![:distorted_face:](https://linux.do/assets/mirrored/84/8409bfdb50cdec5b82b1b0bc3c183a371faa3ef54f8e1252b7ce40b26233b0fb.png)

## #107 Enze (@Enze)

Created: 2026-09-04T02:51:25.141Z
Updated: 2026-09-04T02:53:25.897Z

example.com是写代码时经常用的占位，不可能实际拥有，并非“域名邮箱”。yeah是个常用词，yeahhe 和 365 都不算什么很难重复的ID组合。至少目前不能算铁证。

## #108 iostream (@iostream)

Created: 2026-09-04T02:52:21.526Z
Updated: 2026-09-04T02:56:43.007Z
Reply to: #73 ZackWill

很简单，因为muyuan被80重定向栽赃过，重定向还是很明显有301/302的，或者直接curl看源码也行，这个网站现在也进不去了，具体可以找Muyuan佬确认一下这个console是不是重定向的，而且还有就算是重定向为什么帖子一出来网站就关闭了。又想到一个点，要是这个佬是被重定向陷害的，完全可以公开自己的源站来自证，而不是发一个苍白无力的服务器ip的图来证明

## #109 wjy (@wjy)

Created: 2026-09-04T02:52:54.664Z
Updated: 2026-09-04T02:52:54.664Z

怎么排除栽赃陷害，毕竟这个邮箱想填什么就填什么吧？

## #110 coulson96 (@coulson)

Created: 2026-09-04T02:53:17.460Z
Updated: 2026-09-04T02:53:17.460Z
Reply to: #107 Enze

觉得是铁证，是因为，邮箱和 l 站的帖子发帖人一致

## #111 SUN (@YuChenSUN)

Created: 2026-09-04T02:56:35.852Z
Updated: 2026-09-04T02:56:35.852Z

[@neo](https://linux.do/u/neo) 当事人可能在L站，建议始皇调查下

## #112 变鱼 (@B1anYu)

Created: 2026-09-04T02:56:48.943Z
Updated: 2026-09-04T02:56:48.943Z

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> [![截屏2026-06-24 00.42.49](https://linux.do/assets/mirrored/a0/a0a0b68907a98d3fdb167282685a7390c46c1463fefcd0a9afe86441b66a45a6.png)截屏2026-06-24 00.42.492724×1718 401 KB](https://cdn3.ldstatic.com/original/4X/a/0/1/a0153cb43c66eb3b1772a364d3cc5397ff628683.png)

没看懂，这个图片是证据链里最关键的一个，但是原帖似乎没解释这个图的具体来源，是打开这个demo站就是这样？

## #113 传奇睡觉王 (@CQGFW)

Created: 2026-09-04T02:57:45.845Z
Updated: 2026-09-04T02:57:45.845Z

怎么感觉又是一次栽赃，有时候过于巧合就不是巧合

## #114 wjy (@wjy)

Created: 2026-09-04T02:58:18.409Z
Updated: 2026-09-04T02:58:18.409Z
Reply to: #110 coulson96

这个邮箱是不是可以自己随便设置一个

## #115 Theo (@jmklkj)

Created: 2026-09-04T03:00:15.484Z
Updated: 2026-09-04T03:00:15.484Z
Reply to: #114 wjy

![image](https://linux.do/assets/mirrored/fa/faa9e3ba6978d24ddd0bbf9ddb7d25ddc38b04032b6b6548c71d25298ec5d9e2.png)

## #116 布鲁斯·韦恩 (@Bruce.Wayne)

Created: 2026-09-04T03:01:49.188Z
Updated: 2026-09-04T03:01:49.188Z

让子弹飞一会，证据还是有点难锤死

## #117 皮皮快跑！ (@kkjinping)

Created: 2026-09-04T03:02:09.032Z
Updated: 2026-09-04T03:02:09.032Z

感觉像是对方的二次栽赃把，找到一个demo地址故意转过去

## #118 wjy (@wjy)

Created: 2026-09-04T03:02:18.285Z
Updated: 2026-09-04T03:02:18.285Z
Reply to: #115 Theo

如果蓄意栽赃陷害为什么不会写？我只关心有没有这种可能，我不明白为什么楼主会说“没有可能”

## #119 George (@Lobster)

Created: 2026-09-04T03:03:59.399Z
Updated: 2026-09-04T03:03:59.399Z

话说这些人是怎么盗刷的呀？如果key没有公开的情况下 撞出来的吗？有安全大牛能解释一下吗？

## #120 yydxx (@yydxx)

Created: 2026-09-04T03:05:24.107Z
Updated: 2026-09-04T03:05:24.107Z

建议君佬持续深扒，直接捶死，盗刷的数额有点大了

## #121 皮皮快跑！ (@kkjinping)

Created: 2026-09-04T03:05:27.998Z
Updated: 2026-09-04T03:05:27.998Z
Reply to: #119 George

CPA开了公网，有的是默认密钥没改，有的是改错了配置弄成不需要密钥了

## #122 undefined (@tuan2046)

Created: 2026-09-04T03:05:31.118Z
Updated: 2026-09-04T03:05:31.118Z
Reply to: #119 George

有些小白是部署的默认key。。不带改的

之前有人发过，说某个漏洞研究院不断的在扫各大ip端口

而cpa是有特征的

然后就有人根据特征搜，挨个撞库。

## #123 moom (@omoos)

Created: 2026-09-04T03:05:54.358Z
Updated: 2026-09-04T03:05:54.358Z
Reply to: #119 George

看之前的帖子，有的配置文件里面的配置名写错了，导致key没有生效

## #124 George (@Lobster)

Created: 2026-09-04T03:07:01.265Z
Updated: 2026-09-04T03:07:01.265Z
Reply to: #121 皮皮快跑！

那我就放心了，要是能撞出来就太nb来

## #125 princezyj (@princezyj)

Created: 2026-09-04T03:07:52.872Z
Updated: 2026-09-04T03:07:52.872Z
Reply to: #112 变鱼

子域名对应的网站是这个demo，确定就是这个人拥有的这个域名

## #126 Stephan (@Stephan)

Created: 2026-09-04T03:08:21.072Z
Updated: 2026-09-04T03:08:21.072Z

不管是哪个佬干的这种事儿，都是经典的中国人不骗中国人。

管理员能否严肃处理呢？太坏了 ![:tieba_027:](https://linux.do/assets/mirrored/cb/cbf188a8a0af364bd9356ca253bfa6dda4498e31d6d458b8db4729965aa88ed0.png)

另外博主这个事情走法律程序有没有用呢 ![:tieba_006:](https://linux.do/assets/mirrored/fd/fdaba4a439f693f72095be02c04b27fad872be0af6cdab22726fff434c0a8536.png)

## #127 alairack (@alairack)

Created: 2026-09-04T03:08:46.881Z
Updated: 2026-09-04T03:08:46.881Z

柯南都没这么精彩，还能这么溯源的

## #128 Stephan (@Stephan)

Created: 2026-09-04T03:10:33.937Z
Updated: 2026-09-04T03:10:33.937Z

其实我也比较关心有一个佬的deepseek被人黑了 那个事件 。

## #129 ychell (@user1645)

Created: 2026-09-04T03:11:01.991Z
Updated: 2026-09-04T03:11:01.991Z

一大早就有这种瓜吃吗？不过当事人都出现了，还是观望一下发言吧

## #130 麟瑞Sama (@LinRui_Sama)

Created: 2026-09-04T03:13:08.158Z
Updated: 2026-09-04T03:13:08.158Z

我去我去，站内的吗，能@出来看看不

## #131 大耳朵 (@mayonnaise12138)

Created: 2026-09-04T03:14:24.328Z
Updated: 2026-09-04T03:14:24.328Z

锤死盗刷的，能逮一个是一个，狠狠鞭打

## #132 zhangko (@zhangko)

Created: 2026-09-04T03:14:45.727Z
Updated: 2026-09-04T03:14:45.727Z
Reply to: #130 麟瑞Sama

前面帖子那个佬已经出来对线了，你可以往上翻翻，主贴的链接也能定位到这个佬的主页

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> [https://linux.do/u/yeahhe](https://linux.do/u/yeahhe)

## #133 Big Bang (@bangCz)

Created: 2026-09-04T03:15:10.510Z
Updated: 2026-09-04T03:15:10.510Z

吃瓜吃瓜，都是墙内人何苦为难墙内人；蹲个结果

