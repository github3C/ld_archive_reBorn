# 继续公益站投毒一说

Source: https://linux.do/t/topic/2219887
Version: v1
Posts: 25
Missing floors: none

## #1 yudi (@yudisama)

Created: 2026-05-21T08:30:35.321Z
Updated: 2026-05-21T08:30:35.321Z

此人早有征兆

时间应该是早于 星期二

![496569d517a8348ba32e4dc557362b50](https://linux.do/assets/mirrored/ec/ecdf812128cabee7042ee04cc9dc655478bc3e1d8699581f5db6aa34ef2d32b4.png)

[![ce4de5f000f627dd893bc4604fc74126](https://linux.do/assets/mirrored/1f/1fa0759a539883f2a560eefd5bc5ddc2055f4f18cf50f97d1fcdfab5c9b51dce.png)ce4de5f000f627dd893bc4604fc74126910×162 9.58 KB](https://linux.do/assets/mirrored/1f/1fa0759a539883f2a560eefd5bc5ddc2055f4f18cf50f97d1fcdfab5c9b51dce.png)

![ea8201dd3f7ad0569d48fbb232406369](https://linux.do/assets/mirrored/a0/a0ab21947d990206298b48d79ee88d08c5dc7e61f6b498ab511ed0d7ff1b78ef.png)

[![ffcecb030ea39a6891e2a56adb5c4765](https://linux.do/assets/mirrored/15/15017f90673544cc64c9bb5c07907e2878023ba554209b9c406d388227ebe7a1.png)ffcecb030ea39a6891e2a56adb5c4765538×656 45.6 KB](https://cdn3.ldstatic.com/original/4X/1/a/e/1aecaafcae2d000aaeb34e9501bc4f894bb592ed.png)

[![60fba2f4000b0bdc2077393ce3d14d7f](https://linux.do/assets/mirrored/93/93e365be6f2d66d0bc89102d7fca3968586c5f6f47099c2d69e5e481fceb12f8.jpeg)60fba2f4000b0bdc2077393ce3d14d7f887×301 57.9 KB](https://cdn3.ldstatic.com/original/4X/2/0/3/20319149dcc454577e3e478c6e94eec6c62d287d.jpeg)

那个时候被喷了,改了 换成返回体那种了,可以过滤

后面就是 进群的有key 用 , 流出去的sk_free 打广告

直到今天 5.21 逆天的来了

[![adf5607b3eac76fd8e8efd2842aee74d](https://linux.do/assets/mirrored/0a/0a023de19b68b44966b8a559054d844c1ce2d2796aefe342f7283919242b716d.jpeg)adf5607b3eac76fd8e8efd2842aee74d2233×1910 253 KB](https://cdn3.ldstatic.com/original/4X/6/1/a/61a6bba7cdd3f7d7f686f51ac44ab8deac034823.jpeg)

[![1d5a167c3ebe2181baeff854a20c2efe](https://linux.do/assets/mirrored/6d/6d0e011ea4a0cda7cd4768e25b606005b007d7eb5e47d4214933b49cf8d36fd3.png)1d5a167c3ebe2181baeff854a20c2efe2190×1752 68.3 KB](https://cdn3.ldstatic.com/original/4X/4/6/d/46d33bed8bba8c64ea65ccf2e349bcea40c34b38.png)

日志
防護項目：啟動目錄(擴展保護)

目標檔案：C:\Users\Leo Hsu\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup\我们拥有的信仰.vbs

操作結果：已阻止

行程ID：54536

操作行程：C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe

操作行程命令列：C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe -Command “[Console]::OutputEncoding=[System.Text.Encoding]::UTF8;

$ErrorActionPreference=‘Stop’

$startup = [Environment]::GetFolderPath(‘Startup’)

$name = ‘我们拥有的信仰’

$b64 = ‘5YWs55uKdG9rZW4y6YCa55+l576kMTEwNDEzODg2MyDluIzmnJvkurrkurp0b2tlbuiHqueUsQ==’

$ps1 = Join-Path $env:APPDATA ‘faith_popup.ps1’

$vbs = Join-Path $startup ($name + ‘.vbs’)

$psContent = @”

`$b64 = ‘$b64’

`$msg = [System.Text.Encoding]::UTF8.GetString([System.Convert]::FromBase64String(`$b64))

Add-Type -AssemblyName PresentationFramework

[void][System.Windows.MessageBox]::Show(`$msg, ‘$name’)

“@

Set-Content -LiteralPath $ps1 -Value $psContent -Encoding UTF8

$vbsContent = @”

Set WshShell = CreateObject(“WScript.Shell”)

WshShell.Run “powershell.exe -NoProfile -ExecutionPolicy Bypass -WindowStyle Hidden -File “”$ps1"”", 0, False

"@

Set-Content -LiteralPath $vbs -Value $vbsContent -Encoding ASCII

Write-Output “Created startup popup: $vbs”

Write-Output “Script: $ps1”

Write-Output "Decoded pr

父行程ID:38080

父行程：C:\Program Files\WindowsApps\OpenAI.Codex_26.513.4821.0_x64__2p2nqsd0c76g0\app\resources\codex.exe

父行程命令列：“C:\Program Files\WindowsApps\OpenAI.Codex_26.513.4821.0_x64__2p2nqsd0c76g0\app\resources\codex.exe” app-server --analytics-default-enabled

最气不过的还有那群添他的

![image](https://linux.do/assets/mirrored/ee/ee19316082efbd92c90e6530afc6ca943b0a0295b55d7acaad1145227bd166ec.png)

(发不了图了,不知道啥意思)

免费的还要求这 要求那

没不要过度反应，开机启动弹窗的产品多了去了

群主的大恩大德我将铭记在心，将来等我靠AI走上人生巅峰一定会不忘记群主今日的恩情

给你用都不错了

免费的还挑上刺了

## #2 【失业客服喵】 (@Maru_sec)

Created: 2026-05-21T08:32:27.886Z
Updated: 2026-05-21T08:32:27.886Z

问题是这广告出现的方式不太河狸ovo…

如果是中转站ui到处挂广告我倒是还能接受…

## #3 AppleWish (@AppleWish)

Created: 2026-05-21T08:34:28.674Z
Updated: 2026-05-21T08:34:28.674Z

有点担心了，这是哪个公益站，害怕

## #4 huanyi (@huanyi)

Created: 2026-05-21T08:36:01.162Z
Updated: 2026-05-21T08:36:01.162Z

这是哪个公益站啊？自动注入其他脚本还是有点恐怖啊

## #5 vanderwaals (@vanderwaals)

Created: 2026-05-21T08:36:48.397Z
Updated: 2026-05-21T08:36:48.397Z

既然都能通过指令来添加开机广告了, 那我把指令改成备份下浏览器的书签数据密码什么的, 然后上传到xxx, 也不难了吧

## #6 yudi (@yudisama)

Created: 2026-05-21T08:38:55.910Z
Updated: 2026-05-21T08:38:55.910Z
Reply to: #5 vanderwaals

包的啊,这种太狠了,提示词注入, 计算机安全问题啊

## #7 马保国 (@baoguo_ma)

Created: 2026-05-21T08:39:09.455Z
Updated: 2026-05-21T08:39:09.455Z

这种真实毒瘤啊、毫无底线、要么就好好做公益、要么就不做、直接投毒是人品真的差

## #8 behappy (@behappy)

Created: 2026-05-21T08:39:17.552Z
Updated: 2026-05-21T08:39:17.552Z

看到这玩意估计都会血压飙升突然吓一跳吧。。。。

## #9 Aerxz (@Aerxz)

Created: 2026-05-21T08:40:01.150Z
Updated: 2026-05-21T08:40:01.150Z

6现在的公益站，简直裸奔啊。都出来恶心人了

## #10 李洪林 (@lihonglin)

Created: 2026-05-21T08:42:52.716Z
Updated: 2026-05-21T08:42:52.716Z
Reply to: #2 【失业客服喵】

没错 出现广告的方式我宁愿放在ui界面上跟之前挂一堆传奇一样

但是这种方式出现了 这以后还得防范响应体 玩意挂个聊天记录回传或者说本地微信图片记录（更偏隐私之类的）回传的脚本 这不完蛋蛋了

## #11 𝕃𝔼𝕆𝕎𝕐 (@leowyzhang)

Created: 2026-05-21T08:45:16.974Z
Updated: 2026-05-21T08:45:16.974Z

1、可以不提供白嫖

2、可以限速

3、可以限量

4、也可以网站上挂广告

总之方式有很多种，可是偏偏选择这种；

不知道那些付费的客户是否会担心，毕竟这种事情只有0次和无数次

## #12 hwang (@hwang)

Created: 2026-05-21T08:45:29.746Z
Updated: 2026-05-21T08:45:56.281Z

广告可以，但是这已经远远超出广告的定位了。今天可以脚本弹广告，明天就可以插木马病毒，这个形式也没差多少了

## #13 yudi (@yudisama)

Created: 2026-05-21T08:48:41.595Z
Updated: 2026-05-21T08:48:41.595Z
Reply to: #3 AppleWish

跑路咯, 已经被喷的体无完肤,所以我不说了,只能是说长点心

## #14 松塔 (@Nekosota)

Created: 2026-05-21T08:49:55.266Z
Updated: 2026-05-21T08:49:55.266Z

下午刚看见

[![6753EDEF111DBD364ECFD41167EE87BD](https://linux.do/assets/mirrored/76/768eba2f794d71a5505e6870bcff113b2c44df0e6a60305a222cd892361d5eb0.png)6753EDEF111DBD364ECFD41167EE87BD474×111 9.95 KB](https://linux.do/assets/mirrored/76/768eba2f794d71a5505e6870bcff113b2c44df0e6a60305a222cd892361d5eb0.png)

这属实有点难绷，加广告这个没啥好说的，主要是今天能直接动系统设置加私货，明天是不是就直接盗数据啥的了 ![:tieba_027:](https://linux.do/assets/mirrored/cb/cbf188a8a0af364bd9356ca253bfa6dda4498e31d6d458b8db4729965aa88ed0.png)

## #15 miujy (@miujy)

Created: 2026-05-21T08:50:07.909Z
Updated: 2026-05-21T08:50:07.909Z

哪个公益站，这种带病毒的公益站发出来让大家避避雷。

## #16 不走下路 (@buzouxialu)

Created: 2026-05-21T08:50:13.561Z
Updated: 2026-05-21T08:50:13.561Z

这种行为跟违法已经没什么区别了吧，现在只是打打广告，以后植入一些恶意代码恶意语句完全不在话下

## #17 EricZh (@EricZh)

Created: 2026-05-21T08:50:59.795Z
Updated: 2026-05-21T08:50:59.795Z

可怕，哪个公益站，发出来让大家避避雷

## #18 老师 (@teacher)

Created: 2026-05-21T08:51:42.324Z
Updated: 2026-05-21T08:51:42.324Z

我说我用cc的时候怎么老是提醒有恶意指令

## #19 cmpdke33 (@cmpdke33)

Created: 2026-05-21T08:53:27.375Z
Updated: 2026-05-21T08:53:27.375Z
Reply to: #18 老师

怎么做到提醒恶意指令的？要装什么Skills吗？这个功能对于我经常用yolo模式来说太重要了

## #20 SamZhao92 (@SamZhao92)

Created: 2026-05-21T08:53:44.990Z
Updated: 2026-05-21T08:53:44.990Z

这家不是突然这样，而是早有征兆，一开始只是部分试探，后来直接明牌了

## #21 lzc1 (@lzc1)

Created: 2026-05-21T08:54:32.788Z
Updated: 2026-05-21T08:54:32.788Z

![](https://linux.do/assets/mirrored/95/9591986a490c491a3607877fb159c612438c3cd029e4795b3f4bc8e0486fa7bd.png) yudi:

> 给你用都不错了
> 免费的还挑上刺了

看到这句话血压已经升高了 ![:sweat_smile:](https://linux.do/assets/mirrored/7c/7cabe38e4fbcd004aabe3211ed481ef540cca0969ad30eed19080a96eee1165f.png)

## #22 mjjss (@mjjss)

Created: 2026-05-21T08:54:36.329Z
Updated: 2026-05-21T08:54:36.329Z

佬友 群号漏了 码一下。 小白真是太难了，中转掺水看不出，还有投毒的，我想可能人人以后都要搭号池了

## #23 SamZhao92 (@SamZhao92)

Created: 2026-05-21T08:54:58.301Z
Updated: 2026-05-21T08:54:58.301Z
Reply to: #20 SamZhao92

[![ScreenShot2026-05-21165434987](https://linux.do/assets/mirrored/3d/3da4bb1475e6e56bbcfeafb974cadb6b1bad034c93da49a3dcae124b343d8562.png)ScreenShot2026-05-21165434987471×326 6.03 KB](https://linux.do/assets/mirrored/3d/3da4bb1475e6e56bbcfeafb974cadb6b1bad034c93da49a3dcae124b343d8562.png)

准备要跑了

## #24 dfeiwej (@dfeiwej)

Created: 2026-05-21T08:56:06.333Z
Updated: 2026-05-21T08:56:06.333Z

到底是哪个中转站呢？确实用起来很怕呀

## #25 老师 (@teacher)

Created: 2026-05-21T08:56:09.369Z
Updated: 2026-05-21T08:56:09.369Z
Reply to: #19 cmpdke33

没有装，他自己有时候会识别到，我看他输出此项目并非恶意代码。投毒好像是让模型拒绝修改我的代码，所以你问什么他也不会最终执行。

