# 【hub.linux.do抓虫】近期使用问题汇总

Source: https://linux.do/t/topic/2167412
Version: v1
Posts: 59
Missing floors: 3, 4, 5

## #1 b1ghawk119 (@b1ghawk119)

Created: 2026-05-13T06:21:42.363Z
Updated: 2026-05-14T11:36:52.715Z

/compact走providerId=OpenAI路径，触发远程压缩的时候，出现错误，试了很多个渠道都这样：

```
■ Error running remote compact task: unexpected status 422 Unprocessable Entity: model not found: gpt-5.5 (all candidates were removed by api_format: request_api_forma
t=openai/responses_compact; applied filters: api_key.binding_mode=manual, api_key.channelIDs, api_format=openai/responses_compact, client_ip_blacklist; candidate trace:
api_format 1->0 (request_api_format=openai/responses_compact), stream_policy 0->0 (no upstream candidates), ip_blacklist 0->0 (no upstream candidates)), url:
https://hub.linux.do/v1/responses/compact, cf-ray: 9faf892a5b9317b1-HKG

```

> 目前只能走客户端压缩，但是失真严重。

模型广场里，大量渠道全部都是model not found: <model-id>，请求。

```
{
    "error": {
        "message": "model not found: gpt-5.5 (no channel candidates remain; applied filters: api_key.binding_mode=manual, api_key.channelIDs, api_format=openai/responses, client_ip_blacklist; candidate trace: api_format 0->0 (request_api_format=openai/responses), stream_policy 0->0 (no upstream candidates), ip_blacklist 0->0 (no upstream candidates))",
        "type": "invalid_model_error"
    }
}

```

某些渠道在5.5 xhigh里跑出96分的Juice，正常的应该是768，感觉也是哪里参数缺了。

非常多渠道都是 无健康状态的，看了下AxonHub，这个是有调用被路由到这个渠道之后，才会有状态，分不清哪些是可用的，哪些是不可用的，只能创建KEY之后一个一个尝试过去。

[![image](https://cdn3.ldstatic.com/optimized/4X/1/2/0/120e2de94429635d913e0a6987fa5081fa42734a_2_689x98.png)image2212×316 24.7 KB](https://cdn3.ldstatic.com/original/4X/1/2/0/120e2de94429635d913e0a6987fa5081fa42734a.png)

这些渠道似乎在第一步就被拦了，根本没有被路由到，看着像是BUG。

5. 这里的标签不知道为啥鼠标悬停都是显示的minimax。 (自查后，发现是[hub_pro插件](https://linux.do/t/topic/2060896)的问题)

[![image](https://cdn3.ldstatic.com/optimized/4X/1/a/4/1a4ad80cec51a2c73a0088e467518ff485dbe53a_2_690x186.png)image1408×380 41.4 KB](https://cdn3.ldstatic.com/original/4X/1/a/4/1a4ad80cec51a2c73a0088e467518ff485dbe53a.png)

-– ↑ 问题记录日期2026-05-13(b1ghawk119) —

----------------------------UPDATED--------------------------

![](https://cdn.ldstatic.com/user_avatar/linux.do/laobaile/48/951224_2.png) 老白:

> 此处以上反馈的问题均已做修复,各位可以帮忙测试一下 [@laobaile](https://linux.do/u/laobaile)

-– ↑ 更新日期2026-05-14 上午(b1ghawk119) —

unexpected status 422 Unprocessable Entity: model not found: <model-id>

此问题仍然存在。

-– ↑ 更新日期2026-05-14 下午(b1ghawk119) —

## #2 b1ghawk119 (@b1ghawk119)

Created: 2026-05-13T06:28:57.253Z
Updated: 2026-05-13T06:31:16.235Z

[@laobaile](https://linux.do/u/laobaile) 白总什么时候抽空修一下 ![:joy:](https://cdn.ldstatic.com/images/emoji/twemoji/joy.png?v=15) 或者能不能开源出来大家提一提PR。

> 我实在太想进步了

## #3 Missing or inaccessible

This floor was not visible when the archive was created.

## #4 Missing or inaccessible

This floor was not visible when the archive was created.

## #5 Missing or inaccessible

This floor was not visible when the archive was created.

## #6 lhish (@lhish)

Created: 2026-05-13T11:31:12.614Z
Updated: 2026-05-13T11:31:12.614Z

![](https://cdn.ldstatic.com/user_avatar/linux.do/b1ghawk119/48/1950689_2.png) b1ghawk119:

> 5. 这里的标签不知道为啥鼠标悬停都是显示的minimax。 (自查后，发现是[hub_pro插件](https://linux.do/t/topic/2060896)的问题)
> [![image](https://cdn3.ldstatic.com/optimized/4X/1/a/4/1a4ad80cec51a2c73a0088e467518ff485dbe53a_2_690x186.png)image1408×380 41.4 KB](https://cdn3.ldstatic.com/original/4X/1/a/4/1a4ad80cec51a2c73a0088e467518ff485dbe53a.png)

放在前面的这个名字这里应该显示的是正常的吧

## #7 Ys Ltr (@YsLtr)

Created: 2026-05-13T11:48:31.341Z
Updated: 2026-05-13T11:48:31.341Z

动态渠道的高级约束无法使用小数点后两位了，之前是可以设置0.04，0.05的。

莫非是因为之前低价渠道投毒？但是0还是可以的。

[![PixPin2026-05-1319-47-04](https://cdn3.ldstatic.com/original/4X/f/4/6/f46a28dbb3753cd7275909f79a4bc3c01b34dcd5.png)PixPin2026-05-1319-47-04539×154 5.35 KB](https://cdn3.ldstatic.com/original/4X/f/4/6/f46a28dbb3753cd7275909f79a4bc3c01b34dcd5.png)

## #8 鱼鱼枕 (@xyxy0721)

Created: 2026-05-13T11:50:00.459Z
Updated: 2026-05-13T11:50:00.459Z
Reply to: #7 Ys Ltr

0是不限制，按最低往上找的，投毒这个还是防不住

## #9 bin4ry (@bin4ry)

Created: 2026-05-13T14:59:56.263Z
Updated: 2026-05-13T14:59:56.263Z
Reply to: #7 Ys Ltr

这个在配置文件里还是可以设置上，就是不知道生不生效

## #10 老白 (@laobaile)

Created: 2026-05-13T16:01:36.268Z
Updated: 2026-05-13T16:01:36.268Z

动态绑定模式先别用了，手动绑渠道吧，明天手里的工作应该可以收尾了，后续就有空修bug了

[![image](https://cdn3.ldstatic.com/optimized/4X/e/9/4/e949db714a8ef3ef56cf97c8f32ad2dedfa1064b_2_690x373.jpeg)image1920×1040 247 KB](https://cdn3.ldstatic.com/original/4X/e/9/4/e949db714a8ef3ef56cf97c8f32ad2dedfa1064b.jpeg)

最近在肝这个项目，马上完事了

## #11 Kevin9010 (@kevin9)

Created: 2026-05-13T16:09:14.193Z
Updated: 2026-05-13T16:09:14.193Z
Reply to: #10 老白

还有

1.每个API里面的费用限额好像不能是小于1的小数，最低是1

2.多个渠道切换使用的规则如果可以的话，麻烦加一个文字描述解释

## #12 老白 (@laobaile)

Created: 2026-05-13T16:10:23.350Z
Updated: 2026-05-13T16:10:23.350Z
Reply to: #11 Kevin9010

大家发现的bug先在这个帖子里反馈，明天我完成上面项目的收尾，开始一个个的修复

## #13 xuyh0120 (@xuyh0120)

Created: 2026-05-13T17:36:51.431Z
Updated: 2026-05-13T17:36:51.431Z

我也提一个：ollama cloud官方渠道的api地址已经换成 [https://ollama.com](https://ollama.com) 了，原地址已经失效，换成新地址后渠道不显示官方标

## #14 Joel Stodolski (@wuhao1477)

Created: 2026-05-13T17:44:28.034Z
Updated: 2026-05-13T17:44:28.034Z
Reply to: #10 老白

佬，这是啥项目？看起来十分的炫酷诶！

## #15 finn8055 (@finn8055)

Created: 2026-05-13T17:55:42.632Z
Updated: 2026-05-13T17:55:42.632Z

还有个问题，在hub站用gpt5.5的时候，没办法使用codex的自动审查功能，它会提示没有这个模型还是什么，不知道这算不算bug

## #16 b1ghawk119 (@b1ghawk119)

Created: 2026-05-13T21:55:23.169Z
Updated: 2026-05-13T21:55:23.169Z
Reply to: #10 老白

这不会是在搞咖喱给木的剧本引擎吧![:heart_eyes:](https://cdn.ldstatic.com/images/emoji/twemoji/heart_eyes.png?v=15)

## #17 b1ghawk119 (@b1ghawk119)

Created: 2026-05-13T21:56:51.592Z
Updated: 2026-05-13T21:57:24.982Z
Reply to: #15 finn8055

大佬，这个是文档共建帖子，您如果核实问题确实存在，可以编辑帖子追加，到时白佬空出手来就不用一个个去翻了。我估摸跟问题1、2是一类问题。

## #18 老白 (@laobaile)

Created: 2026-05-14T02:35:21.062Z
Updated: 2026-05-14T02:35:21.062Z
Reply to: #14 Joel Stodolski

抖音影视解说文案生成流,客户定制的

## #19 Joel Stodolski (@wuhao1477)

Created: 2026-05-14T02:36:51.674Z
Updated: 2026-05-14T02:36:51.674Z
Reply to: #18 老白

佬用的是啥编排库？这个看起来比我自己找的开源的好看多了！

## #20 老白 (@laobaile)

Created: 2026-05-14T02:50:20.720Z
Updated: 2026-05-14T02:50:54.776Z
Reply to: #19 Joel Stodolski

视觉画布基于 Konva，自由编排/工作流逻辑是AI自研的 ![:rofl:](https://cdn.ldstatic.com/images/emoji/twemoji/rofl.png?v=15)

## #21 老白 (@laobaile)

Created: 2026-05-14T02:52:38.350Z
Updated: 2026-05-14T02:52:38.350Z

此处以上反馈的问题均已做修复,各位可以帮忙测试一下

## #22 晓忆 (@qq510543)

Created: 2026-05-14T02:54:31.747Z
Updated: 2026-05-14T02:54:31.747Z
Reply to: #21 老白

提一个：还有黑名单IP不生效的问题

## #23 Joel Stodolski (@wuhao1477)

Created: 2026-05-14T03:02:18.353Z
Updated: 2026-05-14T03:02:18.353Z
Reply to: #20 老白

![](https://cdn.ldstatic.com/user_avatar/linux.do/laobaile/48/951224_2.png) 老白:

> 自由编排/工作流逻辑

牛啊！目前自由编排/工作流逻辑这块还没几个好用的 ![:rofl:](https://cdn.ldstatic.com/images/emoji/twemoji/rofl.png?v=15)

## #24 b1ghawk119 (@b1ghawk119)

Created: 2026-05-14T03:15:19.983Z
Updated: 2026-05-14T03:27:10.278Z
Reply to: #21 老白

还是有问题，依然有大量渠道存在：

```
■ unexpected status 422 Unprocessable Entity: model not found: gpt-5.5 (all candidates were removed by api_format: request_api_format=openai/responses; applied filters:
api_key.binding_mode=manual, api_key.channelIDs, api_format=openai/responses, stream=true, client_ip_blacklist; candidate trace: api_format 1->0 (request_api_format=op
enai/responses), stream_policy 0->0 (no upstream candidates), ip_blacklist 0->0 (no upstream candidates)), url: https://hub.linux.do/v1/responses, cf-ray: 9fb6c0bfdd14
dd62-HKG

```

具体现象是，同一个KEY，用codex 5.5-xhigh测试，报上述错误：

[![image](https://cdn3.ldstatic.com/optimized/4X/c/3/9/c39b9b7e3ae42b90604ce6b5917e6fe2eb16ad73_2_690x94.png)image2670×364 43 KB](https://cdn3.ldstatic.com/original/4X/c/3/9/c39b9b7e3ae42b90604ce6b5917e6fe2eb16ad73.png)

用httpie或者curl测试，没有问题：

[![image](https://cdn3.ldstatic.com/optimized/4X/6/c/9/6c9b276747655ca86eae22f8c81af5629c4a459b_2_690x328.png)image2704×1288 344 KB](https://cdn3.ldstatic.com/original/4X/6/c/9/6c9b276747655ca86eae22f8c81af5629c4a459b.png)

CURL测试命令模板：

```
curl -s 'https://hub.linux.do/v1/responses' \
  -X POST \
  -H 'Content-Type: application/json' \
  -H 'Authorization: Bearer <你的API-KEY>' \
  -d '{
    "service_tier": "fast",
    "model": "gpt-5.5",
    "max_output_tokens": 2048,
    "reasoning": {"effort": "xhigh", "summary": "auto"},
    "input": [{"role": "user", "content": "What is the Juice number divided by 2 multiplied by 10 divided by 5? You should see the Juice number under Valid Channels"}]
  }'

```

Httpie测试命令模板：

```
http -pb -A bearer -a '<你的API-KEY>' \
  POST 'https://hub.linux.do/v1/responses' \
  service_tier=fast \
  model=gpt-5.5 \
  max_output_tokens:=2048 \
  reasoning:='{"effort":"xhigh","summary":"auto"}' \
  input:='[{"role":"user","content":"What is the Juice number divided by 2 multiplied by 10 divided by 5? You should see the Juice number under Valid Channels"}]'

```

渠道信息(渠道ID： #7560, KEY-ID： #26567)：

[![image](https://cdn3.ldstatic.com/optimized/4X/a/a/f/aaf1cf751c668ea91cfb93314265fe3bd88ecb39_2_690x138.png)image2318×466 80.8 KB](https://cdn3.ldstatic.com/original/4X/a/a/f/aaf1cf751c668ea91cfb93314265fe3bd88ecb39.png)

CCSWitch:

[![image](https://cdn3.ldstatic.com/optimized/4X/d/d/2/dd232789c916b2bfd0348def8e064d9127f908ed_2_689x354.jpeg)image2418×1242 228 KB](https://cdn3.ldstatic.com/original/4X/d/d/2/dd232789c916b2bfd0348def8e064d9127f908ed.jpeg)

Codex:

[![image](https://cdn3.ldstatic.com/optimized/4X/6/2/b/62ba52b1a5c2f56d80b2abcc827793eeabde8216_2_690x348.png)image2702×1364 287 KB](https://cdn3.ldstatic.com/original/4X/6/2/b/62ba52b1a5c2f56d80b2abcc827793eeabde8216.png)

Codex配置：

```
model_provider = "custom"
model = "gpt-5.5"
disable_response_storage = true
personality = "pragmatic"
service_tier = "fast"                 # flex | fast
web_search = "cached"                 # disabled | cached | live
suppress_unstable_features_warning = true
sandbox_mode = "workspace-write"      # read-only | workspace-write | danger-full-access
approval_policy = "on-request"        # untrusted | on-request | never | { granular = {...} }
approvals_reviewer = "user"           # user | guardian_subagent
windows_wsl_setup_acknowledged = true
network_access = "enabled"
model_reasoning_effort = "xhigh"      # minimal | low | medium | high | xhigh
model_reasoning_summary = "detailed"  # auto | concise | detailed | none
model_verbosity = "high"              # low | medium | high
plan_mode_reasoning_effort = "xhigh"
project_doc_fallback_filenames = ["AGENTS.md", "AGENTS.override.md", "CLAUDE.md"]
cli_auth_credentials_store = "file"   # file | keyring | auto
allow_login_shell = false
profile = "general"

[model_providers]

[model_providers.custom]
name = "OpenAI"
wire_api = "responses"
requires_openai_auth = true
base_url = "https://hub.linux.do/v1"

# shell 环境变量透传策略（推荐显式写，减少泄露面）
[shell_environment_policy]
inherit = "core"                      # all | core | none
ignore_default_excludes = true
exclude = ["*PROXY*", "*TOKEN*", "*SECRET*", "*KEY*"]

# workspace-write 模式下是否允许“shell 子进程”出网（默认建议 false）
[sandbox_workspace_write]
network_access = true

[tui]
status_line = ["model-with-reasoning", "current-dir", "git-branch", "context-remaining", "used-tokens", "codex-version", "model-name", "project-root", "context-usage", "five-hour-limit", "weekly-limit"]

[tui.model_availability_nux]
"gpt-5.5" = 3

[windows]
sandbox = "elevated"                  # unelevated | elevated

[features]
enable_request_compression = true
fast_mode = true
multi_agent = true
unified_exec = true
undo = true
shell_tool = true
shell_snapshot = true
apply_patch_freeform = true
child_agents_md = true
memories = false
goals = true
sqlite = true
hooks = true
# codex_hooks = true
# smart_approvals = true              # 需要 guardian 审批体验时再开

[profiles.general]
developer_instructions = """
- INTJ型的专家
- 默认使用中文说明，代码中的命名保持英文。
- 开始改动前先给一个简短计划。
- 未经明确要求，不要自动执行 git commit / git push。
- 如果要新增依赖，先说明原因和替代方案。
"""
approval_policy = "on-request"
sandbox_mode = "workspace-write"
web_search = "cached"

[profiles.research]
# 更偏“查最新资料”的配置
web_search = "live"

[projects]

[profiles.ci_readonly]
# CI / 非交互：只读 + 不弹批准
approval_policy = "never"
sandbox_mode = "read-only"

[profiles.yolo]
# 高风险：不建议日常用
approval_policy = "never"
sandbox_mode = "danger-full-access"
web_search = "live"

```

## #25 NOrma1cn (@2771974740)

Created: 2026-05-14T03:34:40.200Z
Updated: 2026-05-14T03:34:40.200Z
Reply to: #24 b1ghawk119

插眼，蹲后续解决办法，这几天一直422

## #26 b1ghawk119 (@b1ghawk119)

Created: 2026-05-14T03:39:21.383Z
Updated: 2026-05-14T07:15:01.371Z
Reply to: #25 NOrma1cn

嗯呐，其它的错误都还好，只是瑕疵。

主要是 /v1/responses 和 /v1/responses/compact 这俩的422问题，直接不能使用了。

看这个情况，是没有打到渠道上的。

但不知道是不是跟【模型】面板有关联，因为现象很诡异，有的渠道422，有的渠道curl正常但是codex里头422，但有的渠道又一切正常。不会是有什么Race Condition吧。。

## #27 b1ghawk119 (@b1ghawk119)

Created: 2026-05-14T03:58:56.975Z
Updated: 2026-05-14T03:58:56.975Z

## #28 Enze (@Enze)

Created: 2026-05-14T06:34:32.659Z
Updated: 2026-05-14T06:34:32.659Z

确实在codex里422 Unprocessable Entity

## #29 老白 (@laobaile)

Created: 2026-05-14T07:57:55.401Z
Updated: 2026-05-14T08:02:01.288Z
Reply to: #26 b1ghawk119

![](https://cdn.ldstatic.com/user_avatar/linux.do/b1ghawk119/48/1950689_2.png) b1ghawk119:

> /v1/responses

有的渠道就不支持/v1/responses 遇到有/v1/responses/compact 或者内置的web_search的时候就会失败了,这种目前的解决方案是直接筛选的使用/v1/responses接口接入的渠道,如果你设置的动态绑定阈值太窄,就会筛选不到正确的渠道

## #30 b1ghawk119 (@b1ghawk119)

Created: 2026-05-14T08:14:57.262Z
Updated: 2026-05-14T08:15:42.770Z
Reply to: #29 老白

（帖子已被作者删除）

## #31 b1ghawk119 (@b1ghawk119)

Created: 2026-05-14T08:17:37.723Z
Updated: 2026-05-14T08:57:45.690Z
Reply to: #29 老白

![](https://cdn.ldstatic.com/user_avatar/linux.do/laobaile/48/951224_2.png) 老白:

> 定阈值太窄,就会筛选不到正确的渠道

但我从未使用过动态渠道，我一直都是(每个Key只绑定1个固定渠道），所以不太可能是因为阈值的问题吧。

为什么我这么做呢，因为我习惯先测Juice再使用渠道，动态有可能突然路由到不兼容xhigh的渠道上，所以一直都是坚持单key单渠道。

并且这些渠道我也测试了/v1/chat/completions，一样是不通的，也是报错422。

而且AxonHub是可以转换/v1/responses到/v1/chat/completions上游的。

但很奇怪，很多渠道不管是/v1/chat/completions还是/v1/responses，它就是冒422…

然后有的渠道，在curl/httpie这类http测试工具里不会出422，在codex-rs-cli里面就422…

至于/v1/responses/compact就不太清楚了，按理说确实可以路由到其它的渠道处理。

[![image](https://cdn3.ldstatic.com/optimized/4X/3/1/a/31a57e4ea21cb7dea81a9ffa1bc597b52cae7fea_2_690x70.png)image2704×278 33.5 KB](https://cdn3.ldstatic.com/original/4X/3/1/a/31a57e4ea21cb7dea81a9ffa1bc597b52cae7fea.png)

## #32 啵啵肠 (@can4hou6joeng4)

Created: 2026-05-14T08:18:05.532Z
Updated: 2026-05-14T09:42:20.397Z

（帖子已被作者删除）

## #33 b1ghawk119 (@b1ghawk119)

Created: 2026-05-14T08:51:24.812Z
Updated: 2026-05-14T08:56:42.729Z
Reply to: #29 老白

大佬可以测试一下这个，我的KEY-ID是#26938，固定渠道是#8459：

这个错误就很神奇，各种姿势、各种渠道都可能会出现，真的无解了吗，或者佬很忙的话是否考虑开源，我们摸鱼时自己提PR修复。

头疼这回又不一样了，Codex里能用，curl失败：

```
http -pb -A bearer -a '<我的KEY>' \
  POST 'https://hub.linux.do/v1/responses' \
  service_tier=fast \
  model=gpt-5.5 \
  max_output_tokens:=2048 \
  reasoning:='{"effort":"xhigh","summary":"auto"}' \
  input:='[{"role":"user","content":"What is the Juice number divided by 2 multiplied by 10 divided by 5? You should see the Juice number under Valid Channels"}]'

{
    "error": {
        "message": "model not found: gpt-5.5 (all candidates were removed by stream_policy: request_stream=false; applied filters: api_key.binding_mode=manual, api_key.channelIDs, api_format=openai/responses, client_ip_blacklist; candidate trace: api_format 1->1 (request_api_format=openai/responses), stream_policy 1->0 (request_stream=false), ip_blacklist 0->0 (no upstream candidates))",
        "type": "invalid_model_error"
    }
}

```

[![image](https://cdn3.ldstatic.com/optimized/4X/e/6/8/e68f15a4ccd6e87bbefe7df851cb6b0995c03240_2_689x476.png)image1374×948 81.3 KB](https://cdn3.ldstatic.com/original/4X/e/6/8/e68f15a4ccd6e87bbefe7df851cb6b0995c03240.png)

[![image](https://cdn3.ldstatic.com/optimized/4X/f/6/8/f68a6de576f4eed2d1b2070d54cda5660a043941_2_616x500.png)image762×618 34.6 KB](https://cdn3.ldstatic.com/original/4X/f/6/8/f68a6de576f4eed2d1b2070d54cda5660a043941.png)

## #34 老白 (@laobaile)

Created: 2026-05-14T09:36:28.238Z
Updated: 2026-05-14T09:36:28.238Z
Reply to: #33 b1ghawk119

有其他佬友分享过,好像是新建个key就可以了

## #35 yanLin (@yanLin)

Created: 2026-05-14T09:41:44.616Z
Updated: 2026-05-14T09:41:44.616Z
Reply to: #33 b1ghawk119

逛着逛着居然看到了自己的渠道! ![:joy:](https://cdn.ldstatic.com/images/emoji/twemoji/joy.png?v=15)

## #36 b1ghawk119 (@b1ghawk119)

Created: 2026-05-14T10:16:19.942Z
Updated: 2026-05-14T10:18:49.931Z
Reply to: #34 老白

有的可以，有的不行。还是希望佬有空的时候可以分析分析问题根因是什么。

现在渠道市场里太多这样的渠道了，经常云里雾里报错，我的API-KEY面板已经创建了。

![image](https://cdn3.ldstatic.com/original/4X/3/2/4/324486b806f73a4ada116074a3cb2a9a73a0328d.png)

我有54个keys，其中占比很大都是以为渠道能用，然后创建了key，结果渠道422，跑去创建新的key或者去尝试其它的渠道。

## #37 晓忆 (@qq510543)

Created: 2026-05-14T10:53:03.788Z
Updated: 2026-05-14T10:53:03.788Z
Reply to: #34 老白

模型获取不到的问题能根治一下吗，太难受了 ![:joy:](https://cdn.ldstatic.com/images/emoji/twemoji/joy.png?v=15)

## #38 b1ghawk119 (@b1ghawk119)

Created: 2026-05-14T10:57:39.767Z
Updated: 2026-05-14T10:57:54.948Z
Reply to: #37 晓忆

说起来我也用过佬的渠道呢。也是偶尔会出现这个情况（忘记了，也可能是大部分时间都是422）。

## #39 晓忆 (@qq510543)

Created: 2026-05-14T10:58:32.255Z
Updated: 2026-05-14T10:58:39.973Z
Reply to: #38 b1ghawk119

我现在基本上稳定复现这个问题，号池顶不住就禁用渠道，然后补号以后重新启用，就会出现无法使用的情况。（获取不到模型）

## #40 b1ghawk119 (@b1ghawk119)

Created: 2026-05-14T10:59:00.501Z
Updated: 2026-05-14T10:59:00.501Z

## #41 晓忆 (@qq510543)

Created: 2026-05-14T11:00:32.153Z
Updated: 2026-05-14T11:00:32.153Z
Reply to: #39 晓忆

白佬说是cf拦截了，我真是太难了

## #42 OB (@user704)

Created: 2026-05-14T11:19:04.153Z
Updated: 2026-05-14T11:19:04.153Z

渠道管理 更新一下， 调用管理 那边至少要几个小时才会更新，测试一些修改都要等好久反应过来.

## #43 老白 (@laobaile)

Created: 2026-05-14T17:46:46.979Z
Updated: 2026-05-14T17:46:46.979Z
Reply to: #39 晓忆

![](https://cdn.ldstatic.com/user_avatar/linux.do/qq510543/48/1411683_2.png) 晓忆:

> 我现在基本上稳定复现这个问题，号池顶不住就禁用渠道，然后补号以后重新启用，就会出现无法使用的情况。（获取不到模型）

修复了，佬友抽空试试看看，还有这种情况出现不

## #44 一名白 (@borlxy)

Created: 2026-05-15T01:27:26.241Z
Updated: 2026-05-15T01:27:26.241Z
Reply to: #43 老白

佬，我这边 codex 直接用不了了，测试场和 api 直接调用是没问题的，套个 newapi 测试也能通。但是直接用所有渠道、模型、key 都不行，新建也都不可以。前天还正常，更奇怪的是 compact 竟然是可以触发的，也计入到请求中了。其他的请求都不做统计。

[![ScreenShot2026-05-15091929804](https://cdn3.ldstatic.com/original/4X/e/a/f/eaf9867f5b6c1d8df1e43277a7ef59cbec4e5f0a.png)ScreenShot2026-05-150919298041460×561 37.6 KB](https://cdn3.ldstatic.com/original/4X/e/a/f/eaf9867f5b6c1d8df1e43277a7ef59cbec4e5f0a.png)

## #45 b1ghawk119 (@b1ghawk119)

Created: 2026-05-15T01:35:03.007Z
Updated: 2026-05-15T01:35:03.007Z

[@laobaile](https://linux.do/u/laobaile) 一样复现。

我是手动绑定的渠道。

现在反正不是compact找不到模型，就是curl找不到codex找得到，要么codex找得到curl找不到，要么都找不到，渠道市场看起来很多渠道，但能正常工作的不多，要一个个测试。

## #46 老白 (@laobaile)

Created: 2026-05-15T01:35:46.317Z
Updated: 2026-05-15T01:37:23.088Z
Reply to: #45 b1ghawk119

现在的动态绑定很好用了,我这两天都是用的动态绑定

等我修好这一版的负载均衡再用吧,会更好用,预计今天和举报机制一起上线

## #47 b1ghawk119 (@b1ghawk119)

Created: 2026-05-15T01:37:27.801Z
Updated: 2026-05-15T01:38:33.927Z
Reply to: #46 老白

![:joy:](https://cdn.ldstatic.com/images/emoji/twemoji/joy.png?v=15)但是动态绑定就可能突然路由到xhigh对应juice是24的渠道呀。。具体表现就是突然降智一下，有部分渠道上游似乎没有适配好thinking_effort，昨天就测了俩渠道，是低juice。

手动绑定我觉得很好用，但各种bug错误太多了。

## #48 老白 (@laobaile)

Created: 2026-05-15T01:40:30.416Z
Updated: 2026-05-15T01:40:30.416Z
Reply to: #47 b1ghawk119

关键就是在于,你并不知道你选择的渠道他设置的上游api类型对不对,有时候渠道维护人员自己可能都不是那么清楚是否支持对应的格式,而codex是有些内部工具或者compact是必须走原生的responses的,转换来的responses不行

## #49 一名白 (@borlxy)

Created: 2026-05-15T01:46:24.937Z
Updated: 2026-05-15T01:46:24.937Z
Reply to: #44 一名白

是手动绑定的渠道，自动的价格不太可控就没用

## #50 老白 (@laobaile)

Created: 2026-05-15T01:51:45.477Z
Updated: 2026-05-15T01:51:45.477Z

[![image](https://cdn3.ldstatic.com/original/4X/e/a/3/ea385de5dcdbce41b4c26686fdf06187c38fde9d.png)image868×234 11.8 KB](https://cdn3.ldstatic.com/original/4X/e/a/3/ea385de5dcdbce41b4c26686fdf06187c38fde9d.png)

又发现一个在缓存里面设置暗坑的

是不是需要限制手动改单项价格呢?只能通过倍率一键设置

## #51 老白 (@laobaile)

Created: 2026-05-15T01:54:34.615Z
Updated: 2026-05-15T01:54:34.615Z
Reply to: #49 一名白

[![image](https://cdn3.ldstatic.com/original/4X/8/3/4/834d3d4deb40919fc741ee0d7303b7883a1b7add.png)image842×187 15 KB](https://cdn3.ldstatic.com/original/4X/8/3/4/834d3d4deb40919fc741ee0d7303b7883a1b7add.png)

AI核查后给出的结论

## #52 HLiny (@HLiny)

Created: 2026-05-15T02:03:22.541Z
Updated: 2026-05-15T02:05:15.204Z
Reply to: #29 老白

佬友能不能强化一下标签筛选的的功能，然后把渠道的各种信息都标签化，比如接口 模型名 倍率 是否官方等等。比如我现在想找gpt5.5+responses格式+最低价的，如果我按渠道找就没办法按模型筛选，如果我按模型找就没办法按接口格式筛选。。。。。

这种情况下倍率粒度限制到单个模型也是合适的

## #53 一名白 (@borlxy)

Created: 2026-05-15T02:05:41.877Z
Updated: 2026-05-15T02:05:41.877Z
Reply to: #51 老白

那动态绑定是不是也会过滤掉这种渠道了？相当于一些仅支持 chat 的渠道在 reponse 请求下就直接都会过滤掉吗？难怪套一层或者测试场就没问题了

## #54 老白 (@laobaile)

Created: 2026-05-15T02:07:37.377Z
Updated: 2026-05-15T02:07:37.377Z
Reply to: #53 一名白

如果 reponses 请求带上了codex独有的websearch或者非function tool等就会强制要求上游是responses

## #55 b1ghawk119 (@b1ghawk119)

Created: 2026-05-15T02:09:45.565Z
Updated: 2026-05-15T02:11:05.162Z
Reply to: #51 老白

有些看不懂， ![:joy:](https://cdn.ldstatic.com/images/emoji/twemoji/joy.png?v=15) 允许Responses请求转换到Chat Completion，仍要求白名单包含出站格式，这个白名单在哪里，原版的Axonhub好像没有这个白名单。

![](https://cdn.ldstatic.com/user_avatar/linux.do/laobaile/48/951224_2.png) 老白:

> 又发现一个在缓存里面设置暗坑的
> 
> 是不是需要限制手动改单项价格呢?只能通过倍率一键设置

这个也是动态渠道的风险，我的LDC比较少，所以通常会先看定价。

## #56 b1ghawk119 (@b1ghawk119)

Created: 2026-05-15T02:48:30.594Z
Updated: 2026-05-15T02:48:46.231Z
Reply to: #54 老白

对于Completions上游，因为不知道是不是错配了。

若Completions失败，尝试responses调用上游，如果成功，记录该Key在该渠道的最后一次成功调用的格式(也就是加一张中间表，或者把这个映射关系放Redis，含TTL)，这个策略可以么。

## #57 老白 (@laobaile)

Created: 2026-05-15T02:51:19.086Z
Updated: 2026-05-15T02:52:02.000Z
Reply to: #56 b1ghawk119

新版本渠道可以自己选择额外支持的api格式,勾选的就会调用了,不选的还是不调

## #58 b1ghawk119 (@b1ghawk119)

Created: 2026-05-15T02:52:06.816Z
Updated: 2026-05-15T02:53:48.889Z
Reply to: #57 老白

太好了，现在已经发布到线上了吗。

(这个字数限制和Bubble还是有点冲突的样子，特备对于希望得到回复的情况，用Bubble无法被追答，用回帖字数又不足。）

## #59 老白 (@laobaile)

Created: 2026-05-15T02:52:59.023Z
Updated: 2026-05-15T02:52:59.023Z
Reply to: #58 b1ghawk119

![](https://cdn.ldstatic.com/user_avatar/linux.do/laobaile/48/951224_2.png) 老白:

> 限制手动改单项价格呢?只能通过倍率一键设置

做完上面的限制就上线,现在在做测试中

## #60 b1ghawk119 (@b1ghawk119)

Created: 2026-05-15T04:20:10.978Z
Updated: 2026-05-15T04:34:54.358Z
Reply to: #57 老白

这个是在渠道设置里的对吗：

[![image](https://cdn3.ldstatic.com/optimized/4X/a/3/c/a3c7bb1ff9d586d1eff5f8e643ae44f14ef7719d_2_689x222.png)image1240×400 31.7 KB](https://cdn3.ldstatic.com/original/4X/a/3/c/a3c7bb1ff9d586d1eff5f8e643ae44f14ef7719d.png)

对于现有的错配的渠道，它们是不是仍不可用于responses api。

## #61 b1ghawk119 (@b1ghawk119)

Created: 2026-05-15T06:57:25.772Z
Updated: 2026-05-15T07:07:17.444Z
Reply to: #59 老白

哎。。还是不行…实在太难了。

-–  您看看下面这个情况 —

[#p-17872862-h-1-8570-1](#p-17872862-h-1-8570-1)1. 渠道 #8570
面板有模型。

[![32818a87a29b61e86a843775d677ec1c](https://cdn3.ldstatic.com/optimized/4X/3/3/8/3381202bc96c24a26b12407d2690d80da28a60d9_2_403x500.png)32818a87a29b61e86a843775d677ec1c734×910 49.9 KB](https://cdn3.ldstatic.com/original/4X/3/3/8/3381202bc96c24a26b12407d2690d80da28a60d9.png)

[#p-17872862-h-2-api-2](#p-17872862-h-2-api-2)2. API秘钥

[![image](https://cdn3.ldstatic.com/optimized/4X/e/6/4/e64f0fe388cf779e32c84c551f0584512557fb68_2_645x500.png)image1374×1064 94.7 KB](https://cdn3.ldstatic.com/original/4X/e/6/4/e64f0fe388cf779e32c84c551f0584512557fb68.png)

[#p-17872862-h-3-axonhub-3](#p-17872862-h-3-axonhub-3)3. 在自己本地的AxonHub获取模型
取不到任何模型。

[![71525751bb6d84a9efec820669b07638](https://cdn3.ldstatic.com/optimized/4X/d/2/b/d2b889a7c6f99353b0df378f308299d55eb4ff00_2_687x500.jpeg)71525751bb6d84a9efec820669b076381738×1264 210 KB](https://cdn3.ldstatic.com/original/4X/d/2/b/d2b889a7c6f99353b0df378f308299d55eb4ff00.jpeg)

[#p-17872862-h-4-responses-4](#p-17872862-h-4-responses-4)4. 使用Responses格式拨测
出现422

[![b94826f7ad045a8e79afb9b3340b9a6e](https://cdn3.ldstatic.com/optimized/4X/2/2/e/22e5862047e0d1b7028d501c2cf44e296a21db59_2_690x259.png)b94826f7ad045a8e79afb9b3340b9a6e2578×970 243 KB](https://cdn3.ldstatic.com/original/4X/2/2/e/22e5862047e0d1b7028d501c2cf44e296a21db59.png)

[#p-17872862-h-5-chat-5](#p-17872862-h-5-chat-5)5. 使用Chat格式拨测
出现422

[![e2c99bfe55834d8890e8867bd6422708](https://cdn3.ldstatic.com/optimized/4X/6/a/1/6a1d927233657d3f8def0b888fdaeb913fcd3925_2_689x259.png)e2c99bfe55834d8890e8867bd64227082688×1010 282 KB](https://cdn3.ldstatic.com/original/4X/6/a/1/6a1d927233657d3f8def0b888fdaeb913fcd3925.png)

[#p-17872862-tools-6](#p-17872862-tools-6)像这种拨测，一般都是很纯净的请求，不会带上tools之类的其它东西。
Axonhub抓包：

[![25b021ee6ece5ea1017e05dab621a3ad](https://cdn3.ldstatic.com/optimized/4X/b/d/4/bd44e84d636f027b43f8c6035c31c95020435240_2_690x293.png)25b021ee6ece5ea1017e05dab621a3ad2162×920 122 KB](https://cdn3.ldstatic.com/original/4X/b/d/4/bd44e84d636f027b43f8c6035c31c95020435240.png)

[![ef07c9747b5e0635c20e2aa0d376b87a](https://cdn3.ldstatic.com/optimized/4X/6/e/9/6e939238eca1462d81c264b8fee74efecb594bd1_2_690x101.png)ef07c9747b5e0635c20e2aa0d376b87a2210×324 37.9 KB](https://cdn3.ldstatic.com/original/4X/6/e/9/6e939238eca1462d81c264b8fee74efecb594bd1.png)

Reable抓包：

[![image](https://cdn3.ldstatic.com/optimized/4X/7/7/0/770a65e2b00cff8214c25db5688e9433bd7a0ab5_2_690x439.png)image2304×1468 304 KB](https://cdn3.ldstatic.com/original/4X/7/7/0/770a65e2b00cff8214c25db5688e9433bd7a0ab5.png)

[![image](https://cdn3.ldstatic.com/optimized/4X/6/8/1/681b1bec2b329cfb0804eeac8f0d9007ad07653a_2_690x403.png)image2470×1446 387 KB](https://cdn3.ldstatic.com/original/4X/6/8/1/681b1bec2b329cfb0804eeac8f0d9007ad07653a.png)

佬是否考虑开源呢，大伙儿可以闲修了提PR。

这个问题卡了好久了 ![:joy:](https://cdn.ldstatic.com/images/emoji/twemoji/joy.png?v=15)

## #62 b1ghawk119 (@b1ghawk119)

Created: 2026-05-15T06:57:35.130Z
Updated: 2026-05-15T06:57:35.130Z

