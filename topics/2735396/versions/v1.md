# 此次风波的时间线以及道歉声明

Source: https://linux.do/t/topic/2735396
Version: v1
Posts: 138
Missing floors: none

## #1 慕鸢 (@user792)

Created: 2026-08-10T11:09:21.802Z
Updated: 2026-08-10T12:23:28.876Z

最开始是这位佬提出了质疑，帖子如下

  
    

    ![](https://linux.do/assets/mirrored/41/418425d7073e369e6193dd27eb083469c6fb6fd5df3d16861eb5b5371aab3161.png)
    
      [奥特曼，你搞砸了一切。（原标题：那个最帅的男人的星辰站，出来解释下呗？）](https://linux.do/t/topic/2710112) [
  

搞七捻三](https://linux.do/c/gossip/11)
    

  

  
> 再次编辑一下帖子，从隔壁hlool佬得到的结果，哪怕是官方sol-high确实也有可能得到48的juice值。当时真的有可能是奥特曼搞砸了一切。 
> 我在这先给muyuan佬道个歉。 
> 当时没等到号池记录和后续监控网站我确实对这个事情越发怀疑，但是目前来看真的没法依靠juice值下定论。我的判断还是太武断了。 
> 
> 
> 
> muyuan佬已经给了处理了。说是之后会持续保持监控juice值。希望能保持下去吧…

帖子是半夜发的，我是第二天上午看到的

然后我的回应如下

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png)[奥特曼，你搞砸了一切。（原标题：那个最帅的男人的星辰站，出来解释下呗？）](https://linux.do/t/topic/2710112/169)

> 我不关心这些，掺没掺可以后面慢慢研究，但是先给各位佬退了，先让大家拿到实惠再说

我最开始以为是某个上游掺假了，我连后台都没看。

我直接发了退款公告，并安排了客服去处理退款和善后工作，然后我开始排查这个事件，我找贴主要了id，查了调用日志发现，这个用户的请求是打在了自己的号池的渠道上，并且是前一天的，但是服务器的磁盘有限，每天24时都自动清理日志，所以就没要找到当时的号池日志。

但是这位佬引用了一个开源项目，说是用这个开源项目检测的

  

      [github.com](https://github.com/chen-006/gpt56_api_detector)
  

  
    
  ![](https://linux.do/assets/mirrored/ca/cac428693db9541fe8a196dd0fb0b35d3e047335295af15ec9056ea3c52a028b.png)

  [GitHub - chen-006/gpt56_api_detector: 用于检测api是否路由真实gpt5.6模型](https://github.com/chen-006/gpt56_api_detector)

    用于检测api是否路由真实gpt5.6模型

  

  
    
    
  

  

我使用这个开源项目检测了一下我的gpt plus号池，具体看这个帖子

  
    

    ![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png)
    
      [给大家看一下号池记录吧，我觉得可以终结这个话题了](https://linux.do/t/topic/2712809) [
  

搞七捻三](https://linux.do/c/gossip/11)
    

  

  
> 从[关于这位佬要的解释](https://linux.do/t/topic/2712260)继续讨论： 
> 今天上午我也自测了一下，给大家看一眼 
> 先看所谓的掺假记录 
>  [[ef8c8bd2d284d1f828340b0243758a9c]](https://cdn3.ldstatic.com/original/4X/b/8/d/b8d6f1ad05d38e31e8602c072cde933d32fb2ee4.png) 
> 记住这个时间 2026-08-06 11:59:00 
> 再看调用日志 
>  [[image]](https://cdn3.ldstatic.com/original/4X/5/a/0/5a07a3d05afc353116db08f6a51629ebdf088e5a.png) 
> 最后看号池日志 
>  [[image]](https://cdn3.ldstatic.com/original/4X/c/8/d/c8dcab6be9097cf39b460397d2b5c49cac42715b.png) 
> [#p-21269466-h-1](#p-21269466-h-1)结束，接着奏乐接着舞
> 给看不懂的佬稍微说明下，之前那个帖子拿着 [GitHub - chen-006/…](https://github.com/chen-006/gpt56_api_detector)

这个检测脚本

如下，我已经证明了这个检测方法是不准确的，自然而然，基于这个方法指控我掺假，就是不对的。

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png)[给大家看一下号池记录吧，我觉得可以终结这个话题了](https://linux.do/t/topic/2712809/1)

> 这个开源项目的监测结果说我掺假，于是我自己监测了一下，第一张图就这个开源项目的监测结果，然后我在星辰后台找到了对应的调用记录，也就是第二张图，最后一张图就是对应调用记录的账号调用记录，可以很直观的看到，这是一个 gpt plus 账号的 gpt-5.6sol 模型调用记录
> 所以，这个开源项目的监测结果是不准确的，如果说他是准的，那就是在说奥特曼掺假。

然后我下达了指令，让客服团队暂停退款，这是一次乌龙事件，君の的星辰没有掺假。

在这个求证是否掺假的期间，客服团队一共给五十三位星辰的用户退款到余额。

部分截图如下

稍微解释一下，这个分组的倍率非常之低，只有0.06-0.08，所以金额看上去确实比较少。

[![image](https://cdn3.ldstatic.com/optimized/4X/2/7/d/27d9a50e10f61584e52e0cf86ab1e5de99abb68a_2_690x368.png)image1657×885 52.9 KB](https://cdn3.ldstatic.com/original/4X/2/7/d/27d9a50e10f61584e52e0cf86ab1e5de99abb68a.png)

关于已经退款到账的余额，我这边的处理方式就是落袋为安，既然已经退给用户了，就不能再要回来了，这一点当时也在群里说了。

需要说明的是：当时tg群这边还在收集整理阶段，qq群那边是直接退款的。

这就导致这53名用户全部都是qq群这边的，tg群那边都没有退款，这是我的失职，后续一定一碗水端平，处理好售后服务，非常抱歉！希望各位佬原谅。

按理说事情到这里就应该结束了，我证明了自己没有掺假，部分用户拿到了余额，皆大欢喜~

但是有tg群的用户表示：我在暂停退款之前提交了申请，为什么也没给退？

客服团队处理售后也是有先后的，售后的主力在qq群那边，tg群的处理的确有些滞后，这确实是我们的问题，我在此道歉并承诺，后续会继续优化tg群的售后服务质量，不让类似的事件再次发生。

但是究其根本，退款是因为掺假，在已经证明掺假的指控不成立的情况下，暂停退款也是ok的。

关于这句话的情绪化表达，言辞确实有些激烈，我在此向各位佬道歉，以后一定注意言辞。

但是有些人开始揪着这句话疯狂攻击公益站，可是，我提过公益吗？

君の星辰 哪个月不送tokens？

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png)[关于这位佬要的解释](https://linux.do/t/topic/2712260/1)

> 我几万 B 的 tokens 都送出去了，我犯得上掺假吗，服了

[![image](https://linux.do/assets/mirrored/ac/ac257a1fc9761dfb79b28f84b54502ffea049ec4c546ba68569074a59c57d522.png)image942×481 53.5 KB](https://cdn3.ldstatic.com/original/4X/d/a/e/dae45cc2b35d9de560d69fbdf0ae725c7ebdf159.png)

[![image](https://linux.do/assets/mirrored/1f/1f10cdb0b47f869c928042418193a6f1ebe087c8d3a1911bbcb9adebb4206b11.png)image994×412 43.9 KB](https://cdn3.ldstatic.com/original/4X/7/7/e/77efcd2669ba3b9cc3a3fc450c5776d992b0be8b.png)

君の星辰 哪个月不送tokens？

为什么一提到送tokens，就开始疯狂抹黑公益站？

为什么就事论事的时候，要“以最高的山”开头？

为什么对事不对人的时候，先聊一大段“君の公益”？

那些揪着这句话不放的，到底是想分析问题解决问题，还是说想借着这次风波，来一次彻底的抹黑？不得而知

最后，也向所有的佬友道个歉，处理舆情不及时，公关能力不到位，导致浪费了各位佬大量的时间和精力，非常抱歉！非常抱歉！非常抱歉！

如果大家在使用[君の星辰](https://ai.centos.hk/)过程中遇到问题，欢迎扫描下方的二维码，加入我们的售后qq群，论坛回复不及时的时候，直接群里反馈就行，会有qq群的管理员协助处理，无论是分组报错/退款/开票/协助分析问题，都有专人跟进。

多说一句。

星辰在早期的时候，售后团队确实出现过售后服务态度差的问题，我当时也是羞愧万分，怎么还有佬友充钱还被怼的，那次事件之后，我对星辰售后团队进行一次彻底的整顿。

现在只要在群里反馈问题的，绝对是超高服务质量，哪怕用户codex不会安装，售后团队这边都是直接todesk远程过去帮忙解决，力求让用户满意。

星辰的售后群只有两条红线，第一不许提公益站，第二不许刷屏

[#p-21428729-openai-1](#p-21428729-openai-1)事后又有别的佬证明，openai官方的确有降智，路由到低端模型的行为，原贴主也进行了声明

![](https://linux.do/assets/mirrored/41/418425d7073e369e6193dd27eb083469c6fb6fd5df3d16861eb5b5371aab3161.png)[奥特曼，你搞砸了一切。（原标题：那个最帅的男人的星辰站，出来解释下呗？）](https://linux.do/t/topic/2710112/1)

> 再次编辑一下帖子，从隔壁 hlool 佬得到的结果，哪怕是官方 sol-high 确实也有可能得到 48 的 juice 值。当时真的有可能是奥特曼搞砸了一切。
> 我在这先给 muyuan 佬道个歉。
> 当时没等到号池记录和后续监控网站我确实对这个事情越发怀疑，但是目前来看真的没法依靠 juice 值下定论。我的判断还是太武断了。

> 打扰大家了，祝大家天天开心呀~

[![image](https://linux.do/assets/mirrored/18/184e72bb806efdca9d835bf33246b024f40c8e8f022ef6190e274c35ba3f7326.png)image311×371 33.6 KB](https://linux.do/assets/mirrored/18/184e72bb806efdca9d835bf33246b024f40c8e8f022ef6190e274c35ba3f7326.png)

## #2 凡 (@MortalKing)

Created: 2026-08-10T11:11:46.109Z
Updated: 2026-08-10T11:11:46.109Z

保持关注，最近的争论挺多的，希望后面能做好服务

## #3 FrankHuy (@FrankHuy)

Created: 2026-08-10T11:12:27.495Z
Updated: 2026-08-10T11:12:27.495Z

保持关注，也希望盈利站公益站都能越来越好，不要糊弄消费者

## #4 YangG (@YangG)

Created: 2026-08-10T11:12:47.943Z
Updated: 2026-08-10T11:12:47.943Z

哥们来来回回横跳，缺失了公信力。

## #5 wjy (@wjy)

Created: 2026-08-10T11:13:54.399Z
Updated: 2026-08-10T11:13:54.399Z

到底是道歉还是美美再吃一波流量，不愧是宣传大师，最帅的男人

## #6 gep (@ElonMusk)

Created: 2026-08-10T11:14:53.340Z
Updated: 2026-08-10T11:21:53.866Z

时间线还是有点问题

是先////

然后我下达了指令，让客服团队暂停退款，这是一次乌龙事件，君の的星辰没有掺假。

在这个求证是否掺假的期间，客服团队一共给五十三位星辰的用户退款到余额。

部分截图如下

稍微解释一下，这个分组的倍率非常之低，只有0.06-0.08，所以金额看上去确实比较少。///

然后///

事后又有别的佬证明，openai官方的确有降智，路由到低端模型的行为，原贴主也进行了声明

我再补充点：帖子发出来后，先在站里说退款，然后过了十几分钟就在Q群里说暂停了原因是自己测得没问题（也没在站里说暂停退款），然后到晚上才辟谣的原贴主道歉

## #7 Shawn_Aaron (@Shawn_Aaron)

Created: 2026-08-10T11:15:05.398Z
Updated: 2026-08-10T11:15:05.398Z

结论不多说，这确实是进站以来见到的持续时间最长，波及最广的话题了 ![:melting_face:](https://linux.do/assets/mirrored/9e/9e93fb8c3bb4ac119d8c84cb34d4024b41c1a12dc76b847b91a1f04a328705d9.png)

## #8 回忆 (@memor221)

Created: 2026-08-10T11:16:03.005Z
Updated: 2026-08-10T11:20:19.178Z

比较好奇 [@Allan](https://linux.do/u/allan) 佬的退款了吗 ![:thinking:](https://linux.do/assets/mirrored/51/5116f7d07677f06785887c0af23c189b541a306d6b792d605ffaf3ed9f0e912d.png) 实际行动比较重要吧

## #9 Hifumi Mizuhara 🍥 (@hifumi_mizuhara)

Created: 2026-08-10T11:16:07.658Z
Updated: 2026-08-10T11:17:26.611Z

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 君の星辰 哪个月不送tokens？
> 为什么一提到送tokens，就开始疯狂抹黑公益站？
> 
> 为什么就事论事的时候，要“以最高的山”开头？
> 
> 为什么对事不对人的时候，先聊一大段“君の公益”？
> 那些揪着这句话不放的，到底是想分析问题解决问题，还是说想借着这次风波，来一次彻底的抹黑？不得而知

道歉就好好道歉吧，为什么一定要说一句这个，前面帖子也分析的很清楚了，确实是有影响

知错能改善莫大焉，但是希望是真的知错了

## #10 Rakuyo  (@Rakuyo)

Created: 2026-08-10T11:16:32.998Z
Updated: 2026-08-10T11:16:32.998Z

我现在就在想一件事：这个事会有始皇下场来 “终结” 吗？还是一直就是双方这样来回发帖。 ![:thinking:](https://linux.do/assets/mirrored/51/5116f7d07677f06785887c0af23c189b541a306d6b792d605ffaf3ed9f0e912d.png)

## #11 sylarQAQ (@sylarQAQ)

Created: 2026-08-10T11:17:01.055Z
Updated: 2026-08-10T11:17:01.055Z

流量大了肯定会有各种问题的，我觉得质疑也合理，拿出证据即可。也及时回应了，挺好的。

## #12 impouo (@impouo)

Created: 2026-08-10T11:17:16.168Z
Updated: 2026-08-10T11:18:20.892Z

不是哥们你能不能不提公益站了，我真受不了。道歉就道歉，中转出问题就出问题，说来龙去脉就说来龙去脉，为啥非要在那说半天公益站啊。。

本来看前面感觉说的也还能接受，道歉也还算诚恳，结果突然又开始一转公益站我真绷不住了

## #13 慕鸢 (@user792)

Created: 2026-08-10T11:17:18.268Z
Updated: 2026-08-10T11:18:02.573Z
Reply to: #9 Hifumi Mizuhara 🍥

这一点不提的话，会一直有人拿这个点带节奏，我没办法

![](https://linux.do/assets/mirrored/79/792ee6aeb8011b7755e4f2691d9ebad007dd5225127af32a653396694f104e7c.png) impouo:

> 不是哥们你能不能不提公益站了，我真受不了。道歉就道歉，中转出问题就出问题，说来龙去脉就说来龙去脉，为啥非要在那说半天公益站啊。。

![](https://linux.do/assets/mirrored/55/55db2b929638408e6af3e755fdb6fdd7a71f00761d504bc0ce44e66eb1c5b1d3.png) Hifumi Mizuhara 🍥:

> 道歉就好好道歉吧，为什么一定要说一句这个，前面帖子也分析的很清楚了，确实是有影响

## #14 J＆G (@JasonGui)

Created: 2026-08-10T11:19:19.728Z
Updated: 2026-08-10T11:19:19.728Z
Reply to: #13 慕鸢

我感觉你不说这个就不会有人说了，你是源头

## #15 Chinamobile (@Chinamobile)

Created: 2026-08-10T11:19:22.384Z
Updated: 2026-08-10T11:19:30.718Z

对不起，我读下来，时间线梳理占60%，送token占20%，整顿团队占10%，那道歉占多少呢？关键点不该是道歉吗 ![:bili_040:](https://linux.do/assets/mirrored/58/58a161463a67ba070bf5bdaf761f6dc19395980fa13f0dbb8ab29f8b0b026eee.png)

## #16 小易易 (@xiaoyiyi)

Created: 2026-08-10T11:19:53.241Z
Updated: 2026-08-10T11:19:53.241Z
Reply to: #13 慕鸢

解决办法：带节奏点举报让社区处理

## #17 欣欣|林可欣 (@StellaFortuna)

Created: 2026-08-10T11:19:59.869Z
Updated: 2026-08-10T11:21:53.866Z
Reply to: #7 Shawn_Aaron

你无可否认，他作为全站第九，就是中转站最高的山(限定放在下一句)

[![Screenshot_20260810_191919](https://linux.do/assets/mirrored/9c/9c438b3fc511214f9cfdba6644f030c06417c0e6cce1fc69eda24413284e2d38.jpeg)Screenshot_20260810_1919191260×2250 296 KB](https://cdn3.ldstatic.com/original/4X/1/a/2/1a20677170f60644c9e0abc847d5ec03a1a039a5.jpeg)

在人气方面无可置疑

影响力巨大

人们喜欢类比 公益站是个很好的类比

把公益这种靠打野和特殊渠道开出来的站的高质量再和中转站的质量去对比，发现中转竟然存在「掺水」 会认为这不如公益 也就是充钱打不过白嫖

关于AI我不想说太多了

谈来谈去都是那些

掺水现象越来越多之后

人们似乎忘了:

[#p-21429024-h-1](#p-21429024-h-1)降智才是主旋律

## #18 ちーのサバアカです (@_chi_chan_desuka)

Created: 2026-08-10T11:20:12.510Z
Updated: 2026-08-10T11:29:19.424Z

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 为什么就事论事的时候，要“以最高的山”开头？

为什么呢 [应该能成为公益站最高的山吧](https://linux.do/t/topic/2590032)

## #19 s T (@s_T)

Created: 2026-08-10T11:20:20.047Z
Updated: 2026-08-10T11:20:20.047Z

不是，洋洋洒洒一大片，没看到对那个佬的事情的处理

## #20 listening (@listening)

Created: 2026-08-10T11:20:34.048Z
Updated: 2026-08-10T11:21:12.847Z
Reply to: #13 慕鸢

道歉的主体是付费站，不应该是你。（本身这次事件就是付费站的服务问题）

把公益站拿出来说不就又陷入了“我做公益这么舍得，会在付费站坑人吗”的逻辑了吗。

## #21 zhx47 (@zhx47)

Created: 2026-08-10T11:20:38.722Z
Updated: 2026-08-10T11:20:38.722Z

你时间线最好是对的

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 星辰的售后群只有两条红线，第一不许提公益站，第二不许刷屏

不过这个终于还是等到了明确的切分，后面如果星辰的反馈还有没有根据，因为公益发表支持态度的，可以点点举报了

## #22 慕鸢 (@user792)

Created: 2026-08-10T11:22:00.314Z
Updated: 2026-08-10T11:22:00.314Z
Reply to: #20 listening

不说要挨骂，说了还要挨骂，我干脆全说清楚吧，免得在出问题

## #23 borisjohny (@borisjohny)

Created: 2026-08-10T11:22:01.062Z
Updated: 2026-08-10T11:24:50.021Z

其实很简单的一件事，当时事情出来没有昨天的记录与数据直接发个贴然后道歉就行了，承诺第一时间退款就退，不然就别说退款第一时间排查下，承诺退款排查之后又说不退这搞人心态，对于自己承诺的了事情就立马去做，而不是事后诸葛亮。本来很简单的一件事如果第一时间就处理，哪用浪费时间开这么多帖子来让大家关注。付费站的用户需要的是售后问题第一时间有客服响应，而不是仅仅靠说自己忙而推卸的，消费者的权益才是最高的山!

## #24 impouo (@impouo)

Created: 2026-08-10T11:22:13.684Z
Updated: 2026-08-10T11:22:13.684Z
Reply to: #13 慕鸢

我说句实话，虽然我不用你的公益站，但是你一直坚持公益这点我还是敬佩的，所以我是不愿意用恶意去揣测你的动机。

但是每次你回复或者提到公益站下面就会刷新各种因为公益站而无脑站你的言论，我不清楚你是如何看待这种情况，但这很明显是不健康也不正常的，公益是公益生意是生意，一码归一码。

况且你不是已经另外开贴说公益站的事了吗？如果你真的不想把公益站掺和进去，最好的办法就是不要提，并且阻止下面有人提。你不提，我不提，谁提说谁，我相信自然没人会说公益站的事了。

## #25 慕鸢 (@user792)

Created: 2026-08-10T11:23:10.828Z
Updated: 2026-08-10T11:23:10.828Z
Reply to: #24 impouo

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png)[在另一个话题中](https://linux.do/t/2537747/1)

> 公益站遇到任何问题我这边都不会有任何技术支持，我很忙。
> 
> 再发私信和开帖，后续公益站一律封号
> 
> 唯一反馈问题的方式是回帖评论

我限制过了，我真没招，他们账号又不在我手里

## #26 重度粉毛厨 (@MatsuzakaSato)

Created: 2026-08-10T11:23:14.659Z
Updated: 2026-08-10T11:23:14.659Z

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 君の星辰 哪个月不送tokens？
> 为什么一提到送tokens，就开始疯狂抹黑公益站？
> 
> 为什么就事论事的时候，要“以最高的山”开头？
> 
> 为什么对事不对人的时候，先聊一大段“君の公益”？

[![Screenshot_2026-08-10-19-22-08-045_com.android.chrome-edit](https://linux.do/assets/mirrored/bb/bb3cb1056ec842bb7c8c36a9fb8d5fff051b5c821b97720b73def7695ecc2e01.jpeg)Screenshot_2026-08-10-19-22-08-045_com.android.chrome-edit1440×2542 432 KB](https://cdn3.ldstatic.com/original/4X/c/d/4/cd4e0d8bb99cdf77efe8a719e946514f81097dac.jpeg)

[![Screenshot_2026-08-10-19-22-29-967_com.android.chrome-edit](https://linux.do/assets/mirrored/50/507d4d6a404fd382ff9f804ea1f2ef3a209c234889cf8274393ee8658c93385e.jpeg)Screenshot_2026-08-10-19-22-29-967_com.android.chrome-edit1440×982 135 KB](https://cdn3.ldstatic.com/original/4X/5/b/0/5b0719a02787ffa27f851022a334567ad3820194.jpeg)

你不能只在跌落神坛的时候劝勉别人不要造神

## #27 gep (@ElonMusk)

Created: 2026-08-10T11:24:01.012Z
Updated: 2026-08-10T11:24:01.012Z
Reply to: #25 慕鸢

你不是premium吗，自己搞个小号搞公益站好了，切割干净点，也省的大家说了

## #28 NeKo fatcat (@NeKo_fatcat)

Created: 2026-08-10T11:24:42.011Z
Updated: 2026-08-10T11:24:42.011Z

无非是大梦一场…但其间若是自在得意，还是要戒骄戒躁啊

## #29 brown Jack (@brownJack)

Created: 2026-08-10T11:25:01.074Z
Updated: 2026-08-10T11:25:01.074Z

那我可不可以理解到这一点：你的公益站和商业中转站完完全全切分开来，任何人不能因为你的公益做的好，而包庇中转的问题，也不能因为你的中转出事，就波及到你的公益或者拿公益说事or当盾牌，对吧

## #30 慕鸢 (@user792)

Created: 2026-08-10T11:25:04.181Z
Updated: 2026-08-10T11:25:04.181Z
Reply to: #26 重度粉毛厨

我什么时候上过神坛阿，我靠，我帽子真是高高的

## #31 Thoth (@Thoth)

Created: 2026-08-10T11:26:16.641Z
Updated: 2026-08-10T11:34:02.531Z

希望早点处理清楚吧 这几天天天吃瓜

## #32 zhx47 (@zhx47)

Created: 2026-08-10T11:26:41.497Z
Updated: 2026-08-10T11:27:03.621Z
Reply to: #30 慕鸢

你可能认为自己没有上神坛，实则在只有公益站的用户眼里不然，能切割开还是切割开，公益和商业搅在一起会很麻烦

这不单单只是你自己的想法，别人的裹挟也很重要

## #33 散装江苏 (@is_hp)

Created: 2026-08-10T11:27:05.411Z
Updated: 2026-08-10T11:27:05.411Z

我的想法：

![](https://linux.do/assets/mirrored/2c/2c1f79f99abaad713c7860786f9aa408326b46b519f77bdf5150f638f640834a.png)[我是真不敢吃公益站的流量阿](https://linux.do/t/topic/2731681/211)

> 这事跟当年LDC被禁用差不多
> 
> 
> 
> ![](https://linux.do/assets/mirrored/04/04faa363bfffb14b547443203596867f456c71f4ebd0caeaa1124280e3a016e9.png)[LDC服务临时下线](https://linux.do/t/topic/1770169/1)
> 
> 它只是社区活跃的积分，不是数字货币，更不是真实货币。但慢慢的还是在供需关系中走偏了，这是大家可以看到的事实
> 
> 
> 是的，公益站不和付费站绑定，自然也没有“引流”一说，但是LDC也是如此啊，不也走偏了吗？
> 
> 这件事不是muyuan一句两句不引流就能解决的

但是还是：

[![image](https://linux.do/assets/mirrored/2a/2a14747fe32cfb6a75a70da6dc53038c84c734eaaab8a7c1761d0ead1884d913.png)image1792×439 51.1 KB](https://cdn3.ldstatic.com/original/4X/c/d/a/cda88e9715bb4b8f054ea1c3991497d712b9e700.png)

[![image](https://linux.do/assets/mirrored/16/16dac4ddfb6a220dec0c4b284b531e138edfa1bde1c9417a0834f9e1db4c02d8.png)image1791×440 46.8 KB](https://cdn3.ldstatic.com/original/4X/5/f/7/5f7ec06f74cff8a79c61655c755d9ab9da97bfe1.png)

[![image](https://linux.do/assets/mirrored/40/40c9714517cdb0baddda57de4f2125cca347653daa6bb9863fe3a6b2c99fac42.png)image1800×418 41.6 KB](https://cdn3.ldstatic.com/original/4X/9/c/8/9c8b965f305daa1fba11579d07891f2043a3d102.png)

[![image](https://linux.do/assets/mirrored/5c/5c860d733391ef747f07126d69ecb3ebd8a2aba65f58c77775f2d7132b88f1ae.png)image1803×422 46.5 KB](https://cdn3.ldstatic.com/original/4X/1/4/9/1492c2f84af8f377b59134246f6e0c88a8916c8e.png)

总得来说，道歉固然是好的，但是你不能否认公益的作用

当然，阴谋论不可取，我们只能说明，公益确实造成了一定的影响（没说好坏），最让我不解的就是上面那几个了……谁能解释下？这些发言能过人机验证吗？还有一个更离谱的，反过来咬我的已经被我举报off-topic了，根本不知所云，请问muyuan如何解释？真的是自发的吗

## #34 重度粉毛厨 (@MatsuzakaSato)

Created: 2026-08-10T11:28:04.119Z
Updated: 2026-08-10T11:28:04.119Z
Reply to: #30 慕鸢

也就是说，

“最高的山”的标题不是你写的

部分人用公益站维护你的时候你是看不见的

商业推广帖里的公益站链接也不是你放的，对吗

我不觉得你有什么帽子，反倒是佬友们被扣了不少帽子

[![Screenshot_2026-08-10-19-27-14-695_com.android.chrome-edit](https://linux.do/assets/mirrored/5c/5c72ea5a47e0a96d22dea3c8cba2342671c6391a51a84647c47470a1b1c0b923.jpeg)Screenshot_2026-08-10-19-27-14-695_com.android.chrome-edit1440×1407 264 KB](https://cdn3.ldstatic.com/original/4X/7/7/5/7756d133788144174387322accdcfb8fbda6bc88.jpeg)

## #35 云水归山 (@yunshuiguishan1343)

Created: 2026-08-10T11:28:46.644Z
Updated: 2026-08-10T11:37:05.302Z

省流：

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 我已经证明了这个检测方法是不准确的，自然而然，基于这个方法指控我掺假，就是不对的

无法拿出当时日志，也无法鉴定模型为真，只能鉴定测出错误的模型的方法是错误的，鉴于日志确实被删了，似乎也没有更好的鉴定方法但咬死没掺假感觉也是不严谨的吧

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 但是有tg群的用户表示：我在暂停退款之前提交了申请，为什么也没给退？
> 客服团队处理售后也是有先后的，售后的主力在qq群那边，tg群的处理的确有些滞后，这确实是我们的问题，我在此道歉并承诺，后续会继续优化tg群的售后服务质量，不让类似的事件再次发生。
> 但是究其根本，退款是因为掺假，在已经证明掺假的指控不成立的情况下，暂停退款也是ok的。

因为你没有加我们的QQ群，我们不退款

有用户指责中转站出了问题，但似乎使用了质量不佳的脚本，你的选择是

A：找出当时的日志 / 用科学方法说明该脚本为何没问题，仅凭借 juice 的鉴定为何是片面的，告知用户的情况属于正常模型，不予补偿

B：迅速滑轨后该时间段内全部退款

C：用自己的号证明检测脚本不靠谱，却不去证明当时的号是靠谱的，先给了一部分用户用财消灾，客服没看到就等于不存在

## #36 甘尼克斯 (@KIVINXU)

Created: 2026-08-10T11:28:59.484Z
Updated: 2026-08-10T11:28:59.484Z

已经吃腻了，这些瓜。怎么感觉持续了好长时间。

## #37 vernicligm (@vernicligm)

Created: 2026-08-10T11:29:53.406Z
Updated: 2026-08-10T11:33:53.280Z

干嘛对公益站这么苛刻呢，能用就用觉得不好不用就是了，掺假不掺假很多是上游问题，检测一个值就能说明问题吗，不见得

## #38 慕鸢 (@user792)

Created: 2026-08-10T11:30:39.975Z
Updated: 2026-08-10T11:32:37.829Z
Reply to: #34 重度粉毛厨

![](https://linux.do/assets/mirrored/08/0879026348318feba799ec360d9fc70a5760e4ea54ff6140fc30a0e46a169fce.png) 重度粉毛厨:

> “最高的山” 的标题不是你写的

是我的写的，但是公益站是公益站，星辰是星辰，公益站和星辰没有相关性，但是有人拿最高的山代指我，我觉得这是不对的，君の公益不是我一个人功劳

![](https://linux.do/assets/mirrored/08/0879026348318feba799ec360d9fc70a5760e4ea54ff6140fc30a0e46a169fce.png) 重度粉毛厨:

> 部分人用公益站维护你的时候你是看不见的

如果你看见了，麻烦你点举报

![](https://linux.do/assets/mirrored/08/0879026348318feba799ec360d9fc70a5760e4ea54ff6140fc30a0e46a169fce.png) 重度粉毛厨:

> 商业推广帖里的公益站链接也不是你放的，对吗

用商业站给公益站引流没有问题

![](https://linux.do/assets/mirrored/08/0879026348318feba799ec360d9fc70a5760e4ea54ff6140fc30a0e46a169fce.png) 重度粉毛厨:

> 我不觉得你有什么帽子，反倒是佬友们被扣了不少帽子

我没有扣帽子

## #39 散装江苏 (@is_hp)

Created: 2026-08-10T11:31:45.062Z
Updated: 2026-08-10T11:31:45.062Z
Reply to: #37 vernicligm

[![image](https://linux.do/assets/mirrored/c2/c27f26731fc5474f03faa18c2e70b0a91281dcf6c99e437a7dd8c05ba620d7d2.png)image1405×357 41.8 KB](https://cdn3.ldstatic.com/original/4X/9/7/5/9753aeeb81d06bd41900b8aeedbe7bc2b0f7aedc.png)

这位先生，你在说什么？再见了，off-topic

## #40 hsiangron (@hsiangron)

Created: 2026-08-10T11:32:02.786Z
Updated: 2026-08-10T11:34:01.953Z

大佬，注册了你的付费站是不是公益站就自动销号了，我公益站余额显示的 NaN

哦好了恢复了，是raw的站才是二选一

## #41 MumuSir (@MumuSir)

Created: 2026-08-10T11:32:42.578Z
Updated: 2026-08-10T11:32:42.578Z

我接下来只做一件事，在这个帖子下面找人机然后点点举报

## #42 lram (@lram)

Created: 2026-08-10T11:32:48.767Z
Updated: 2026-08-10T11:32:48.767Z
Reply to: #31 Thoth

举报了，就事论事muyuan佬自己都切割了，说公益站去其他帖子。

## #43 listening (@listening)

Created: 2026-08-10T11:33:06.388Z
Updated: 2026-08-10T11:33:06.388Z
Reply to: #39 散装江苏

看到“公益”两个字就入魔了，全然不顾话题在讨论什么。

## #44 小易易 (@xiaoyiyi)

Created: 2026-08-10T11:33:13.461Z
Updated: 2026-08-10T11:33:35.222Z
Reply to: #38 慕鸢

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 如果你看见了，麻烦你点举报

请问这个该用什么理由举报呢，貌似不合理吧![:laughing:](https://linux.do/assets/mirrored/0d/0d46390df7858374bd26a539915193d11a6bfb5fef11ff8e7572a1d32851b126.png)

## #45 darkhandz (@darkhandz)

Created: 2026-08-10T11:33:18.517Z
Updated: 2026-08-10T11:33:18.517Z

我觉得佬早点一次性，及时地，把所有大家关注的，有疑问的点回答清楚就不会有这么长的风波了

## #46 HollowKnight (@HollowKnight)

Created: 2026-08-10T11:33:57.953Z
Updated: 2026-08-10T11:33:57.953Z
Reply to: #36 甘尼克斯

![](https://linux.do/assets/mirrored/43/43fd7ec0b1270763c874856f15df7f5a1cc360a6cb52a5f2f5a689f93b3d4f2f.png) 甘尼克斯:

> 已经吃腻了，这些瓜。怎么感觉持续了好长时间。

天天都是熟瓜，瓜农们，你方唱罢我登场，这几天L站的瓜都是熟透了的瓜，我也吃腻了 ![:yawning_face:](https://linux.do/assets/mirrored/8c/8cba57ab5078acc32da0eb87acc3e6aaae25e91290a64c0b5f2a2acfb76d3f00.png)

## #47 慕鸢 (@user792)

Created: 2026-08-10T11:34:21.044Z
Updated: 2026-08-10T11:34:21.044Z
Reply to: #35 云水归山

![](https://linux.do/assets/mirrored/b3/b382c33c9a1c53c40544d3d3c0ab77f4585f3a2a1e2e4c89c445d02a93b3c721.png) 云水归山:

> 因为你没有加我们的 QQ 群，我们不退款

为什么要断章取义呢？

![](https://linux.do/assets/mirrored/b3/b382c33c9a1c53c40544d3d3c0ab77f4585f3a2a1e2e4c89c445d02a93b3c721.png) 云水归山:

> 似乎也没有更好的鉴定方法但咬死没掺假感觉也是不严谨的吧

哪里不严谨

## #48 慕鸢 (@user792)

Created: 2026-08-10T11:34:58.411Z
Updated: 2026-08-10T11:34:58.411Z
Reply to: #44 小易易

偏离话题，不当言论即可，这种在我看来就是反串的

## #49 jay (@jaysherlock)

Created: 2026-08-10T11:36:43.805Z
Updated: 2026-08-10T11:38:13.086Z

是你自己说你自己是最帅的男人 也是你自己发帖说公益站是最高的山的

大家真跟着你的那些头衔帖子你捧起来了然后给你摔地上了 你又不乐意了

你也不要狡辩什么最高的山是公益站不是你自己

你的公益站原本也叫muyuan，大家也都知道后来合并改名的君の公益 是你负责的

就像我那天说你 最高的山是你自己评的 最低的沟是rate站评的

说到底大家造神也是跟着你自己起的那些头衔跟着你的公益站捧你而已

但是每次遇到你星辰的负面舆情你好好回应过吗

除了今天，你哪次回应书面格式工整过啊？都不说你的回复态度了

多少人因为你公益站而去付费站充值你一点不知情吗？

你不能只在你享受红利的时候奏乐跳舞 自封头衔

等到把你挂起来狠狠鞭笞你的时候你才说没吃公益站红利

## #50 JokerIvanZK (@JokerIvanZK)

Created: 2026-08-10T11:37:09.388Z
Updated: 2026-08-10T11:37:09.388Z

其实把本篇中公益相关描述删除，解释清楚，道了歉，说明下后续处理办法就完了，没人会揪着不放的

## #51 rickyl (@rickyl)

Created: 2026-08-10T11:37:37.534Z
Updated: 2026-08-10T11:37:37.534Z

原本对你印象挺好的，之前帮你说了几句话还被其他佬喷了，现在作为纯路人就觉得叽里咕噜说一大堆，完全说不到点子上，嘴上说就事论事，行动上东拉西扯、反复横跳

动辄最高的山，最帅的人，这对吗?

## #52 慕鸢 (@user792)

Created: 2026-08-10T11:38:12.917Z
Updated: 2026-08-10T11:39:21.924Z
Reply to: #49 jay

![](https://linux.do/assets/mirrored/73/7366a004a3f11d716f004907b5c795c9457def9537c248b9b94df862014684d9.png) jay:

> 你也不要狡辩什么最高的山是公益站不是你自己

我一个人确实完成不了这么大的工作量

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png)[我是真不敢吃公益站的流量阿](https://linux.do/t/topic/2731681/1)

> 君の公益 是公益站最高的山，我只不过为这座山添了一把土。
> 
> 可以给大家简单说一下分工
> 
> 有人出了两台 ovh 物理服务器，两天 netcup 的 root vps，域名，cf pro 订阅。
> 有人拿出了 Gemini cli 号池
> 有人拿出了自己的时间通宵写防御规则，抵御 ddos 和 cc 攻击
> 有人研究 openai 的风控，自动化拉 k12
> 有人研究怎么防止滥用
> 有人 24 小时如坐针毡盯着后台
> 有人写 outlook 注册机，提供了 6000 多个邮箱
> 有人买代理池和接码
> 有人去找号商买 k12 母号、买 bugteam
> 有人导出数据库的 ip，检查有没有宵小搞分发
> 有人腆着大脸，仗着自己有点名气，到处白嫖接口接入后台
> 
> 不要造神！不要搞个人崇拜！

我之前也早有回应

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png)[关于最近几天 君の的公益 签到都是520的一些解释](https://linux.do/t/topic/2342560/1)

> 对了，大家遇到问题回帖询问即可，不需要单独开贴占用社区资源；
> 
> 以及，不要搞个人崇拜，不要在其他帖子下面刷无关内容，这是不好的。
> 感谢很多佬友的无偿帮助，没有他们，就没有 君の的公益

## #53 LuoYeah (@LuoYeah)

Created: 2026-08-10T11:39:31.783Z
Updated: 2026-08-10T11:45:04.737Z

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 君の星辰 哪个月不送tokens？

呃啊，看的血压高了，你自己都没分清问题的来源。对“造谣掺假”在乎的是有质量需求的用户。送tokens已经类似于公益站的行为，维护的是一般轻度用户，没必要在本次道歉中出现。你这样出道歉申明，除了让轻度用户去攻击其他用户，屁用没有。

实在不行就招个公关吧，顶着“不会公关”的帽子在输出，是何意味![:zany_face:](https://linux.do/assets/mirrored/d6/d62c07b3176f768fde3a6b181fef0780a20ca6cc54d462f0956528056fd4ac7b.png)

## #54 慕鸢 (@user792)

Created: 2026-08-10T11:40:31.189Z
Updated: 2026-08-10T11:40:31.189Z
Reply to: #53 LuoYeah

已经证明了没有掺假

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 然后我下达了指令，让客服团队暂停退款，这是一次乌龙事件，君の的星辰没有掺假。

## #55 jiujiula99 (@jiujiula99)

Created: 2026-08-10T11:40:44.085Z
Updated: 2026-08-10T11:40:44.085Z

相信你的，佬，有些检测的说不定就是不准呢，![:star_struck:](https://linux.do/assets/mirrored/49/494a5d33fa83756c26384a2e7a90142bde9d8d0b4f81c7f2721b9527cf5ce684.png)

## #56 云水归山 (@yunshuiguishan1343)

Created: 2026-08-10T11:41:39.990Z
Updated: 2026-08-10T11:41:39.990Z
Reply to: #47 慕鸢

若 A 方法检测 a 模型，结果为 True ，则 a 模型没有掺假，否则就有掺假嫌疑

现有 B 方法检测 a 模型，结果为 False ，则可证明 B 方法不准确

但 B 方法检测 b 模型结果为 False，无法证明 b=a

不过日志都删了确实当时的真伪无法得证，所以现在没有好的方法，仅就您帖子的描述不当产生质疑

## #57 freeqbar (@freeqbar)

Created: 2026-08-10T11:42:00.960Z
Updated: 2026-08-10T11:42:00.960Z

![](https://linux.do/assets/mirrored/d7/d74cfe9b33859f913e71c4629b7e438bff23e43b533b68f1f7e5fbb15fd026d6.png)[【夜间科研成果】果汁值和概率层测试，可能确实存在点问题](https://linux.do/t/topic/2728901/53)

> 就比如星辰AI的这个thinking异常，群里不是一个人都遇到这种情况，当时我自己用也出现了，没截图留存就用了群里的图
> [![f328211dead4e16fea22d5584d79afb9](https://linux.do/assets/mirrored/7e/7ee9161989cd7692d28ac2ea230e2129e83470c34dc6fc0be870308deaeb5f0d.png)f328211dead4e16fea22d5584d79afb9906×1052 76.2 KB](https://cdn3.ldstatic.com/original/4X/b/a/b/bab752f253c9ef76d5e2c6635a10b82454870460.png)

这个问题群里也有人问（图片从售后群里找来的，我自己当天的记录没翻到，但是也遇到过好几次这个情况），客服说没问题 ![:distorted_face:](https://linux.do/assets/mirrored/84/8409bfdb50cdec5b82b1b0bc3c183a371faa3ef54f8e1252b7ce40b26233b0fb.png)

[![ScreenShot_2026-08-10_193922_695](https://linux.do/assets/mirrored/fb/fbe8cdee5995e8529d30188da6d698dbf86f5be59f94219dee728d1d76bb79a7.png)ScreenShot_2026-08-10_193922_695388×749 28.2 KB](https://cdn3.ldstatic.com/original/4X/2/d/7/2d743c86ccbc1db5a059023b02c8fc1df1a66544.png)

7月29日我同时在蹬其他中转和自建的号池，L站、各种AI群也搜了一圈，没有其他人说codex反代有出现这个问题，就星辰AI的GPT是这样的

  
    

    ![](https://linux.do/assets/mirrored/c5/c5b9ffaef468155aebfc3b0d90b1a99e88352e44861f21b432b2ea9d3d8ba9c5.png)
    
      [【夜间科研成果】果汁值和概率层测试，可能确实存在点问题](https://linux.do/t/topic/2728901/77) [
  

开发调优](https://linux.do/c/develop/4)
    

  

  
> ooioo的0.08也总是这个情况，另外还有一家记得不是很清楚了 
>  [[image]](https://cdn3.ldstatic.com/original/4X/b/4/a/b4ae66c4e27f2c7798987d042a4ed0327ac81ed0.png)

另一位佬友在其他中转站当天也遇到了这个情况，有合理的解释吗？

thinking输出在正文里的，怎么都不太像是codex反代出来的GPT吧

## #58 vernicligm (@vernicligm)

Created: 2026-08-10T11:42:34.945Z
Updated: 2026-08-10T11:42:34.945Z
Reply to: #37 vernicligm

哈哈，发现真是捅了马蜂窝，有气不要往我身上发，公益是公益，付费是付费，谢谢各位佬友了

## #59 繁星之子卡萨蒂亚 (@Kasidia)

Created: 2026-08-10T11:43:16.719Z
Updated: 2026-08-10T11:45:00.461Z

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 为什么一提到送tokens，就开始疯狂抹黑公益站？

我估计很多人以为你说的是公益站大放送=

就是没明确到底是以哪个站的名义送的 所以会有这种问题

## #60 慕鸢 (@user792)

Created: 2026-08-10T11:43:30.641Z
Updated: 2026-08-10T11:43:30.641Z
Reply to: #57 freeqbar

这个应该是开启了输出思考到正文

## #61 抹茶毛巾卷 (@SSSS)

Created: 2026-08-10T11:43:33.543Z
Updated: 2026-08-10T11:47:38.158Z
Reply to: #37 vernicligm

不是，这到底是在干嘛啊 ![:distorted_face:](https://linux.do/assets/mirrored/84/8409bfdb50cdec5b82b1b0bc3c183a371faa3ef54f8e1252b7ce40b26233b0fb.png) 我真的后背发凉

三级号就算了，新注册一头扎进节奏帖子开始宣传公益站是在干嘛？

这跟公益有关系吗？

## #62 LuoYeah (@LuoYeah)

Created: 2026-08-10T11:43:59.945Z
Updated: 2026-08-10T11:43:59.945Z
Reply to: #54 慕鸢

可以的，不过这是一个单方面的申明，希望站内的佬友也这么认为吧![:thinking:](https://linux.do/assets/mirrored/51/5116f7d07677f06785887c0af23c189b541a306d6b792d605ffaf3ed9f0e912d.png)

宣传的多了已经成固有印象了说是（），我的问题，我改一下说法，避免歧义

## #63 J＆G (@JasonGui)

Created: 2026-08-10T11:44:33.153Z
Updated: 2026-08-10T11:44:33.153Z
Reply to: #37 vernicligm

此话题和公益站无关，此次是商业站回应，muyaun佬也说不谈公益站了

## #64 Zeitwanderer (@Ethan_BY)

Created: 2026-08-10T11:44:34.831Z
Updated: 2026-08-10T11:44:34.831Z

重新发一个 简短干练的官方声明吧

描述问题：引用你之前的帖子
解决方案 处理方法
展望未来 表达未来怎么做
表达你的态度
声明人
时间日期

再别提中转站的情况下，提公益站了 ![:melting_face:](https://linux.do/assets/mirrored/9e/9e93fb8c3bb4ac119d8c84cb34d4024b41c1a12dc76b847b91a1f04a328705d9.png)

## #65 重度粉毛厨 (@MatsuzakaSato)

Created: 2026-08-10T11:44:40.614Z
Updated: 2026-08-10T11:44:40.614Z
Reply to: #38 慕鸢

既然认为没有相关性，为什么要在商业推广底下引用公益站内容？
既然你要求我们举报这些内容，应该可以认为，你其实知道这些内容违反了某条版规。那你作为直接相关方，为什么不进行举报，或者采取其他措施控制？
没有实锤我就不说什么数字生命了
争议还没平息，问题原委还没查实，所有参与讨论的人莫名其妙地成了相互攻击/血流成河/社区矛盾/个人恩怨，然后莫名其妙地被要求结束讨论，接着奏乐接着舞？

哦对了

> 本帖使用社区公益推广，符合推广要求。我申明并遵循社区要求的以下内容：
> 
> ……
> 
> 《我的项目无关联的商业项目》

## #66 listening (@listening)

Created: 2026-08-10T11:44:49.079Z
Updated: 2026-08-10T11:48:22.820Z
Reply to: #54 慕鸢

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 已经证明了没有掺假

举证责任在谁？目前确切的结论只有检测手段不准确是吧，并不能证明你有没有掺假，这是笔糊涂账。

你说没掺假，站在消费者的角度看这也是一面之辞。（不要在这上面纠缠了，舆论天然不利）

## #67 热爱学习 (@niga)

Created: 2026-08-10T11:45:34.824Z
Updated: 2026-08-10T11:45:34.824Z

我觉得最近站内中转站争议真的好多阿

不禁让人反思是不是应该要有一些审核制度？或是监管制度？

## #68 菜问👀 (@user382)

Created: 2026-08-10T11:45:52.382Z
Updated: 2026-08-10T11:45:52.382Z

嗅到了上一个被抬走的那个风男人的味道![:shaking_face:](https://linux.do/assets/mirrored/34/348b0255d77437c169129b4420b4403c3db8175a857aefc40ccf2bcd9ad9449d.png)

## #69 嘿嘿 (@3299773983)

Created: 2026-08-10T11:48:59.627Z
Updated: 2026-08-10T11:48:59.627Z
Reply to: #58 vernicligm

讨论付费，你谈公益，加入日期一小时前，你是谁的托啊好难猜

## #70 雷暴天王 (@yuda_huo)

Created: 2026-08-10T11:52:05.547Z
Updated: 2026-08-10T11:52:05.547Z
Reply to: #69 嘿嘿

我感觉他有点串的嫌疑，感觉他像拱火的

## #71 z (@ztsyy)

Created: 2026-08-10T11:52:11.166Z
Updated: 2026-08-10T11:52:11.166Z
Reply to: #8 回忆

似乎他的额度都已经用完了，所以不予退款。至于是否应该赔偿不得而知。

## #72 慕鸢 (@user792)

Created: 2026-08-10T11:53:12.349Z
Updated: 2026-08-10T11:53:12.349Z
Reply to: #65 重度粉毛厨

![](https://linux.do/assets/mirrored/08/0879026348318feba799ec360d9fc70a5760e4ea54ff6140fc30a0e46a169fce.png) 重度粉毛厨:

> 既然认为没有相关性，为什么要在商业推广底下引用公益站内容？

用富可敌国推广公益站应该并没有什么不妥，高级推广没有限制

![](https://linux.do/assets/mirrored/08/0879026348318feba799ec360d9fc70a5760e4ea54ff6140fc30a0e46a169fce.png) 重度粉毛厨:

> 既然你要求我们举报这些内容，应该可以认为，你其实知道这些内容违反了某条版规。那你作为直接相关方，为什么不进行举报，或者采取其他措施控制？

我很早就呼吁了，不要在其他帖子下面刷无关内容

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png)[关于最近几天 君の的公益 签到都是520的一些解释](https://linux.do/t/topic/2342560/1)

> 对了，大家遇到问题回帖询问即可，不需要单独开贴占用社区资源；
> 
> 以及，不要搞个人崇拜，不要在其他帖子下面刷无关内容，这是不好的。
> 感谢很多佬友的无偿帮助，没有他们，就没有 君の的公益

![](https://linux.do/assets/mirrored/08/0879026348318feba799ec360d9fc70a5760e4ea54ff6140fc30a0e46a169fce.png) 重度粉毛厨:

> 争议还没平息，问题原委还没查实，所有参与讨论的人莫名其妙地成了相互攻击 / 血流成河 / 社区矛盾 / 个人恩怨，然后莫名其妙地被要求结束讨论，接着奏乐接着舞？

之前的表述确实有一些问题，那个帖子下面的佬已经开始互相要炼化LDC，我看到觉得不好，所以那个帖子我希望他沉下去，不要再起争端，但是显然有些佬不满意，所以才有了这个道歉声明

## #73 kalikali (@kalikali)

Created: 2026-08-10T11:54:44.260Z
Updated: 2026-08-10T11:54:44.260Z

商业推广挂公益站，不就是在表达“这个公益站和中转站有关联”的意思吗？

## #74 一摩尔氚 (@1molchuan)

Created: 2026-08-10T11:55:04.694Z
Updated: 2026-08-10T12:09:03.876Z

看着我又觉得好气又觉得好笑。

这样吧过会开一个星辰AI 付费

站（注意是付费站）的岁月史书的wiki 帖子。客观记录。不予评价。公道自在人心

[https://linux.do/t/topic/2735552](https://linux.do/t/topic/2735552)

各位来吧

## #75 hkxbk (@hkxbk)

Created: 2026-08-10T11:58:01.958Z
Updated: 2026-08-10T11:58:01.958Z

不针对这次的风波，但是感觉佬可以找其他的佬或者你开个小号发公益站相关的内容，免得公益站压力这么大 ![:melting_face:](https://linux.do/assets/mirrored/9e/9e93fb8c3bb4ac119d8c84cb34d4024b41c1a12dc76b847b91a1f04a328705d9.png)

## #76 ちーのサバアカです (@_chi_chan_desuka)

Created: 2026-08-10T11:58:53.920Z
Updated: 2026-08-10T11:59:48.135Z
Reply to: #72 慕鸢

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 互相要炼化LDC

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 麻烦你点举报

那到底能不能炼呢，还是说只有不利于自己的帖子才要沉下去？

问题解决了自然就会沉下去了吧？

## #77 慕鸢 (@user792)

Created: 2026-08-10T11:59:52.577Z
Updated: 2026-08-10T11:59:52.577Z
Reply to: #73 kalikali

只有在星辰的第一个帖子提到过这个公益站，而且只是简单的说明了一下，并没有任何其他的内容，后面再也没提过，最近的风波和半年的帖子关系不大

## #78 慕鸢 (@user792)

Created: 2026-08-10T12:00:28.759Z
Updated: 2026-08-10T12:01:08.831Z
Reply to: #76 ちーのサバアカです

请自行举报交给管理员审核，这不归我管（我不是管理员，我处理不了）

## #79 gep (@ElonMusk)

Created: 2026-08-10T12:01:41.132Z
Updated: 2026-08-10T12:01:41.132Z
Reply to: #78 慕鸢

1个小时了，能不能把时间线先改对咧

## #80 roiding (@roiding)

Created: 2026-08-10T12:02:15.543Z
Updated: 2026-08-10T12:02:15.543Z
Reply to: #56 云水归山

我记得上面muyuan不是说路由到的是他自己的codex嘛？那真假只是无法举证证明，但是他买的他不知道是真的嘛？

## #81 超微蓝胖 (@imgdo)

Created: 2026-08-10T12:02:44.634Z
Updated: 2026-08-10T12:02:44.634Z

我记得oooiii啥的那个站以及给了标准道歉模板,这都抄不会,非要跟客户锱铢必较,要真这样说谁能证明那个点到底发生了什么,你有理我们都怕你

## #82 慕鸢 (@user792)

Created: 2026-08-10T12:03:46.056Z
Updated: 2026-08-10T12:03:46.056Z
Reply to: #79 gep

已经挪到最后了

## #83 慕鸢 (@user792)

Created: 2026-08-10T12:05:09.016Z
Updated: 2026-08-10T12:08:39.489Z
Reply to: #81 超微蓝胖

我肯定没理阿

售后处理不及时，没有回应用户关切，是我们星辰售后团队的问题

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> tg 群的处理的确有些滞后，这确实是我们的问题，我在此道歉并承诺，后续会继续优化 tg 群的售后服务质量，不让类似的事件再次发生。

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 最后，也向所有的佬友道个歉，处理舆情不及时，公关能力不到位，导致浪费了各位佬大量的时间和精力，非常抱歉！非常抱歉！非常抱歉！

## #84 一摩尔氚 (@1molchuan)

Created: 2026-08-10T12:07:00.727Z
Updated: 2026-08-10T12:18:14.336Z

[https://linux.do/t/topic/2735552](https://linux.do/t/topic/2735552)

各位来吧。我只写了基本规则因为人在外面手机快没电了。欢迎编辑。

二编：被拿下

## #85 一个ai的tool (@ailinux)

Created: 2026-08-10T12:08:05.932Z
Updated: 2026-08-10T12:08:05.932Z

这次公关真的就好很多了,希望后面可以跟进中转站透明化

## #86 miemie Jun (@miemie_Jun)

Created: 2026-08-10T12:09:25.923Z
Updated: 2026-08-10T12:09:25.923Z

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 如下，我已经证明了这个检测方法是不准确的，自然而然，基于这个方法指控我掺假，就是不对的。

是不是可以理解为，前一天有人在饭馆吃完饭，然后说自己拉肚子了，去小诊所认为是食物中毒。你知道后发现前一天食材留样已经扔了。然后开始退款

第二天拿第二天的留样找诊所对质了，认为诊所的诊断有问题所以停止退款

可以这么理解吗

## #87 YOKAI (@ECHO1)

Created: 2026-08-10T12:09:29.918Z
Updated: 2026-08-10T12:09:29.918Z

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 星辰在早期的时候，售后团队确实出现过售后服务态度差的问题，我当时也是羞愧万分，怎么还有佬友充钱还被怼的，那次事件之后，我对星辰售后团队进行一次彻底的整顿。

真的假的，早期是多早，7月26算早吗

[![image](https://linux.do/assets/mirrored/bd/bd7a29dc74bd5f7f13bc121e03dbf1c256d3b5cb49088c7d913c92b8ba3caf2c.png)image480×1623 78.4 KB](https://cdn3.ldstatic.com/original/4X/c/b/a/cbabc2f732db86c4e6401248284604f6426beec5.png)

## #88 z (@ztsyy)

Created: 2026-08-10T12:09:55.801Z
Updated: 2026-08-10T12:10:40.213Z
Reply to: #72 慕鸢

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 用富可敌国推广公益站应该并没有什么不妥，高级推广没有限制

慕鸢佬的初心是这般。但是

瓜田不纳履

李下不整冠

大抵如此

## #89 AkaChou (@AkaChou)

Created: 2026-08-10T12:10:13.034Z
Updated: 2026-08-10T12:10:13.034Z

然而站在中立的角度劝说不要起哄的我，被形容成二师兄和狗 ![:melting_face:](https://linux.do/assets/mirrored/9e/9e93fb8c3bb4ac119d8c84cb34d4024b41c1a12dc76b847b91a1f04a328705d9.png)，希望有些佬们还是理性一些，莫要嘲讽开炮，理性看待问题，科学求证～

## #90 慕鸢 (@user792)

Created: 2026-08-10T12:11:11.584Z
Updated: 2026-08-10T12:11:11.584Z
Reply to: #87 YOKAI

这个我单独发帖说一下吧

## #91 一摩尔氚 (@1molchuan)

Created: 2026-08-10T12:16:35.022Z
Updated: 2026-08-10T12:16:35.022Z

集中帖子各位被拿下了。

不多说了，就这样吧。我也不再发这个帖子了

## #92 Foresee (@Foresee)

Created: 2026-08-10T12:17:10.470Z
Updated: 2026-08-10T12:17:10.470Z
Reply to: #91 一摩尔氚

WTF 为啥是这样的 佬 怎么说 跟管理员沟通了吗

## #93 roiding (@roiding)

Created: 2026-08-10T12:17:15.823Z
Updated: 2026-08-10T12:17:15.823Z
Reply to: #91 一摩尔氚

我在吃瓜，我都没弄懂大家在闹啥呢…看帖子就是一个模型有没有造假的问题呗，咋越整越看不懂了…史书我也没见人编辑

ps：帖怎么没了

## #94 齐天小圣 (@sgml)

Created: 2026-08-10T12:17:19.972Z
Updated: 2026-08-10T12:17:19.972Z

关于tg的后续我还是纳闷，管理在tg里说过之前收集的退款全部取消吗，应该没吧 有的话A佬也不会开帖问这个了，没有的话还是补一个吧![:joy:](https://linux.do/assets/mirrored/c2/c252a58367211c11d839155e50dc5e98551826c64b8d2e8d6267124c054ceae0.png)

## #95 💪 🎯 🚀 ☁️ (@lizy)

Created: 2026-08-10T12:17:33.019Z
Updated: 2026-08-10T12:17:33.019Z

官方确实会有降智，周六重置之后 我蹬空了4个plus/team号，代码质量比早几天用中转站/公益站的还差 ，除了偷换模型想不到其他可能～

## #96 一摩尔氚 (@1molchuan)

Created: 2026-08-10T12:17:48.252Z
Updated: 2026-08-10T12:17:48.252Z
Reply to: #92 Foresee

没有直接被举报删帖子。

始皇似乎认为我在挂人。尽管我并不是这么觉得。

当然尊重管理员。

## #97 ҨҨㄋㄟㄋㄟ好喝到咩噗茶 (@Vetmin)

Created: 2026-08-10T12:18:44.518Z
Updated: 2026-08-10T12:18:44.518Z
Reply to: #89 AkaChou

跟你有相同遭遇的佬友不在少数，感觉快要发展到U型锁的程度了。你要是反驳两句还会吃举报删帖 ![:laughing:](https://linux.do/assets/mirrored/0d/0d46390df7858374bd26a539915193d11a6bfb5fef11ff8e7572a1d32851b126.png)

## #98 JamesLi (@JamesLiAndroid)

Created: 2026-08-10T12:19:29.362Z
Updated: 2026-08-10T12:19:29.362Z

openai降智是真的，周五的时候，相关任务死活跑不动，而且不执行指令，自己就飘了

## #99 roiding (@roiding)

Created: 2026-08-10T12:20:05.199Z
Updated: 2026-08-10T12:20:17.449Z
Reply to: #96 一摩尔氚

前几天在某个公益站贴帮站长和黑子对线，吃举报吃的一下午邮件不断，降级了，举报这东西我都习惯了感觉，你还无法申诉…我认为正常的回复，管理说我不良言论啥啥啥的…

## #100 慕鸢 (@user792)

Created: 2026-08-10T12:20:26.523Z
Updated: 2026-08-10T12:23:55.044Z
Reply to: #94 齐天小圣

马上补上

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 需要说明的是：当时 tg 群这边还在收集整理阶段，qq 群那边是直接退款的。
> 
> 这就导致这 53 名用户全部都是 qq 群这边的，tg 群那边都没有退款，这是我的失职，后续一定一碗水端平，处理好售后服务，非常抱歉！希望各位佬原谅。

## #101 一摩尔氚 (@1molchuan)

Created: 2026-08-10T12:21:35.253Z
Updated: 2026-08-10T12:21:35.253Z
Reply to: #99 roiding

理解和尊重管理员吧。不要在这里引起对立。

回头找更好的地方记录吧。

## #102 roiding (@roiding)

Created: 2026-08-10T12:23:08.608Z
Updated: 2026-08-10T12:25:57.348Z
Reply to: #100 慕鸢

muyuan佬，个人的理解啊，请指正（本人没有付费站号）

如果要退，那就应该在你宣布停止退款前登记了退款的人都退，而不是现在一部分退了一部分没退（我看你之前这么表述的）

如果觉得模型是没出问题的，那后面的如果不退的话，应该把前面落袋的也追溯回来

一部分退一部分不退就有点幸存者偏差了，因为人是不患寡而患不均

我也不知道这事来龙去脉，不评价模型的事，但退款这个事我看你回的帖好像就是一部分退了一部分没退

## #103 齐天小圣 (@sgml)

Created: 2026-08-10T12:23:34.596Z
Updated: 2026-08-10T12:23:34.596Z
Reply to: #100 慕鸢

真没发啊 ![:scream:](https://linux.do/assets/mirrored/42/42e6b438eba01cf441e8e1bdde37ddb2bd9278ac26526acbb930c1557a75e0b7.png)tg里的用户现在还在默默苦等退款到账啊![:joy:](https://linux.do/assets/mirrored/c2/c252a58367211c11d839155e50dc5e98551826c64b8d2e8d6267124c054ceae0.png)那tg的售后确实需要优化

## #104 X风流 (@X-Wanderer)

Created: 2026-08-10T12:25:26.597Z
Updated: 2026-08-10T12:29:41.858Z
Reply to: #15 Chinamobile

（帖子已被作者删除）

## #105 云水归山 (@yunshuiguishan1343)

Created: 2026-08-10T12:26:04.337Z
Updated: 2026-08-10T12:26:04.337Z
Reply to: #102 roiding

这件事发展到现在最简单的处理方法就是给tg那个佬退款堵一下嘴，最先爆出这件事情的佬不太计较款项，然后声明juice值不足以证明模型为真，然后冷一阵子过几天发token，有人质疑就拿已退款堵嘴

不管认不认可逻辑就当破财消灾得了

只能说muyuan佬想赚钱

## #106 roiding (@roiding)

Created: 2026-08-10T12:27:45.424Z
Updated: 2026-08-10T12:27:45.424Z
Reply to: #105 云水归山

也不是，想赚钱一开始就不会无条件给那些人退了。但同样的一群人，不管因为什么原因申请的退款，要么都退要么都不退，因为人家既然在你宣布停止退款前提交了申请，前面的退了后面的不退就有点不均了…

## #107 neroZac (@neroZac)

Created: 2026-08-10T12:28:08.751Z
Updated: 2026-08-10T12:35:11.706Z

（帖子已被作者删除）

## #108 Hiccup (@Hiccup_620)

Created: 2026-08-10T12:28:56.311Z
Updated: 2026-08-10T12:28:56.311Z
Reply to: #96 一摩尔氚

想起了更早的关于戏弄诈骗网站的记录，按照这个说法，那也是挂人吧。。。

## #109 X风流 (@X-Wanderer)

Created: 2026-08-10T12:29:21.364Z
Updated: 2026-08-10T12:29:21.364Z
Reply to: #38 慕鸢

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 用商业站给公益站引流没有问题

确实是这样，但是这两个站是不是有点互相引流了 ![:distorted_face:](https://linux.do/assets/mirrored/84/8409bfdb50cdec5b82b1b0bc3c183a371faa3ef54f8e1252b7ce40b26233b0fb.png)

## #110 慕鸢 (@user792)

Created: 2026-08-10T12:29:39.926Z
Updated: 2026-08-10T12:29:39.926Z
Reply to: #102 roiding

你说的有道理，我让客服把收集上来的都退掉吧，也算个了结，现在就让售后团队去弄

## #111 Haruna Amaori (@wyttle)

Created: 2026-08-10T12:29:46.975Z
Updated: 2026-08-10T12:29:46.975Z
Reply to: #105 云水归山

换别家中转早就只要你想退统统退了 不管你用没用充的钱全退 中转站差这么几个token钱吗

## #112 云水归山 (@yunshuiguishan1343)

Created: 2026-08-10T12:29:54.225Z
Updated: 2026-08-10T12:29:54.225Z
Reply to: #106 roiding

其实muyuan佬想赚钱是个梗哈哈哈哈哈

起因是网易的一款乙女游戏被爆出ai作画后发了一个“xxxx想赚钱”阐述自己开发的不容易

## #113 xie reens (@xie_reens)

Created: 2026-08-10T12:30:02.533Z
Updated: 2026-08-10T12:30:02.533Z

从此事可以看出，相比于退款堵漏，更关键的是要找出实际问题，急于先退款并不是个好选择

## #114 慕鸢 (@user792)

Created: 2026-08-10T12:31:09.453Z
Updated: 2026-08-10T12:32:00.527Z
Reply to: #113 xie reens

确实，决策失误了，唉，当时没想清楚，对不起各位佬了，耽误大家事件了

## #115 Angel (@HatsuneMiku)

Created: 2026-08-10T12:32:09.633Z
Updated: 2026-08-10T12:55:23.515Z
Reply to: #107 neroZac

（帖子已被作者删除）

## #116 慕鸢 (@user792)

Created: 2026-08-10T12:33:15.630Z
Updated: 2026-08-10T12:33:15.630Z
Reply to: #115 Angel

这种发布无关内容的直接举报抬走就行了

## #117 Petals (@Petals)

Created: 2026-08-10T12:34:28.012Z
Updated: 2026-08-10T12:34:28.012Z
Reply to: #114 慕鸢

是不是因为我下午的功劳

[![image](https://linux.do/assets/mirrored/1d/1df6b46e2c86cbc803c6ee58479b47921ac43904f7a54c632c28594f030963e2.jpeg)image1035×381 57 KB](https://cdn3.ldstatic.com/original/4X/3/d/9/3d980288b0c7882c94373b6ab39d9c8eb450d805.jpeg)

## #118 慕鸢 (@user792)

Created: 2026-08-10T12:35:09.756Z
Updated: 2026-08-10T12:35:09.756Z
Reply to: #117 Petals

谢谢你，耽误你时间和精力了，对不起

## #119 某人 (@abao)

Created: 2026-08-10T12:38:15.906Z
Updated: 2026-08-10T12:40:59.981Z

说句题外话，这次事件的处理过程与结果和之前那次事件差不多啊，上次和这次的公关问题都很大啊。 ![:distorted_face:](https://linux.do/assets/mirrored/84/8409bfdb50cdec5b82b1b0bc3c183a371faa3ef54f8e1252b7ce40b26233b0fb.png)

ps:说的可不是退款问题，上次那个是客服问题。

## #120 慕鸢 (@user792)

Created: 2026-08-10T12:40:43.360Z
Updated: 2026-08-10T12:40:43.360Z
Reply to: #119 某人

确实有问题，非常抱歉

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 最后，也向所有的佬友道个歉，处理舆情不及时，公关能力不到位，导致浪费了各位佬大量的时间和精力，非常抱歉！

## #121 kevechang (@kevechang)

Created: 2026-08-10T12:42:33.981Z
Updated: 2026-08-10T12:42:33.981Z
Reply to: #56 云水归山

muyuan 的意思是请求拉到了号池 总不能号池出来的是假的吧

## #122 polaris (@polaris)

Created: 2026-08-10T12:46:05.543Z
Updated: 2026-08-10T12:46:05.543Z

跟着吃瓜几天

到这个帖子也才说明白

即最初回应退款认为是上游问题，直接退款

复核发现是自己的号池，那就认为肯定没假，简单跑了一遍测试完事

回复的重点介绍这个是自己的号池，认为只要介绍无上游就可以证明指控虚假

对于更多佬友关注的模型到底有没有掺水懒得解释了，更加懒得回答细节时间线的问题，仅对少数指控重点进行零星片段性回复

一直被盯着几个帖子轮流锤了几天，这才给梳理了一下基本的时间线

以之前的声望，要是第一天按隔壁的路子给个完整的号池juice自测解释，或者哪怕最简单的梳理一个清晰明确无错误的时间线都不至于扯这么多天

但由于证据太少而且原始证据已灭失，到底是掺水还是降智到目前还是无法判断，只能说是两个可能性同时存在的薛定谔状态了

## #123 vernicligm (@vernicligm)

Created: 2026-08-10T12:46:27.376Z
Updated: 2026-08-10T12:54:31.836Z
Reply to: #115 Angel

此帖子已被社区举报，现已被临时隐藏。

## #124 niubiPlus1 (@niubiPlus1)

Created: 2026-08-10T12:48:01.201Z
Updated: 2026-08-10T12:48:01.201Z
Reply to: #121 kevechang

这简单呀 来个人测出官方订阅的sol high juice为 48，这样一切都迎刃而解了

## #125 yumc (@yumc)

Created: 2026-08-10T12:49:10.879Z
Updated: 2026-08-10T12:49:10.879Z

其实佬友们只是需要一个正式的回应，而不是顾左又顾右，随意终结话题只会引起更大波澜。

大家看不惯大多数都是态度问题。就像muyuan佬的签名：“不要在他那浪费时间”，此次事件他没有像自己写的，帖子拖了三天才回应，风波起来才回应，要不是因为这个谁又愿意浪费自己时间。如果从风波开始就发帖回应，或者像今天发道歉声明，也不会持续这么久，也不会浪费时间。

## #126 慕鸢 (@user792)

Created: 2026-08-10T12:49:20.922Z
Updated: 2026-08-10T12:51:50.377Z
Reply to: #123 vernicligm

大哥，不要再在这个帖子下面拿公益站说事了，我真遭不住了阿，公益站的问题去公益站帖子下面反应，别在这里搞了，都删了吧

## #127 半口小希 (@aphoba)

Created: 2026-08-10T12:50:29.269Z
Updated: 2026-08-10T12:50:29.269Z

你什么时候回应这个帖子的问题

  
    

    ![](https://linux.do/assets/mirrored/e4/e4ea3b9ff99685ae7044cb99ebb536bb151b7a4e38c4809fb0643ca32888a2e8.png)
    
      [星辰站这件事其实很好解决的，为什么要一直困难化呢？](https://linux.do/t/topic/2728919) [
  

搞七捻三](https://linux.do/c/gossip/11)
    

  

  
> 本来今天起床之后看到有这么多消息，我就感到星辰站的这件事已经有结果了 
> 我还满怀期待的打开了回复我的那个帖子 
> 
> 结果就是：啊~~原来是这样。 
> 那我只能再次发帖了。 
> 
> [#p-21396785-user792-l-saluting_face-1](#p-21396785-user792-l-saluting_face-1)再次声明：我不针对人，我针对的永远都是事情。 [@user792](https://linux.do/u/user792) 我本来非常不想要把你的站点挂起来的，因为你的最开始创建的那个公益站，是我进入L站之后认识的第一个公益站。。虽然我没用，但是我还是很感谢你作为第一批的公益站主能够给佬…

## #128 慕鸢 (@user792)

Created: 2026-08-10T12:51:23.757Z
Updated: 2026-08-10T12:51:23.757Z
Reply to: #127 半口小希

这个帖子下面我已经回复过了，这里我也做了补充

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 我让客服把收集上来的都退掉吧，也算个了结，现在就让售后团队去弄

## #129 vernicligm (@vernicligm)

Created: 2026-08-10T12:52:59.354Z
Updated: 2026-08-10T12:52:59.354Z
Reply to: #126 慕鸢

好啦好啦，不搞了，我说啥他们都觉得我是你小号，哈哈，XSWL。

## #130 慕鸢 (@user792)

Created: 2026-08-10T12:53:25.410Z
Updated: 2026-08-10T12:53:25.410Z
Reply to: #129 vernicligm

看的我都力竭了

## #131 Angel (@HatsuneMiku)

Created: 2026-08-10T12:54:19.133Z
Updated: 2026-08-10T12:55:10.135Z
Reply to: #129 vernicligm

![](https://linux.do/assets/mirrored/d9/d9098eb323f2cff6e469dba533ef3d3238ceee0cd260f59a624c52e381b24f37.png) vernicligm:

> 我说啥他们都觉得我是你小号，哈哈，XSWL。

不是说你是不是小号 主要是注册1h 第一个帖子就是在 中转站下面发公益站 怎么看怎么像机器人啊![:distorted_face:](https://linux.do/assets/mirrored/84/8409bfdb50cdec5b82b1b0bc3c183a371faa3ef54f8e1252b7ce40b26233b0fb.png)![:distorted_face:](https://linux.do/assets/mirrored/84/8409bfdb50cdec5b82b1b0bc3c183a371faa3ef54f8e1252b7ce40b26233b0fb.png)![:distorted_face:](https://linux.do/assets/mirrored/84/8409bfdb50cdec5b82b1b0bc3c183a371faa3ef54f8e1252b7ce40b26233b0fb.png)![:distorted_face:](https://linux.do/assets/mirrored/84/8409bfdb50cdec5b82b1b0bc3c183a371faa3ef54f8e1252b7ce40b26233b0fb.png)

![](https://linux.do/assets/mirrored/29/29b28fab3cca80372ac1539dc8b919be0eb276c73fdfab4a43d1bc85730735ff.png) 慕鸢:

> 大哥，不要再在这个帖子下面拿公益站说事了，我真遭不住了阿，公益站的问题去公益站帖子下面反应，别在这里搞了，都删了吧

[@user792](https://linux.do/u/user792)  我的也删掉了![:saluting_face:](https://linux.do/assets/mirrored/40/405ef0f64222c8ac24eb7fe1931aafb4443399a6e0862ebe438e11783769285b.png)![:saluting_face:](https://linux.do/assets/mirrored/40/405ef0f64222c8ac24eb7fe1931aafb4443399a6e0862ebe438e11783769285b.png)![:saluting_face:](https://linux.do/assets/mirrored/40/405ef0f64222c8ac24eb7fe1931aafb4443399a6e0862ebe438e11783769285b.png)

## #132 vernicligm (@vernicligm)

Created: 2026-08-10T12:54:24.168Z
Updated: 2026-08-10T12:54:24.168Z
Reply to: #130 慕鸢

咱们身正不怕影子斜，半夜不怕鬼敲门，不是嘛，哈哈哈

## #133 云水归山 (@yunshuiguishan1343)

Created: 2026-08-10T12:55:30.619Z
Updated: 2026-08-10T12:55:30.619Z
Reply to: #132 vernicligm

我都有点觉得你是不是别的中转站跑来串的来火上浇油![:rofl:](https://linux.do/assets/mirrored/4a/4a371ef1123fee52185f3098d3d3b65dc7f695fdd574ea977ea2afedff963ad5.png)

## #134 ks (@kingd)

Created: 2026-08-10T12:55:42.022Z
Updated: 2026-08-10T12:55:42.022Z
Reply to: #132 vernicligm

不知道为什么 看你的话语我有一种尴尬加无语的感觉

## #135 Foresee (@Foresee)

Created: 2026-08-10T12:55:53.339Z
Updated: 2026-08-10T12:56:19.622Z
Reply to: #129 vernicligm

谈论付费站的时候，不要牵扯公益站的事情。

公益做的很好，付费做的很差，不冲突。这篇文章不是对付费站的说明吗

![](https://linux.do/assets/mirrored/d9/d9098eb323f2cff6e469dba533ef3d3238ceee0cd260f59a624c52e381b24f37.png) vernicligm:

> 干嘛对公益站这么苛刻呢

这样看来发言还是很奇怪，佬，你底下的boost那么多反对的声音如果说明不了什么，那就请阅读社区准则…我感觉你再回复能又激发大家讨论的热情就是了

## #136 雷暴天王 (@yuda_huo)

Created: 2026-08-10T12:57:03.811Z
Updated: 2026-08-10T12:57:03.811Z
Reply to: #132 vernicligm

本来事都已经结束了，你非得在那当串子，不理解

## #137 慕鸢 (@user792)

Created: 2026-08-10T12:58:34.626Z
Updated: 2026-08-10T12:58:34.626Z
Reply to: #132 vernicligm

别瞎搞了，你去忙你自己的吧，别再起节奏了

## #138 Theo (@jmklkj)

Created: 2026-08-10T13:07:21.991Z
Updated: 2026-08-10T13:07:21.991Z
Reply to: #137 慕鸢

个人意见：这是节奏，其实也是机会。如果佬开始的时候全力处理这个问题，应该不至于节奏越来越大 ![:smiling_face_with_tear:](https://linux.do/assets/mirrored/ad/ad1dcb074a55b2b3bacd1744db2a851d6ca83decb7e232e3fcb08e5c3e37357b.png)。

