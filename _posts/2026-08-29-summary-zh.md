---
layout: default
title: "Horizon Summary: 2026-08-29 (ZH)"
date: 2026-08-29
lang: zh
---

> 从 66 条内容中筛选出 15 条重要资讯。

---

**科技新闻**
1. [Htmx 4.0 发布：超媒体驱动前端库重大更新](#item-tech-news-1) ⭐️ 8.0/10
2. [OpenAI 在 Cursor 被 SpaceX 收购后公布决定](#item-tech-news-2) ⭐️ 8.0/10
3. [美国制裁 Autistici/Inventati 托管商引发基础设施担忧](#item-tech-news-3) ⭐️ 8.0/10
4. [仅凭漏洞传闻，AI 编码代理数分钟内即可开发出攻击](#item-tech-news-4) ⭐️ 8.0/10
5. [用 Apple Virtualization.framework 启动虚拟 iPhone 的开源工具 vphone-cli](#item-tech-news-5) ⭐️ 7.0/10
6. [键盘驱动 GUI 的呼吁与开发者争议](#item-tech-news-6) ⭐️ 7.0/10

**科技博客**
1. [优势消失后的算法交易困惑](#item-tech-blog-1) ⭐️ 4.0/10

**财经新闻**
1. [玉米和小麦期货价格升至三年多高点](#item-finance-news-1) ⭐️ 8.0/10
2. [美上诉法院：体育赛事事件合约属赌博，预测市场平台或上诉至最高法院](#item-finance-news-2) ⭐️ 8.0/10
3. [PayPal 盘前大跌近 16%；Affirm、Gap 等因财报上涨](#item-finance-news-3) ⭐️ 8.0/10
4. [沃什讲话后，9 月美联储加息概率接近五五开](#item-finance-news-4) ⭐️ 7.0/10
5. [英伟达营收预测强劲，SpaceX 独家采购引发关注](#item-finance-news-5) ⭐️ 7.0/10
6. [美联储主席沃什：通胀问题仍有“工作要做”](#item-finance-news-6) ⭐️ 7.0/10
7. [SBI 以 2.7 亿美元收购印尼 Ajaib 20%股份，拓展日元稳定币东南亚业务](#item-finance-news-7) ⭐️ 7.0/10
8. [阿布扎比王室据报入股特朗普相关加密银行项目 49%股份](#item-finance-news-8) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Htmx 4.0 发布：超媒体驱动前端库重大更新](https://four.htmx.org/announcements/2026-08-28-htmx-4.0.0-is-released) ⭐️ 8.0/10

Htmx 4.0 已正式发布，这是广受欢迎的基于超媒体（hypermedia）驱动的前端库的一次重大版本更新。该版本延续了 htmx 以 HTML 属性实现交互、由后端生成 UI 的设计思路，并引入 hx-alpine-compat 等兼容性改进，以缓解与 Alpine.js 配合使用时的问题。此次发布在 Hacker News 上获得较高关注（565 分、138 条评论），反映出社区对轻量、无需复杂构建步骤的 Web 开发方式的持续兴趣。受制于公告原文细节不详，本次发布的具体特性、变更与兼容性说明尚未完整披露。

hackernews · rmsaksida · 8月28日 13:28 · [社区讨论](https://news.ycombinator.com/item?id=49478178)

**「背景」** htmx 是一个流行的超媒体驱动前端库，允许开发者通过在 HTML 属性中声明请求和响应处理逻辑，实现无需编写大量 JavaScript 的动态 Web 界面。htmx 4.0 是自 2.x 以来的主要版本，官方称其是从底层使用 fetch\(\) API 对实现进行了重写，并内置了基于 Etag 的条件请求支持。该版本还提供了从 htmx 2.x 迁移到 4.x 的升级指南，以及用于平滑处理与 Alpine.js 兼容性问题的 hx-alpine-compat 属性。

**「影响」** Htmx 4.0 的发布为采用超媒体驱动开发的前端项目带来了新特性，例如 hx-partial 标签，但也在开发者社区引发了对该版本方向（尤其是 fetch 迁移）的混合评价。对于正在评估或已使用 htmx 的团队，这一版本可能促使他们重新权衡后端渲染与前端框架之间的选择。

**「社区讨论」** 评论中既有赞赏也有分歧：htmx CEO 与部分开发者认为它简洁、适合 Go+SQLite 等轻量组合，也有 .NET/Angular 背景的开发者认为它迫使后端混入展示逻辑而更困难；还有人认为 alpine-ajax 比 htmx 更小且足够使用。总体上，社区认可其简洁性，但对其适用场景与架构取舍存在不同看法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://four.htmx.org/announcements/2026-08-28-htmx-4.0.0-is-released">htmx 4 . 0 .0 has been released ! ~ htmx</a></li>
<li><a href="https://four.htmx.org/whats-new-in-htmx-4/">htmx ~ Changes in htmx 4 . 0</a></li>
<li><a href="https://biggo.com/news/202511040131_htmx-4-community-reaction">HTMX 4 . 0 Sparks Community Debate: Fetch Migration... - BigGo News</a></li>
<li><a href="https://www.youtube.com/watch?v=cukQ7e9FEik">HTMX 4 . 0 sneak peek - hx-partial tag and overview! - YouTube</a></li>

</ul>
</details>

**标签**: `#htmx`, `#web development`, `#hypermedia`, `#release`, `#frontend`

---

<a id="item-tech-news-2"></a>
### [OpenAI 在 Cursor 被 SpaceX 收购后公布决定](https://openai.com/index/our-decision-on-cursor-following-its-acquisition-by-spacex/) ⭐️ 8.0/10

OpenAI 已就编程助手 Cursor 被 SpaceX 收购一事发布官方决定，此举将影响开发者对 AI 模型的访问，并标志着前沿 AI 领域竞争联盟的转变。该决定与 Cursor 转售第三方模型 API 的业务模式相关，且发生在 Anthropic 此前因类似服务条款违规对 xAI 采取限制措施之后。目前官方尚未公布更多细节，模型访问变更的具体范围和执行方式仍待确认。

hackernews · meetpateltech · 8月29日 01:47 · [社区讨论](https://news.ycombinator.com/item?id=49486172)

**「背景」** OpenAI 于 2026 年 8 月宣布，在 Cursor 被 SpaceX 收购后，将逐步终止向其提供 OpenAI 模型的合同，并提议将 2026 年 11 月 12 日作为模型访问的截止日期。Cursor 是一款广受欢迎的 AI 编程工具，而 SpaceX 由 Elon Musk 控制；Musk 与 OpenAI CEO 之间长期存在激烈竞争，此前 Anthropic 也曾因类似的服务条款问题禁止 xAI 使用其模型。此举反映出前沿 AI 企业在模型供应与竞争联盟上的进一步分化。

**「影响」** OpenAI 已决定在 SpaceX 收购 Cursor 后停止向 Cursor 提供其模型，因此依赖 Cursor 中 OpenAI 模型的开发者将需要改用其他模型提供商或工具。这一决定也导致 Cursor 的多模型平台面临模型选择减少的后果，并可能进一步推动 AI 编码市场的整合。

**「社区讨论」** 评论者普遍认为，Cursor 将自己出售给竞争性模型提供商后，这一决定是意料之中的升级；有人指出 Anthropic 此前已对 xAI 采取过类似行动。部分用户表示，他们将继续使用 Anthropic 或仅在 Cursor 中依赖 Grok/Composer 模型，而不愿为 OpenAI 访问额外付费。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/our-decision-on-cursor-following-its-acquisition-by-spacex/">Our decision on Cursor following its acquisition by SpaceX - OpenAI</a></li>
<li><a href="https://www.reuters.com/business/media-telecom/openai-end-partnership-with-spacexs-cursor-2026-08-29/">OpenAI to end agreement with SpaceX&#x27;s AI coding tool Cursor ... - Reuters</a></li>
<li><a href="https://www.explainx.ai/blog/openai-ends-cursor-partnership-spacex-acquisition-august-2026">OpenAI Ends Cursor Model Access Nov 12 - explainx.ai</a></li>
<li><a href="https://claudecode.jp/en/news/can-cursor-remain-an-open-platform-inside-of-spacex">AI Coding Tools at Risk: Anthropic and Cursor Face... - ClaudeCode JP</a></li>
<li><a href="https://lumienai.com/news/spacex-buying-cursor-openai-anthropic-model-access">SpaceX Is Buying Cursor . What Happens to OpenAI and</a></li>
<li><a href="https://openai.com/index/our-decision-on-cursor-following-its-acquisition-by-spacex/">Our decision on Cursor following its acquisition by SpaceX | OpenAI</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Cursor`, `#SpaceX`, `#AI competition`, `#model access`

---

<a id="item-tech-news-3"></a>
### [美国制裁 Autistici/Inventati 托管商引发基础设施担忧](https://www.inventati.org/) ⭐️ 8.0/10

美国政府将意大利活动人士托管服务商 Autistici/Inventati（A/I）及其博客平台 noblogs.org 列入制裁名单，并将其认定为“全球恐怖分子”。这一决定史无前例地针对基础设施提供者，引发了对隐私工具、去中心化技术和开源社区可能被刑事化的担忧。A/I 始于 2001 年热那亚八国集团峰会期间，曾参与搭建独立媒体中心；目前 autistici.org 已无法访问，noblogs.org 部分失灵。社区讨论中有人质疑缺乏该组织直接支持或托管库尔德工人党（PKK）网站的证据。

hackernews · exiguus · 8月28日 12:58 · [社区讨论](https://news.ycombinator.com/item?id=49477854)

**「背景」** Autistici/Inventati（A/I）是一个由志愿者运营的意大利技术集体，长期为活动人士、个人和组织提供加密邮箱、匿名托管和博客服务（如 noblogs.org），自称提供“数字自卫”工具。美国财政部和国务院依据相关行政命令，以支持“极左恐怖主义”为由将这一基础设施提供方列入制裁名单；此类制裁通常意味着冻结涉事方在美国的资产，并禁止美国个人或实体与其交易。此次被制裁的并非武装团体，而是通信与托管服务的提供者，因此被视为对基础设施供应商的罕见且有争议的打击。

**「影响」** 受影响的用户包括 noblogs.org 的博主和依赖 autistici.org 邮箱及服务的用户，相关服务已出现中断；该案例还可能为其他国家制裁开源基础设施提供先例。

**「社区讨论」** 评论者普遍认为将基础设施提供商列为“恐怖分子”是前所未有的，并担心类似逻辑会波及 I2P、Monero、Veilid、Tox、Signal 等项目；也有评论指出 A/I 参与 2001 年热那亚抗议活动的历史，但多位用户表示找不到该组织直接支持 PKK 的证据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://kollektivbibliothek.noblogs.org/?p=2461">In solidarity with Autistici / Inventati | kollektivbibliothek</a></li>
<li><a href="https://www.zerohedge.com/markets/us-sanctions-3-groups-accused-supporting-far-left-terrorism">US Sanctions 3 Groups Accused Of Supporting Far-Left... | ZeroHedge</a></li>

</ul>
</details>

**标签**: `#sanctions`, `#internet freedom`, `#hosting`, `#privacy`, `#activism`

---

<a id="item-tech-news-4"></a>
### [仅凭漏洞传闻，AI 编码代理数分钟内即可开发出攻击](https://simonwillison.net/2026/Aug/28/just-a-rumour-of-a-bug/) ⭐️ 8.0/10

剑桥大学计算机科学教授、OCaml 编译器核心维护者 Anil Madhavapeddy 发文称，OCaml 项目安全补丁在公开讨论后约十分钟内就会遭到针对百分号编码遍历序列的探测，表明自动化监视者正盯住公共仓库。他用自己的代理演示了这一速度，并称在 Claude Fable 拒绝任务后改用 DeepSeek V4 Pro。rclone 维护者 Nick Craig-Wood 证实，项目近一个月收到超过 40 份安全披露，而此前十年共约 20 份，其中约 75%的披露含有需要处理的问题。GitHub 的 CVE 分配时间也从原来的 2-3 天拉长到 3-4 周，导致维护者不得不在变更日志中先用“CVE-PENDING”标记。这些迹象显示现有开源漏洞披露与封禁流程已难以跟上 AI 驱动漏洞利用的速度。

rss · Simon Willison · 8月28日 22:12

**「背景」** 传统开源安全流程通常会给安全补丁或公告设置一段封禁期，让维护者先完成修复和发布，再公开细节。如今 AI 编码代理可以根据公开仓库中的短短一句话线索快速定位并生成可用的漏洞利用，使“传闻本身就可能成为攻击情报”，从而压缩了传统披露流程的时间窗口。

**「影响」** 开源维护者正面临安全披露和潜在可利用攻击的激增，像 rclone 这样项目不得不在大量时间和 AI 工具帮助下进行分诊与修复，同时 GitHub 的 CVE 编号延迟迫使发布流程临时改用“CVE-PENDING”，可能让下游用户更难快速判断风险并安排升级。

**「社区讨论」** 评论中有人指出“从一句话线索推出漏洞利用”并非 LLM 时代才有的新现象，LLM 的真正影响是让这类利用被规模化、民主化地用于大量低价值目标；也有评论强调，部署和供应链更新往往比发现漏洞更难，未必能在数分钟内完成修复落地。另有开发者提到自己构建了监视提交并尝试检测“静默修复”的工具，进一步印证了对公开仓库自动监控的趋势。

**标签**: `#security`, `#AI agents`, `#OCaml`, `#exploits`, `#open source`

---

<a id="item-tech-news-5"></a>
### [用 Apple Virtualization.framework 启动虚拟 iPhone 的开源工具 vphone-cli](https://github.com/Lakr233/vphone-cli) ⭐️ 7.0/10

vphone-cli 是一个开源的命令行工具，通过 Apple 的 Virtualization.framework 启动虚拟 iPhone，使开发者和安全研究人员能够在虚拟环境中进行 iOS 应用测试与逆向工程。该项目托管在 GitHub 上，采用了不同于常规 iOS 模拟器的虚拟机方案，但仅限于 Apple 平台运行，并且需要关闭或部分关闭系统完整性保护（SIP）。现有材料没有提供具体的固件、系统镜像或完整兼容性说明，因此实际可用范围仍需参考项目文档。

hackernews · hentrep · 8月28日 23:02 · [社区讨论](https://news.ycombinator.com/item?id=49485267)

**「背景」** 苹果的 Virtualization.framework 是 macOS 上的虚拟化框架，允许开发者在 Apple Silicon 上运行虚拟机。vphone-cli 利用其中的 PCC research VM 基础设施，在 macOS 15 及更高版本上启动虚拟 iPhone（iOS 26），并提供命令行界面进行配置与管理。该项目要求 Apple Silicon Mac、Xcode 和 iOS SDK（用于交叉编译 guest 守护进程），主要面向测试、开发与安全研究，与 iOS Simulator 这类模拟器有本质区别。

**「影响」** 对 iOS 开发者和逆向工程师而言，该工具可能开辟一条无需实体 iPhone 的虚拟化测试路径，但前提是运行在 Apple 平台上、正确配置 SIP，并避免在虚拟 iOS 设置中选择日本或欧盟等会触发额外监管检查的地区。

**「社区讨论」** 评论区中，有人对它与 iOS 模拟器的区别提出疑问，也有人好奇未来是否能在 PC 上运行；另有用户指出关闭或部分关闭 SIP 可能破坏某些功能，并询问日本和欧盟地区设置会触发哪些额外的监管检查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Lakr233/vphone-cli">GitHub - Lakr233/ vphone - cli · GitHub</a></li>
<li><a href="https://numfer.com/Lakr233/vphone-cli">vphone - cli : Virtualize iOS on macOS</a></li>
<li><a href="https://senumy.com/vphone-cli-ios-26-virtual-iphone-setup/">vphone - cli &amp; vphone-aio: Easier iOS 26 Virtual iPhone Setup on...</a></li>

</ul>
</details>

**标签**: `#iOS virtualization`, `#Apple Virtualization.framework`, `#reverse engineering`, `#iOS development`, `#open source`

---

<a id="item-tech-news-6"></a>
### [键盘驱动 GUI 的呼吁与开发者争议](https://ckardaris.com/blog/2026/08/28/keyboard-driven-guis.html) ⭐️ 7.0/10

作者 ckardaris 发表博客文章《GUIs should be fully keyboard-driven》，主张图形用户界面应支持完整的键盘驱动操作，而不仅是快捷键兼容。该观点在 Hacker News 上引发大量讨论，共 324 条评论，核心涉及无障碍访问、效率型用户需求以及 UI 框架设计责任。支持者认为键盘可达性常被忽视，且框架负有主要责任；反对者则认为效率型用户体验不等同于通用用户体验，不应强推键盘驱动。讨论还提出“键盘兼容”与“真正键盘驱动”的区分，并指出快捷键可发现性仍是实践难点。

hackernews · ckardaris · 8月28日 15:17 · [社区讨论](https://news.ycombinator.com/item?id=49479837)

**「背景」** 无障碍标准（如 WCAG 和美国残疾人法案 ADA）通常要求软件和网站支持键盘导航，以便视力障碍、运动障碍等用户无需使用鼠标即可操作。自适应键盘、鼠标等辅助设备以及屏幕阅读器都依赖底层界面具备完整的键盘可达性，因此键盘驱动不仅关乎效率，更涉及合规与平等访问。

**「影响」** 对依赖键盘的残障用户和追求效率的开发者而言，该讨论强化了将键盘导航作为 GUI 框架一等公民的必要性，并提醒应用开发者避免因焦点管理不当而让键盘用户“撞墙”。

**「社区讨论」** 评论中，有开发者从无障碍合规角度强调键盘操作的必要性，并认为 UI 框架应为此负责；也有观点认为不应把高难度键盘操作强加给所有用户。另有讨论区分了“快捷键兼容”与“真正键盘驱动”，并指出可发现性仍是难点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://accessibe.com/">Web Accessibility Platform for WCAG</a></li>
<li><a href="https://know-the-ada.com/adaptive-keyboards-and-mice-tools-for-physical-accessibility/">Adaptive Keyboards and Mice: Tools for Physical Accessibility – KNOW-THE-ADA</a></li>
<li><a href="https://slashdot.org/software/ada-compliance/">Best ADA Compliance Software in 2025</a></li>

</ul>
</details>

**标签**: `#accessibility`, `#keyboard-navigation`, `#user-interface`, `#software-design`, `#hn-discussion`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [优势消失后的算法交易困惑](https://www.reddit.com/r/algotrading/comments/1w0ipa5/where_do_i_go_from_here/) ⭐️ 4.0/10

reddit · r/algotrading · /u/Extension\_Ad4492 · 8月28日 06:27

**「背景」** 作者原想用交易实验来反驳交易，却因纸面盈利迅速上头，投入六个月开发交易机器人。中东局势带来的行情让策略最初赚了不少，但随着市场反应减弱，他眼中的优势很快消失。

**「方案」** 作者自建 K 线和回测系统，拥有 6 个月的 tick 数据，在黄金和布伦特原油上测试了六种策略，包括布林带均值回归、趋势回调等。接下来他加入制度过滤器，按趋势/震荡、多空方向以及短周期是否一致划分格子，又用希尔伯特变换、ADX 等变量分类市场状态，却找不到策略明显更有效的区域。他因此倾向于认为日间交易不成立，但又怀疑 tick 数据可能不可靠，或者早期极端趋势应单独分类，所以不愿接受这个结论，于是求教下一步是换资产、做配对交易还是转向波段交易。

**「启示」** 作者的核心纠结在于：当回测和过滤器都找不回消失的利润时，该承认“日间交易不行”，还是质疑自己的数据和分类方式。这个个人反思虽缺乏充分证据，却生动展示了策略优势丧失后常见的困惑与自我怀疑。

**标签**: `#algorithmic trading`, `#backtesting`, `#regime filtering`, `#day trading`, `#trading edge`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [玉米和小麦期货价格升至三年多高点](https://www.cnbc.com/2026/08/28/corn-and-wheat-prices-jump-to-highest-prices-in-more-than-three-years.html) ⭐️ 8.0/10

8 月 28 日，玉米和小麦期货价格升至三年多高点：小麦期货收于每蒲式耳 784 美分，上涨 3.1%，周涨 12.1%；玉米期货收于每蒲式耳 536.5 美分，上涨 0.6%，8 月累计上涨 15.6%。上涨主因黑海地区紧张局势和美国供应担忧。

rss · CNBC Finance · 8月28日 20:00

**「背景」** 小麦涨势主要来自俄乌紧张局势导致黑海地区出口中断，俄罗斯和乌克兰合计占全球小麦出口逾四分之一；玉米涨势则主要源于美国供应担忧，美国农业部 8 月报告将玉米单产预测下调至每英亩 180.7 蒲式耳，叠加乌克兰出口受限。

**标签**: `#agriculture`, `#commodities`, `#wheat`, `#corn`, `#supply disruption`

---

<a id="item-finance-news-2"></a>
### [美上诉法院：体育赛事事件合约属赌博，预测市场平台或上诉至最高法院](https://www.cnbc.com/2026/08/28/appeals-court-rules-against-prediction-markets-tees-up-scotus-fight.html) ⭐️ 8.0/10

美国第九巡回上诉法院裁定，Kalshi、Crypto.com 与 Robinhood 提供的体育赛事“事件合约”不属于美国商品期货交易委员会（CFTC）监管的互换，而是体育博彩，因此内华达等州可以叫停相关产品；这一裁决与第三巡回法院此前的结论相冲突，可能形成上诉至最高法院的法律争议。

rss · CNBC Finance · 8月29日 02:23

**「背景」** 平台和 CFTC 主张所有事件合约都是“互换”、应由联邦专属监管，而 44 个州认为体育赛事合约就是体育博彩；第三巡回法院 4 月曾裁定 CFTC 有专属管辖权，第九巡回法院此次相反，形成“巡回法院分歧”（不同上诉法院对同一法律问题作出相反裁决）。

**「影响」** 这意味着 Kalshi、Crypto.com 和 Robinhood 在内华达州被叫停的体育赛事合约业务暂时无法通过法院禁令恢复。

**标签**: `#prediction markets`, `#CFTC`, `#regulation`, `#derivatives`, `#court ruling`

---

<a id="item-finance-news-3"></a>
### [PayPal 盘前大跌近 16%；Affirm、Gap 等因财报上涨](https://www.cnbc.com/2026/08/28/stocks-making-the-biggest-moves-premarket-pypl-afrm-gap-mrvl.html) ⭐️ 8.0/10

据彭博社援引知情人士报道，Advent 和 Stripe 决定放弃收购 PayPal，PayPal 盘前大跌近 16%。业绩消息令个股分化：Affirm 第四财季营收 11.7 亿美元、高于预期的 11.1 亿美元，股价涨 13%；Gap 第二季度调整后每股盈利 52 美分、高于预期的 48 美分，股价涨近 15%；Elastic 全年盈利指引高于预期，涨逾 17%；Marvell、Rubrik、Autodesk 则因指引或毛利率不及预期分别跌约 8%、逾 5%和近 4%。

rss · CNBC Finance · 8月28日 11:43

**「背景」** 盘前交易指美股常规时段开始前的买卖；这笔 PayPal 收购案若完成，原本可能成为规模最大的杠杆收购案之一（杠杆收购指收购方主要靠借款买下目标公司）。

**标签**: `#PayPal`, `#leveraged buyout`, `#earnings guidance`, `#stock movers`, `#fintech`

---

<a id="item-finance-news-4"></a>
### [沃什讲话后，9 月美联储加息概率接近五五开](https://www.cnbc.com/2026/08/28/-september-fed-decision-now-a-coin-flip-as-rate-hike-odds-increase.html) ⭐️ 7.0/10

美联储主席沃什发表鹰派讲话后，交易员对 9 月 16 日加息 25 个基点的概率预期接近五五开：Kalshi 显示 48%，CME FedWatch 显示 56%，Polymarket 显示 49%。在沃什讲话前，7 月非农就业意外疲弱曾令加息预期降温，但沃什表示仍需看到通胀明确向 2%目标回归的证据。

rss · CNBC Finance · 8月28日 15:22

**「背景」** 在沃什讲话前，交易员对美联储 9 月维持利率不变的概率一度接近 70%；讲话后，CME FedWatch 工具显示 9 月加息 25 个基点的概率升至约 55.7%，较一天前上升约 20 个百分点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/economy/live/jackson-hole-fed-summit-live-kevin-warsh-keynote-speech-180442096.html">Jackson Hole Fed summit live: Kevin Warsh&#x27;s keynote speech comes at a pivotal moment for the Federal Reserve</a></li>
<li><a href="https://www.cnbc.com/2026/08/28/kevin-warsh-jackson-hole-federal-reserve-inflation.html">Fed Chairman Warsh warns on inflation at Jackson Hole</a></li>
<li><a href="https://www.theguardian.com/business/live/2026/aug/28/us-federal-reserve-kevin-warsh-jackson-hole-conference-inflation-economy-ftse-stock-markets-latest-updates">US Federal Reserve’s Kevin Warsh warns there will be ‘work to do’ unless high inflation eases – as it happened | Business | The Guardian</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#Interest Rates`, `#Monetary Policy`, `#Inflation`, `#Treasury Yields`

---

<a id="item-finance-news-5"></a>
### [英伟达营收预测强劲，SpaceX 独家采购引发关注](https://www.marketwatch.com/story/nvidias-revenue-forecast-is-so-huge-that-wall-street-wonders-if-spacex-is-the-reason-1ee7a8a9?mod=mw_rss_topstories) ⭐️ 7.0/10

英伟达给出的营收预测非常强劲，让华尔街猜测部分原因是 SpaceX 最近宣布将只购买英伟达芯片并计划投入巨资。这显示大型科技与航天公司对 AI 算力的需求正在增加。

rss · MarketWatch Top Stories · 8月28日 20:58

**「背景」** 英伟达此前公布了一份高得惊人的营收预测，部分华尔街人士猜测 SpaceX 的大规模芯片采购是原因之一。SpaceX 近期宣布将只购买英伟达的芯片，而英伟达在 8 月 14 日的监管文件中披露持有 SpaceX 约 210 亿美元股权；有报道称 SpaceX 和英特尔都承诺独家购买英伟达芯片。

**「影响」** 对英伟达而言，SpaceX 的独家采购承诺强化了其 AI 芯片需求；消息公布当天英伟达股价上涨 3.12%至 218.56 美元。对 SpaceX 而言，只使用单一供应商会加大供应链集中风险，若未来出现芯片短缺或供应瓶颈，可能影响其 AI 部署进度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.marketwatch.com/story/nvidias-revenue-forecast-is-so-huge-that-wall-street-wonders-if-spacex-is-the-reason-1ee7a8a9">Nvidia&#x27;s revenue forecast is so huge that Wall Street wonders if SpaceX ...</a></li>
<li><a href="https://www.techtimes.com/articles/324564/20260815/nvidia-discloses-50b-equity-stake-spacex-intel-both-exclusive-chip-buyers.htm">Nvidia Discloses $50B Equity Stake in SpaceX and Intel: Both Exclusive ...</a></li>
<li><a href="https://cryptobriefing.com/nvidia-revenue-spacex-impact-speculation/">Nvidia&#x27;s revenue forecast raises speculation about SpaceX impact</a></li>
<li><a href="https://www.techrepublic.com/article/news-spacex-nvidia-exclusive-ai-chip-strategy/">Elon Musk Goes All-In on Nvidia: What SpaceX’s Chip Strategy Means for AI Infrastructure</a></li>
<li><a href="https://thebusinessperspective.com/spacex-nvidia-ai-chip-deal/">SpaceX Nvidia AI Chip Deal: Why $15B Went to Nvidia Not AMD</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#SpaceX`, `#AI chips`, `#revenue forecast`, `#data center demand`

---

<a id="item-finance-news-6"></a>
### [美联储主席沃什：通胀问题仍有“工作要做”](https://www.coindesk.com/markets/2026/08/28/warsh-at-jackson-hole-we-have-work-to-do-on-inflaiton) ⭐️ 7.0/10

美联储主席凯文·沃什在杰克逊霍尔年会上表示，在降低通胀方面“还有工作要做”。这一表态未包含具体政策行动或数据，但被视为货币政策走向的重要信号。

rss · CoinDesk · 8月28日 14:05

**「背景」** 美联储主席凯文·沃什在杰克逊霍尔年度会议上表示，通胀仍过高，美联储在降低物价方面“还有工作要做”。这是他就任后首次在该会议发表重要讲话，市场随即提高了对加息的预期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=EhAKCIK-F0Q">LIVE: Fed Chair Kevin Warsh Speaks at Jackson Hole Amid Inflation ...</a></li>
<li><a href="https://www.nytimes.com/2026/08/28/business/markets-stocks-bonds-warsh-jackson-hole.html">Investors Expect Higher Rates After Fed Chairman’s Inflation Pledge</a></li>
<li><a href="https://www.cbsnews.com/news/kevin-warsh-fed-speech-jackson-hole-inflation/">Fed will have &quot;work to do&quot; if inflation doesn&#x27;t fade, Warsh ... - ...</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#inflation`, `#monetary policy`, `#Jackson Hole`, `#interest rates`

---

<a id="item-finance-news-7"></a>
### [SBI 以 2.7 亿美元收购印尼 Ajaib 20%股份，拓展日元稳定币东南亚业务](https://www.coindesk.com/business/2026/08/28/sbi-stakes-usd270-million-in-ajaib-to-expand-yen-stablecoin-in-southeast-asia) ⭐️ 7.0/10

据 CoinDesk 报道，日本 SBI 以 2.7 亿美元收购印尼公司 Ajaib 的 20%股份，以扩大其日元稳定币在东南亚的业务。

rss · CoinDesk · 8月28日 12:18

**「背景」** SBI Holdings 是一家日本金融集团，Ajaib Group 是印度尼西亚的在线券商。据多家报道，这笔约 2.7 亿美元、20%股权的交易将使 SBI 进入东南亚最大的散户投资市场之一，并以此推广其日元稳定币 JPYSC。

**「影响」** 这笔投资让 SBI 获得印尼最大散户投资平台之一 Ajaib 的渠道，便于在东南亚推广日元稳定币和区块链结算基础设施，可能影响当地散户投资者和区域数字资产市场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.coindesk.com/business/2026/08/28/sbi-stakes-usd270-million-in-ajaib-to-expand-yen-stablecoin-in-southeast-asia">How SBI &#x27;s $ 270 million Ajaib stake drives its Asian stablecoin ...</a></li>
<li><a href="https://gokhshtein.com/news/2026-08-28-sbi-holdings-deploys-270m-in-ajaib-to-establish-yen">SBI Holdings Deploys $ 270 M in Ajaib to Establish Yen Stablecoin ...</a></li>
<li><a href="https://www.indoneo.com/capital/sbi-ajaib-270-million-yen-stablecoin-indonesia/">SBI pays $ 270 M to make Indonesia Ajaib &#x27;s yen stablecoin gateway</a></li>
<li><a href="https://www.coindesk.com/business/2026/08/28/sbi-stakes-usd270-million-in-ajaib-to-expand-yen-stablecoin-in-southeast-asia">How SBI &#x27;s $270 million Ajaib stake drives its Asian stablecoin ...</a></li>
<li><a href="https://gokhshtein.com/news/2026-08-28-sbi-holdings-deploys-270m-in-ajaib-to-establish-yen">SBI Holdings Deploys $270M in Ajaib to Establish Yen Stablecoin ...</a></li>

</ul>
</details>

**标签**: `#SBI`, `#Ajaib`, `#stablecoin`, `#Southeast Asia`, `#fintech acquisition`

---

<a id="item-finance-news-8"></a>
### [阿布扎比王室据报入股特朗普相关加密银行项目 49%股份](https://cointelegraph.com/news/abu-dhabi-royal-trump-world-liberty-crypto-bank-wsj?utm_source=rss_feed&amp;utm_medium=rss&amp;utm_campaign=rss_partner_inbound) ⭐️ 7.0/10

据《华尔街日报》报道，阿布扎比王室成员谢赫·塔赫农的集团已收购 World Liberty 旗下控股公司 49%的股份；该控股公司拥有一家已获美国监管机构有条件批准的信托银行。该报道尚未得到官方确认。

rss · Cointelegraph · 8月28日 04:17

**「背景」** 据《华尔街日报》援引知情人士消息，阿布扎比王室成员谢赫·塔赫农（Sheikh Tahnoon bin Zayed Al Nahyan）及其联合投资者据称持有了 World Liberty Financial 拟建美国信托银行控股公司 49% 的股份。此前在 2025 年 1 月，该集团已向 World Liberty Financial 投资 5 亿美元换取 49%股权，属于加密领域规模最大的主权关联投资之一。该信托银行目前已获得有条件批准，但本次交易的具体金额和更多细节尚未披露。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cointelegraph.com/news/abu-dhabi-royal-trump-world-liberty-crypto-bank-wsj">Abu Dhabi Royal Backs Trump -Linked Crypto Bank Venture</a></li>
<li><a href="https://bingx.com/en/flash-news/post/wsj-abu-dhabi-s-sheikh-tahnoon-and-coinvestors-hold-of-wltc-holdings-behind-world-liberty-s-planned-usd-trust-bank">Abu Dhabi &#x27;s Sheikh Tahnoon Said to Hold 49 % of World ...</a></li>

</ul>
</details>

**标签**: `#crypto banking`, `#Abu Dhabi`, `#World Liberty`, `#investment`, `#regulatory approval`

---