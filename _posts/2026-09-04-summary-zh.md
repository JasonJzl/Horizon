---
layout: default
title: "Horizon Summary: 2026-09-04 (ZH)"
date: 2026-09-04
lang: zh
---

> 从 88 条内容中筛选出 19 条重要资讯。

---

**科技新闻**
1. [OpenAI 发布 GPT-6 Astra 旗舰模型及系统卡](#item-tech-news-1) ⭐️ 9.0/10
2. [Audacity 4.0 发布：基于 Qt6 的主要版本更新](#item-tech-news-2) ⭐️ 8.0/10
3. [用 LLM 将 1993 年 Amiga 汇编游戏移植到 Godot](#item-tech-news-3) ⭐️ 7.0/10
4. [K2 Horizon 发布六款开放模型：开放堆栈与模型质量引发讨论](#item-tech-news-4) ⭐️ 7.0/10
5. [GPS 受太阳风暴干扰，全美误差最多达 33 英尺](#item-tech-news-5) ⭐️ 6.0/10
6. [申真谞让两子击败 AI KataGo](#item-tech-news-6) ⭐️ 6.0/10

**科技博客**
1. [非线性记忆冲击模型的价格操纵分类](#item-tech-blog-1) ⭐️ 8.0/10
2. [切换摩擦、异质交易期限与长记忆订单流](#item-tech-blog-2) ⭐️ 7.0/10
3. [LLM 智能体在双向拍卖市场中的行为与评估框架](#item-tech-blog-3) ⭐️ 7.0/10
4. [用机器学习从公开数据度量高频交易](#item-tech-blog-4) ⭐️ 7.0/10
5. [公开数据下的元订单重构与 LMF 理论检验](#item-tech-blog-5) ⭐️ 7.0/10
6. [带仿射漂移随机 Volterra 积分方程的伪平稳理论](#item-tech-blog-6) ⭐️ 7.0/10

**财经新闻**
1. [英伟达以 129.3 亿美元收购 Hugging Face，加码 AI 软件业务](#item-finance-news-1) ⭐️ 8.0/10
2. [中国反驳 G20“依赖出口”批评 指其“宣扬保护主义”](#item-finance-news-2) ⭐️ 7.0/10
3. [澳大利亚加密企业牌照宽限期将于 9 月 30 日结束](#item-finance-news-3) ⭐️ 7.0/10
4. [美股盘前个股波动：Snowflake 大涨 24%，Ultragenyx 暴跌逾 46%](#item-finance-news-4) ⭐️ 6.0/10
5. [Adobe 宣布新任 CEO 后股价下跌](#item-finance-news-5) ⭐️ 6.0/10
6. [Lululemon 转向宽松裤装以应对紧身裤需求降温](#item-finance-news-6) ⭐️ 6.0/10
7. [渣打银行在迪拜外汇平台推出比特币和以太币现货交易](#item-finance-news-7) ⭐️ 6.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [OpenAI 发布 GPT-6 Astra 旗舰模型及系统卡](https://openai.com/index/gpt-6-astra/) ⭐️ 9.0/10

OpenAI 发布了新一轮旗舰模型 GPT-6 Astra，并同步公开了对应的部署安全系统卡。该模型在 ARC-AGI-3 等基准上表现突出，据发布信息还在 Artificial Analysis Coding Agent Index 上取得明显进展。社区讨论中有人质疑 ARC-AGI-3 评分使用不同测试环境不具可比性，也有观点认为除基准外，其它提升更像是小幅更新。发布之际同时出现了关于模型评测与发布进展的多个相关讨论串。

hackernews · kibae · 9月3日 18:41 · [社区讨论](https://news.ycombinator.com/item?id=49554643)

**「背景」** ARC-AGI-3 是 ARC Prize 推出的抽象推理基准，用未见过的任务衡量模型的通用流体智能。OpenAI 在 2026 年 9 月宣布新一代旗舰模型 GPT-6 Astra，并发布配套系统卡；OpenAI 称其在 ARC-AGI-3 得分 99.9%、在 ExploitBench 上得分 100%。ARC Prize 的评估显示，Astra 在行动效率上超越人类基线，在 96% 的关卡中所用动作少于测试人类的中位数，这也反映不同测评方和测评设置下得分口径存在差异。

**「影响」** 对于使用 OpenAI 模型进行编程和智能体任务的开发者，GPT-6 Astra 在 Coding Agent Index 上的提升可能意味着更强的编码智能体能力，但其 ARC-AGI 成绩的评测口径仍需依赖系统卡和独立复现确认。

**「社区讨论」** 评论区的主要争议集中在 ARC-AGI-3 榜单的可比性上：有用户指出官方展示的 GPT-5.6 Sol 分数与 GPT-6 Astra 分数可能使用了不同的评测框架，若统一用 responses API 评测，此前的得分估计约 30%，因此榜单可能具有误导性；也有用户认为除了 ARC 之外，其余基准提升显得相对温和，更像各实验室常见的“点”更新。另有评论质疑演示为何总以自动购物为例，并指出前沿模型的进步仍主要体现为技能习得而非真正的泛化智能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/blog/astra">OpenAI &#x27;s GPT - 6 Astra on ARC - AGI - 3 | ARC Prize</a></li>
<li><a href="https://openai.com/index/gpt-6-astra/">GPT - 6 Astra : A new generation of intelligence | OpenAI</a></li>

</ul>
</details>

**标签**: `#GPT-6`, `#OpenAI`, `#AI models`, `#ARC-AGI`, `#machine learning`

---

<a id="item-tech-news-2"></a>
### [Audacity 4.0 发布：基于 Qt6 的主要版本更新](https://github.com/audacity/audacity/releases/tag/Audacity-4.0.0) ⭐️ 8.0/10

Audacity 4.0 已作为这款开源音频编辑器的主要版本发布，将用户界面重构为基于 Qt6 的界面，并包含多项改进。此版本之所以重要，是因为 Audacity 是跨平台桌面音频编辑的常用工具，而这次界面与架构更新可能会影响大量用户与插件生态。社区反馈分化：有评论者推荐官方开发团队的介绍视频，认为新界面干净并修复了不少问题；但也有长期用户指出，JACK/Pipewire 支持方式仍不令人满意，并且对 audio.com 云端/遥测功能的推进表示担忧。目前官方发布说明的具体技术细节尚未在本文材料中提供。

hackernews · ClydeN · 9月3日 10:53 · [社区讨论](https://news.ycombinator.com/item?id=49548395)

**「背景信息」** Audacity 是一款广受欢迎的开源多轨音频编辑与录制软件，此前版本基于 wxWidgets 工具包开发。Audacity 4.0 是一次重大重写，彻底改用 Qt6 界面，并引入全新的 .aup4 项目格式和基于片段的剪辑编辑模型。此外，Audacity 曾因遥测与隐私政策引发争议，社区因此衍生出 Tenacity 等分支项目。

**「影响」** 对依赖 JACK/PipeWire 的 Linux 家庭录音室用户而言，Audacity 4 仍未能解决长期存在的 JACK 客户端不持久问题：据论坛报告，Audacity 在 JACK/PipeWire 下通常只在播放或录音活跃期间才显示节点，这与此前版本中的行为一致。

**「社区讨论」** 社区对 Audacity 4.0 的看法分化：有人推荐 Muse 软件主管和官方发布的 UI 演示视频，并认为新版本更干净、修复了不少问题；但仍有用户对持续的 JACK/Pipewire 集成方式、音频保存可靠性以及 audio.com/遥测功能扩张表示不满。部分评论还提到后遥测分支项目（Tenacity、Sneedacity）的现状，反映出信任问题依然存在。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linuxcompatible.org/story/audacity-400-released-complete-qt-rewrite-new-clip-editing-and-aup4-format">Audacity 4.0.0 Released: Complete Qt Rewrite, New Clip Editing, and .aup4 Format</a></li>
<li><a href="https://github.com/tenacityteam/tenacity">GitHub - tenacityteam/tenacity: Mirror of https://codeberg ...</a></li>
<li><a href="https://forum.audacityteam.org/t/audacity-linux-and-pipewire/149582">Audacity, Linux and PipeWire - Audacity 4 - Audacity Forum</a></li>

</ul>
</details>

**标签**: `#audacity`, `#open-source`, `#audio`, `#release`, `#qt6`

---

<a id="item-tech-news-3"></a>
### [用 LLM 将 1993 年 Amiga 汇编游戏移植到 Godot](https://babyloniantwins.com/blog/porting-a-1993-amiga-game-to-godot/) ⭐️ 7.0/10

一位开发者分享了他将 1993 年在巴格达用 MC68000 汇编语言为 Amiga 编写的游戏移植到 Godot 的过程。他使用 Claude 在假期用一个晚上完成了核心移植，之后又花几个周末和晚上调整手感并发布。Claude 在 Mac 上用 vasm 汇编代码，并持续比对直到二进制与其原始游戏中的二进制逐字节一致；最终仍存在约 108 字节的差异，原因是原版使用 AsmOne 在内存中汇编，保存的是已经运行过的内存快照，而不是干净的 AsmOne 输出。作者还免费发布了原版游戏。

hackernews · rabahs · 9月3日 14:28 · [社区讨论](https://news.ycombinator.com/item?id=49550375)

**「背景」** 1993 年的 Amiga 游戏通常直接用 68000 汇编开发，当时互联网尚未普及，参考资料非常稀缺。Godot 是一个现代跨平台游戏引擎。用 LLM 辅助将旧汇编代码翻译到新引擎的做法正在兴起，这个案例展示了结合汇编器验证等流程进行实际移植的可行性。

**「影响」** 对于希望把老旧汇编游戏或软件迁移到现代平台的开发者而言，这个案例说明在 LLM 辅助下，一个晚上即可完成核心逻辑移植，并可以用原始二进制做逐字节回归验证。同时，它也展示了这种工作流对复古游戏保护和重制的实际价值。

**「社区讨论」** 社区评论中，多位用户分享了类似的成功经历：有人让 Claude 将一个 ZX81 游戏的内存转储转成 Go，并建议用 LLM 不熟悉的游戏作为基准测试。还有读者表达了对作者在 1993 年文档匮乏环境下完成汇编游戏的钦佩，称其游戏让人联想到《Gods: Into the Wonderful》，并希望看到 Claude Code 导出适用于类似移植的工程指南。

**标签**: `#LLM`, `#reverse engineering`, `#Godot`, `#assembly`, `#game development`

---

<a id="item-tech-news-4"></a>
### [K2 Horizon 发布六款开放模型：开放堆栈与模型质量引发讨论](https://ifm.ai/blog/k2/) ⭐️ 7.0/10

K2 Horizon 发布了一个由六款开放模型组成的模型族，主打完全开放的 AI 技术栈，包含源代码、训练数据及其处理方式。社区反响积极，认为这是继 Nvidia Nemotron 之后又一个重要的全开放堆栈玩家。然而，有评论指出其自报性能与评测图表不一致：例如密集 32B 模型明显落后于 Qwen3.8 27B。另有开发者实测 3.7B 小模型后发现其不适合编程任务，会生成错误代码并幻觉出不存在的 API。总之，这次发布在开放性和生态意义上值得关注，但具体模型质量仍需谨慎验证。

hackernews · karimf · 9月3日 15:36 · [社区讨论](https://news.ycombinator.com/item?id=49551760)

**「背景」** K2 Horizon 是 IFM 公司发布的一个完全开源的人工智能模型系列，共包含六个模型，覆盖推理、编码、智能体工作流、边缘设备和部署等不同场景，并提供模型权重、训练代码和数据。所谓“fully open”或“radically open”通常意味着不仅开放模型权重，还公开训练代码和数据处理方式，使外部用户能更完整地了解模型内部机制并用于自托管。除了 IFM 的 K2 Horizon，开放 AI 领域此前较受关注的是 NVIDIA 的 Nemotron，但相比之下 Horizon 系列的基准表现仍需结合自报数据仔细评估。

**「影响」** 对于希望自托管开放权重模型、特别是关注编程能力的开发者和组织，K2 Horizon 的 32B 与 3.7B 模型目前都缺乏可靠证据支持其性能宣称，可能不适合直接用于生产环境。真正有竞争力的是完全开放堆栈的长期价值，而非当前这批模型的即用表现。

**「社区讨论」** Hacker News 评论者普遍欢迎完全开放模型，但认为宣传中的性能声明与实际测试结果不符，且有实测发现 3.7B 模型在基本编程测试中失败并开始幻觉。也有人表示 AI 模型发布速度过快，开始感到“模型疲劳”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ifm.ai/k2/">K2 Horizon: Open-Source AI Models for Every Scale | IFM</a></li>
<li><a href="https://ifm.ai/blog/k2">Introducing K2 Horizon: Frontier Performance, Radically Open</a></li>
<li><a href="https://www.reddit.com/r/LocalLLaMA/comments/1w68rj6/introducing_k2_horizon_frontier_performance/">r/LocalLLaMA on Reddit: Introducing K2 Horizon: Frontier Performance, Radically Open</a></li>

</ul>
</details>

**标签**: `#open-source AI`, `#machine learning`, `#language models`, `#AI benchmarks`, `#self-hosted models`

---

<a id="item-tech-news-5"></a>
### [GPS 受太阳风暴干扰，全美误差最多达 33 英尺](https://www.sciencealert.com/gps-glitched-across-the-us-by-as-much-as-33-feet-scientists-have-never-seen-this-before) ⭐️ 6.0/10

一场太阳风暴导致美国全境 GPS 定位误差最高达 33 英尺（约 10 米），这是科学家此前从未见过的异常事件。该故障影响了依赖高精度导航的技术，包括自动驾驶汽车、电子监控设备和精密农业等。尽管具体影响范围和时间尚不清楚，事件凸显了 GPS 基础设施对空间天气的脆弱性。

hackernews · thread\_id · 9月3日 00:49 · [社区讨论](https://news.ycombinator.com/item?id=49544618)

**「背景」** GPS 信号在传播过程中需要穿过地球电离层，而电离层会受到太阳活动（如日冕物质抛射）的干扰。当太阳喷出的高速带电粒子撞击地球磁层并引发地磁暴时，电离层电子密度会发生变化，使 GPS 信号传播延迟，进而造成定位误差。此次报道的事件中，太阳风暴令美国上空 GPS 定位偏差一度高达约 33 英尺，科学家称此前从未见过如此规模的干扰。

**「影响」** 受 2024 年 5 月太阳风暴影响，美国中西部依赖高精度 GPS 的自动驾驶农机在 5 月 10 日至 11 日期间无法正常导航，导致播种等精准农业作业中断；农业经济学家估算相关损失约为 5 亿美元。依赖 GPS 定位的自动导航系统和相关运营者也需警惕类似空间天气事件带来的定位误差风险。

**「社区讨论」** 讨论中，有人指出 GPS 误差可能使电子监控设备误报位置，导致被软禁者错误地再次入狱；也有人担忧自动驾驶出租车（如奥斯汀的 Cybercab）因此偏离位置。另有一位用户质疑文中“美国农业损失 5 亿美元”的估计缺乏证据，还讨论了 RTK 差分技术能否缓解这类大气扰动影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sciencealert.com/gps-glitched-across-the-us-by-as-much-as-33-feet-scientists-have-never-seen-this-before">GPS Glitched Across The US by as Much as 33 Feet. Scientists Have Never Seen This Before. : ScienceAlert</a></li>
<li><a href="https://www.yahoo.com/news/science/articles/solar-storm-broke-gps-across-142735969.html?fr=sycsrp_catchall">The Solar Storm That Broke GPS Across America By Up ... - Yahoo</a></li>
<li><a href="https://cpaess.ucar.edu/news/nasa-jack-eddy-fellow-quantifies-gps-disruption-2024-solar-storm">NASA Jack Eddy Fellow quantifies GPS disruption of 2024 solar ...</a></li>
<li><a href="https://www.space.com/astronomy/sun/may-2024-solar-storm-cost-usd500-million-in-damages-to-farmers-new-study-reveals">May 2024 solar storm cost $500 million in damages to farmers ...</a></li>

</ul>
</details>

**标签**: `#gps`, `#positioning`, `#solar-storm`, `#autonomous-vehicles`, `#navigation`

---

<a id="item-tech-news-6"></a>
### [申真谞让两子击败 AI KataGo](https://www.kedglobal.com/artificial-intelligence/newsView/ked202607210007) ⭐️ 6.0/10

据报道，韩国围棋棋手申真谞在受让两子的对局中击败了围棋 AI KataGo，被视作人类顶尖棋手在让子条件下运用复杂定式和战略规划战胜超人类围棋 AI 的一次展示。申真谞被评论者描述为实力明显高于其他人类顶尖棋手的现役棋手，其取胜方式涉及走出复杂“飞刀”定式中的一路变化。尽管如此，让两子意味着 AI 仍被视为更强的一方，因此该事件属于突出人类创造力的人机对弈结果，而非 AI 技术层面的突破，也不代表人类在分先条件下能战胜 KataGo。

hackernews · gmays · 9月3日 01:11 · [社区讨论](https://news.ycombinator.com/item?id=49544762)

**「背景」** 围棋是使用 19 路棋盘进行策略对弈的棋类游戏，职业棋手分为九个段位，最高为九段；韩国棋手申真谞目前是世界排名第一、持最高九段段位的人类棋手。KataGo 是当前最强的围棋人工智能之一，在分先对局中通常远强于人类棋手。本次事件发生在申真谞与 KataGo 之间的一场正式“棋圣战”系列赛中，他在受让两子的条件下获胜，并成为已知首位在正式两子让子赛中击败 KataGo 的职业棋手。

**「社区讨论」** 评论者普遍强调申真谞并非普通人类棋手，其历史级评分和远超同侪的实力让这场让子胜更显特别；有人具体解释他利用“飞刀”定式的复杂变化将局面引向均势并获胜。也有评论指出标题可能误导，因为让两子意味着 AI 被公认为更强，分先下人类没有机会；还有人质疑这类人机对抗展本身的意义不大。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kedglobal.com/artificial-intelligence/newsView/ked202607210007">Go grandmaster Shin defeats AI KataGo in historic human victory - KED Global</a></li>
<li><a href="https://www.reddit.com/r/baduk/comments/1v28073/shin_jinseo_defeats_katago_with_a_twostone/">r/baduk on Reddit: Shin Jin-seo defeats KataGo with a two-stone handicap in third game of three, winning 2-1</a></li>
<li><a href="https://gostonebase.com/blog/shin-jinseo-vs-katago-kishin-match/">Humans Strike Back: Shin Jinseo Defeats KataGo 2–1 in the Kishin Match | StoneBase Blog</a></li>

</ul>
</details>

**标签**: `#Go`, `#KataGo`, `#Human vs AI`, `#Game AI`, `#AI`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [非线性记忆冲击模型的价格操纵分类](https://arxiv.org/abs/2609.02447) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · 9月3日 04:00

**「背景」** 瞬时影响模型把非线性函数与记忆核组合起来，而价格操纵是否可能出现取决于两者的组合顺序。作者指出，此前的刚性定理要求记忆核在零点有界，因而无法覆盖奇异核；同时，Gatheral 的慢速双块界只排除了部分可操纵区，问题尚未完整解决。

**「方案」** 作者系统分类了两种组合顺序。若任意瞬时律 f 先作用于交易速率、再通过非零可积 Volterra 核，则所有有限分段常数往返成本非负会迫使 f 为仿射，而在卷积核情形下进一步迫使 f 为线性。证明借助“零体积抖动泵”和两条薄基线读数，适用于奇异核。对幂律冲击 sgn\(x\)\|x\|^δ 配幂律衰减 t^\{-γ\}，作者得出可操纵当且仅当 δ≠1：平方根冲击在每个衰减指数下都可操纵，Gatheral 留下的 δ+γ≥1 安全区塌缩成 δ=1 这条线。若反过来让单调读出作用在记忆之后的冲击状态，则对所有输入和所有读出安全等价于记忆核的完全正性，作者还给出构造性逆命题；例如幂律记忆后的平方根冲击无操纵。远程补偿块进一步表明，具有均匀消失尾部的核使往返安全与全输入安全一致，而永久记忆下两者相差一个显式存储商。这些机制完整分类了双模 Prony 核、一阶时变记忆和稳定全驱动矩阵记忆，并量化了幂律情形中的摩擦、双块相位与切换复杂度。作者总结，标定的指数对都落在可操纵集合中：在没有摩擦时，凹性必须放在记忆之后，而不是记忆之前。

**「启示」** 作者的核心结论是：在非线性瞬时影响模型中，记忆之前的瞬时非线性必须受刚性线性约束，而记忆之后的凹性安全等价于核的完全正性；这为经验上常见的平方根冲击与幂律记忆组合为何易被操纵提供了统一解释。

**标签**: `#price manipulation`, `#transient impact models`, `#Volterra kernels`, `#complete positivity`, `#market microstructure`

---

<a id="item-tech-blog-2"></a>
### [切换摩擦、异质交易期限与长记忆订单流](https://arxiv.org/abs/2609.02525) ⭐️ 7.0/10

rss · arXiv q-fin \(Quantitative Finance\) · 9月3日 04:00

**「背景」** 作者指出，已有的订单流长记忆现象通常被归因于交易者异质性，但缺少对投资者为何缓慢调整头寸表示形式的微观解释。他提出，更换投资组合选择表示形式本身需要成本，因此成交订单流可能比简单随机过程更具持续性。

**「方案」** 作者建立了一个机制：交易者面对异质的切换阈值和机会波动率，形成异质的驻留时间分布。通过更新过程加总，执行权重加权的驻留时间尾部决定了聚合订单流协方差的衰减速度。文章的关键贡献在于，利用首达更新分析导出联合约束：在通常执行权重下，表示切换驻留时间长度层的指数、订单流记忆衰减指数和有限市场缩放必须终止的期限都对应同一尾部。结构模拟能从模拟路径中恢复这些约束，同时显示权重设定错误会扭曲结论，有限横截面会缩短可用的推断期限。由此提出的经验协议将一次聚合持久性拟合转换成跨数据集限制，帮助研究者判断某类基于持续时间的内核是否适合用于另一项执行成本模型。

**「启示」** 作者的核心论点是，订单流长期相关性可以来自投资者切换成本与异质阈值之间的相互作用，而不仅仅来自外生随机冲击。这一机制为连接微观行为、长期记忆和可检验的经验约束提供了统一框架，但作者仍未给出完整实证验证，读者需要参考全文来评估其方法在真实市场数据中的适用性。

**标签**: `#order flow`, `#long memory`, `#trading horizons`, `#renewal processes`, `#execution costs`

---

<a id="item-tech-blog-3"></a>
### [LLM 智能体在双向拍卖市场中的行为与评估框架](https://arxiv.org/abs/2609.02580) ⭐️ 7.0/10

rss · arXiv q-fin \(Quantitative Finance\) · 9月3日 04:00

**「背景」** 大型语言模型（LLM）正越来越多地被部署为经济智能体，但作者指出，目前几乎没有证据表明它们是否适合参与为人类设计的市场机制，以及这些机制在面对 LLM 智能体时能否实现预期效果。该研究通过复制经典经济实验，将人类受试者替换为 LLM 智能体，置于广泛使用的双向拍卖市场环境中，从而检验 LLM 智能体与这一基本市场机制的兼容性。

**「方案」** 作者将 LLM 智能体放入双向拍卖市场，观察其是否能实现资源的有效配置，并将结果与人类市场进行比较。他们发现，由 LLM 智能体构成的市场达到均衡的速度更慢甚至无法收敛，因此资源分配的效率低于人类市场。进一步分析个体交易决策后，结果显示不同模型家族和市场角色之间存在显著异质性。通过对智能体生成的思维链（CoT）痕迹进行词汇分析，作者发现从逐步调整价格转向执行交易的决策，往往伴随着从策略性考量向紧迫感的转变。基于这些发现，作者公开了测试框架，供未来的经济行为评估使用。

**「启示」** 作者的核心论点是，LLM 智能体与面向人类设计的市场机制之间尚未充分对齐，其在双向拍卖中的慢收敛或非收敛行为可能导致资源配置效率低于人类。更大的意义在于，作者提供了一种可复用的评估框架，把“与市场机制的兼容性”纳入 LLM 对齐的研究维度。

**标签**: `#LLM agents`, `#market design`, `#double auction`, `#alignment`, `#economic behavior`

---

<a id="item-tech-blog-4"></a>
### [用机器学习从公开数据度量高频交易](https://arxiv.org/abs/2608.00858) ⭐️ 7.0/10

rss · arXiv q-fin.TR \(Trading &amp; Microstructure\) · 9月3日 04:00

**「背景」** 公开数据通常无法直接识别高频交易（HFT），且传统的代理指标无法区分流动性供给型与流动性需求型 HFT。作者指出，这一度量缺口使研究者难以用公开可得的数据研究 HFT 对市场质量的影响。

**「方案」** 作者基于纳斯达克专有数据训练机器学习模型，将已观测到的 HFT 活动映射到公开的日内变量上，再将该映射应用于全美股票，生成了 2010–2023 年每日的流动性供给型和需求型 HFT 度量。这些度量在相当程度上包含了标准代理指标所反映的信息，并能捕捉后者遗漏的时间序列变化。利用 Euronext Paris 专有数据，作者证明该方法可跨市场推广，且在训练多年后仍保持预测力。基于 14 年面板，研究发现：流动性供给型 HFT 与公告前的信息获取、知情交易增加以及买卖价差下降持续相关，而流动性需求型 HFT 则呈现相反关联。疫情期间，HFT 提供的流动性保持韧性，且其与更低价差的关联有所增强。

**「启示」** 作者的核心论点是：借助机器学习，可以从公开数据构造出行之有效、可持续数年并跨市场推广的 HFT 日度度量，从而把对 HFT 与市场质量关系的探讨扩大到 14 年的长时间维度。这种将专有标签迁移为公开度量的思路，为市场微观结构研究提供了可复用的实证工具。

**标签**: `#high-frequency trading`, `#machine learning`, `#market microstructure`, `#liquidity measurement`

---

<a id="item-tech-blog-5"></a>
### [公开数据下的元订单重构与 LMF 理论检验](https://arxiv.org/abs/2608.30999) ⭐️ 7.0/10

rss · arXiv q-fin \(Quantitative Finance\) · 9月3日 04:00

**「背景」** 市场价格订单流普遍存在长程相关性，Lillo-Mike-Farmer（LMF）订单拆分理论是经典解释，但其定量检验长期依赖包含交易者标识的专有数据，难以复现和跨市场验证。作者想考察是否能用匿名的公开数据重构元订单，从而检验这一理论。

**「方案」** 作者使用约翰内斯堡证券交易所（JSE）市值最大的 239 只股票在 2023 年 1 月 1 日至 2025 年 12 月 31 日期间的交易和报价数据，通过合成元订单重构方法进行网格搜索，并用元订单冲击风格事实和 LMF 关系评估各参数配置。结果显示，以最小化元订单冲击风格事实误差为目标选出的配置，能够复现目标聚合特征，但 LMF 关系拟合较差；而以最小化 LMF 差异为目标选出的配置，虽然能按构造恢复 LMF 关系并保留若干冲击特征，但部分个股层面的执行与衰减拟合较弱。这种不对称结果表明，仅通过恢复聚合冲击风格事实不足以保证 LMF 一致的订单拆分，LMF 定向配置也只是在该重构类别内建立了兼容性，并非独立检验。

**「启示」** 作者认为，研究结果支持 LMF 理论与匿名市场数据的一致性，而非对理论的直接验证；在缺乏交易者标识的情况下，从公开数据中识别订单拆分机制有其内在局限。

**标签**: `#market microstructure`, `#order splitting`, `#metaorder modelling`, `#empirical finance`, `#JSE`

---

<a id="item-tech-blog-6"></a>
### [带仿射漂移随机 Volterra 积分方程的伪平稳理论](https://arxiv.org/abs/2511.03474) ⭐️ 7.0/10

rss · arXiv q-fin \(Quantitative Finance\) · 9月3日 04:00

**「背景」** 带仿射漂移的正向随机 Volterra 积分方程（SVIE）因核函数引入记忆与路径依赖，通常不存在经典意义下的平稳解，长期行为的刻画也因此困难。作者以这类方程为对象，研究其有限时域与长期平稳性质。

**「方案」** 论文的核心概念是“伪平稳 regime”：在扩散、漂移与核结构下，通过显式闭式选取确定性初值φ和均值回复函数μ，或在扩散系数中加入与核相关的确定性稳定因子ς、同时保持μ几乎任意，可使解的所有边际分布具有相同期望与方差。在此基础上，作者证明不同初值对应的解在 p&gt;0 的 L^p 意义下随时间趋于“融合”（confluence），并建立泛函弱长期渐近：时移后的解弱收敛到一族共享相同协方差函数的 L^2 平稳过程。这些结果被用于α∈\(0,1\]时由α-伽马型分数积分核驱动的指数-分数 SVIE，即粗糙路径区域，并据此引入一类稳定的粗糙波动率模型。

**「启示」** 作者表明，即使 SVIE 具有长期记忆，仍可通过伪平稳与融合性质获得可用的长期渐近框架；这为金融中常见但难处理的粗糙波动率模型提供了可分析的平稳化建模路径。

**标签**: `#stochastic Volterra equations`, `#stationarity`, `#long-run asymptotics`, `#rough volatility`, `#mathematical finance`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [英伟达以 129.3 亿美元收购 Hugging Face，加码 AI 软件业务](https://cointelegraph.com/news/nvidia-buys-hugging-face-12-9-billion-ai-software?utm_source=rss_feed&amp;utm_medium=rss&amp;utm_campaign=rss_partner_inbound) ⭐️ 8.0/10

英伟达已同意以 129.3 亿美元收购 AI 模型平台 Hugging Face，该平台拥有超过 1800 万开发者用户，用于共享和部署 AI 模型。

rss · Cointelegraph · 9月3日 12:41

**「背景」** Hugging Face 是一个供开发者分享和部署 AI 模型（尤其是开放权重模型）的平台，常被比作“AI 界的 GitHub”；英伟达此前以 GPU 等 AI 硬件著称，收购这家拥有超过 1800 万开发者的公司，是其向 AI 软件与开发者生态扩张的重要一步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rits.shanghai.nyu.edu/ai/nvidia-hugging-face-acquisition/">NVIDIA Reportedly Buys Hugging Face for $12.9B — llama.cpp...</a></li>
<li><a href="https://finance.yahoo.com/markets/article/nvidia-confirms-13-billion-acquisition-of-open-weight-ai-platform-hugging-face-141058641.html">Nvidia confirms $13 billion acquisition of open-weight AI platform...</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#Hugging Face`, `#acquisition`, `#AI software`, `#mergers and acquisitions`

---

<a id="item-finance-news-2"></a>
### [中国反驳 G20“依赖出口”批评 指其“宣扬保护主义”](https://www.cnbc.com/2026/09/03/china-g20-exports-trade.html) ⭐️ 7.0/10

中国商务部发言人周四反驳 G20 声明中对中国依赖出口的批评，称这“本质上是在宣扬保护主义”。此前，美国财长贝森特表示 19 个 G20 成员同意解决“廉价出口”造成的不平衡，中国是唯一对相关表述提出异议的成员。

rss · CNBC Finance · 9月3日 11:12

**「背景」** 此次交锋发生在中美欧贸易关系紧张之际。美国近期以伊朗为由制裁中国企业，并威胁切断协助伊朗的金融机构与美国金融体系的联系；法国通过旨在限制 Temu 等中国电商低价商品的新法律，欧盟也要求中国在 10 月前就削减贸易逆差拿出“具体成果”。

**标签**: `#China`, `#Trade policy`, `#G20`, `#Protectionism`, `#E-commerce`

---

<a id="item-finance-news-3"></a>
### [澳大利亚加密企业牌照宽限期将于 9 月 30 日结束](https://www.coindesk.com/business/2026/09/03/australia-is-cracking-down-on-crypto-businesses-as-its-strict-new-regulatory-deadline-nears) ⭐️ 7.0/10

澳大利亚证券和投资委员会（ASIC）已收到超过 45 份数字资产相关牌照申请；针对加密企业的临时执法宽限期将在 9 月 30 日到期，届时监管执行将转严。

rss · CoinDesk · 9月3日 10:09

**「背景」** 澳大利亚证券和投资委员会（ASIC）已收到超过 45 份数字资产相关的牌照申请；现有的临时执法宽限期将于 9 月 30 日到期，届时依赖该宽限期的加密货币公司必须申请金融服务牌照，否则可能面临最高相当于年营业额 10%的罚款。

**「影响」** 尚未取得牌照、目前在澳大利亚提供加密资产服务的企业，需要在截止日前完成牌照申请，以规避更严格的执法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.binance.com/en/square/post/09-03-2026-australian-crypto-firms-face-sept-30-deadline-for-licensing-applications-362622322999626">Australian Crypto Firms Face Sept . 30 Deadline for Licensing ...</a></li>
<li><a href="https://crypto.news/australia-gives-crypto-firms-sept-30-licence-deadline/">Australia gives crypto firms Sept . 30 licence deadline</a></li>
<li><a href="https://en.coin-turk.com/asic-sets-sept-30-deadline-for-crypto-firms-to-apply-for-financial-services-license/">COINTURK NEWS - Bitcoin, Blockchain and Cryptocurrency News and...</a></li>

</ul>
</details>

**标签**: `#cryptocurrency`, `#regulation`, `#Australia`, `#compliance`, `#financial-policy`

---

<a id="item-finance-news-4"></a>
### [美股盘前个股波动：Snowflake 大涨 24%，Ultragenyx 暴跌逾 46%](https://www.cnbc.com/2026/09/03/stocks-making-the-biggest-moves-premarket-snow-mrna-avgo.html) ⭐️ 6.0/10

财报、业绩指引和临床试验结果引发美股盘前个股大幅波动：Snowflake 公布的第二季度业绩好于分析师预期，并上调全年产品收入指引，股价大涨 24%；Ultragenyx 治疗 Angelman 综合征（一种罕见遗传神经发育障碍）的药物 III 期试验未达主要终点，股价暴跌逾 46%。

rss · CNBC Finance · 9月3日 11:35

**「背景」** 本轮波动多为公司个体因素而非宏观消息；软件同业也受到 Snowflake 强劲业绩的带动。

**标签**: `#premarket movers`, `#earnings`, `#guidance`, `#biotech`, `#software`

---

<a id="item-finance-news-5"></a>
### [Adobe 宣布新任 CEO 后股价下跌](https://www.marketwatch.com/story/adobe-just-announced-its-next-ceo-heres-why-its-stock-is-dropping-bad9ed8a?mod=mw_rss_topstories) ⭐️ 6.0/10

Adobe 宣布 Anil Chakravarthy 出任下一任 CEO，股价随之下跌，原因是另一名长期业务负责人也将离开，引发市场对领导层进一步变动的担忧。

rss · MarketWatch Top Stories · 9月4日 00:25

**「背景」** Anil Chakravarthy 是 Adobe 的资深高管，但公司同时宣布另一位长期业务负责人即将离任，市场担忧这可能预示领导层会有更多变动。

**「影响」** 投资者担忧 Adobe 高管团队持续流失，导致公司股价承压。

**标签**: `#Adobe`, `#CEO transition`, `#Leadership change`, `#Stock drop`, `#Corporate governance`

---

<a id="item-finance-news-6"></a>
### [Lululemon 转向宽松裤装以应对紧身裤需求降温](https://www.marketwatch.com/story/lululemons-sales-drop-raises-deeper-concerns-about-the-companys-turnaround-ddf9256a?mod=mw_rss_topstories) ⭐️ 6.0/10

Lululemon 销售额下滑并给出令人失望的展望，分析师开始质疑其时尚产品组合。面对顾客对紧身瑜伽裤兴趣减弱，公司正押注“away from body”裤装，即更宽松、不紧贴身体的款式。

rss · MarketWatch Top Stories · 9月4日 00:24

**「背景」** 露露乐蒙（Lululemon）此前以紧身瑜伽裤知名，但近期增长承压。该公司第二季度紧身裤销售额大约下降 20%，而剪裁较宽松的“away from body”（离身剪裁）裤款获得良好反响，公司由此调整产品方向，以应对顾客对贴身裤装兴趣减弱以及业绩指引令人失望带来的质疑。

**「影响」** 杰富瑞分析师 Randal J. Konik 认为，宽松版型流行趋势可能冲击 Lululemon、耐克等运动服饰零售商，同时为李维斯等宽松牛仔品牌带来利好。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ca.finance.yahoo.com/news/no-love-leggings-lululemon-sales-213909301.html">No Love for Leggings? Lululemon Sales Drop Ahead of Heidi...</a></li>
<li><a href="https://wwd.com/sourcing-journal/sj-denim/levi-lululemon-nike-fashion-shift-denim-looser-fits-wider-leg-athletic-apparel-1238836801/">Analyst: Levi’s Loose Fits Could Impact Athletic Apparel Retailers</a></li>

</ul>
</details>

**标签**: `#Lululemon`, `#retail`, `#athleisure`, `#earnings-outlook`, `#fashion trend`

---

<a id="item-finance-news-7"></a>
### [渣打银行在迪拜外汇平台推出比特币和以太币现货交易](https://www.coindesk.com/business/2026/09/03/standard-chartered-first-top-global-bank-to-offer-bitcoin-and-ether-trading-in-uae) ⭐️ 6.0/10

渣打银行表示，它成为首家在迪拜外汇平台上向机构客户提供比特币和以太币现货交易的大型全球银行；目前未披露交易规模或财务条款。

rss · CoinDesk · 9月3日 15:58

**「背景」** 渣打银行此前已于 2025 年 7 月通过其英国分行向机构客户提供比特币和以太币现货交易（即按市场价直接买卖并交割），此次在迪拜国际金融中心推出同类服务，使它成为首家进入阿联酋市场的全球系统重要性银行（G-SIB，指规模大、对全球金融体系影响重大的银行）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tokenpost.com/news/business/22956">Standard Chartered Launches Bitcoin, Ether Spot Trading in UAE</a></li>
<li><a href="https://finance.yahoo.com/markets/crypto/articles/standard-chartered-launches-spot-bitcoin-174300514.html?fr=sycsrp_catchall">Standard Chartered Launches Spot Bitcoin, Ether Trading for ...</a></li>

</ul>
</details>

**标签**: `#Standard Chartered`, `#Cryptocurrency`, `#Dubai`, `#Institutional adoption`, `#UAE`

---