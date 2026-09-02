---
layout: default
title: "Horizon Summary: 2026-09-02 (ZH)"
date: 2026-09-02
lang: zh
---

> 从 118 条内容中筛选出 20 条重要资讯。

---

**科技新闻**
1. [Claude Fable 5.1 与 Mythos 5.1 发布：改进写作与科学，缓存读取降价](#item-tech-news-1) ⭐️ 9.0/10
2. [Dan Luu 对 Zitron AI 预测的细致评估](#item-tech-news-2) ⭐️ 8.0/10
3. [1.5 小时训练的小 Transformer 在 ARC 基准上超越许多 LLM](#item-tech-news-3) ⭐️ 8.0/10
4. [Python 3.15.0 RC2 发布，进入最终测试阶段](#item-tech-news-4) ⭐️ 8.0/10
5. [Google Play 禁止 AnkiDroid 显示 Open Collective 捐赠链接](#item-tech-news-5) ⭐️ 7.0/10
6. [Jujutsu 作者 Martin 加入 ERSC](#item-tech-news-6) ⭐️ 7.0/10

**科技博客**
1. [质量调整后的 AI 推理价格指数：传统方法低估 87%降幅](#item-tech-blog-1) ⭐️ 9.0/10
2. [现实摩擦下的比特币期权对冲：经典方法胜过深度对冲](#item-tech-blog-2) ⭐️ 8.0/10
3. [无需交叉资产协方差的组合风险界与配置规则](#item-tech-blog-3) ⭐️ 8.0/10
4. [神经收缩不定相关矩阵，改善小市值组合](#item-tech-blog-4) ⭐️ 8.0/10
5. [权威与推理分离：智能体金融的可执行边界](#item-tech-blog-5) ⭐️ 8.0/10
6. [电池储能在英国平衡机制中的边际定价作用](#item-tech-blog-6) ⭐️ 8.0/10

**财经新闻**
1. [美联储理事巴尔：若通胀未缓解将支持加息](#item-finance-news-1) ⭐️ 8.0/10
2. [全球债券收益率触及 2008 年以来最高水平](#item-finance-news-2) ⭐️ 8.0/10
3. [美国打击霍尔木兹海峡伊朗目标 油价涨至六周高点](#item-finance-news-3) ⭐️ 8.0/10
4. [SEC 提议更新转账代理规则，并计划讨论美股 24 小时交易](#item-finance-news-4) ⭐️ 8.0/10
5. [Anthropic 350 亿美元 AI 交易包含 Hut 8 得州电力站点](#item-finance-news-5) ⭐️ 8.0/10
6. [特朗普二世关联公司据报牵头 Polymarket 10 亿美元融资，估值 210 亿美元](#item-finance-news-6) ⭐️ 8.0/10
7. [习近平密集外访：出席上合、金砖峰会并预计访美](#item-finance-news-7) ⭐️ 7.0/10
8. [戴尔财报亮眼，AI 服务器需求推动订单积压至 950 亿美元](#item-finance-news-8) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Claude Fable 5.1 与 Mythos 5.1 发布：改进写作与科学，缓存读取降价](https://www.anthropic.com/claude-fable-and-mythos-5-1) ⭐️ 9.0/10

Anthropic 发布了 Claude Fable 5.1 和 Claude Mythos 5.1，宣称改进了散文风格、增强了科学能力，并将缓存读取价格从每百万 token 1 美元降至 0.25 美元，使 Fable 5.1 的缓存读取成本仅为 Opus 的一半。系统卡和平台文档已同步公开。新模型还支持思考力度（低、中、高、极高）设置，但社区反馈指出，在复杂异步工作负载下，模型有时会提前结束回合或描述下一步而非执行，需要额外提示才能完成工作。

hackernews · denysvitali · 9月1日 17:53 · [社区讨论](https://news.ycombinator.com/item?id=49525378)

**「背景」** Claude 是 Anthropic 开发的大语言模型系列。根据背景资料，Anthropic 于 2026 年 6 月 9 日通过 Project Glasswing 发布 Claude Mythos 5，并向公众推出 Claude Fable 5，其中 Fable 增加了针对网络安全等高风险领域的额外安全护栏；Mythos 类别被描述为高于 Opus 的能力层级。Claude Fable 5.1 和 Claude Mythos 5.1 是该系列的新版本，主要在写作风格、科学表现和缓存读取价格上带来变化。

**「影响」** 对于依赖长上下文和缓存的开发者，缓存读取成本的大幅下降将直接降低使用成本；如果 Fable 5.1 的整体定价未同步调整，这一价格变化也可能反映 Anthropic 在根据市场反馈调整缓存相关定价策略。

**「社区讨论」** Anthropic 员工认为 Fable 5.1 的写作风格比以往更自然、更少模板化，且能更可靠地遵循风格指令；但也有评论指出，除去终端科学基准后难以看到明显提升，同时多人在实际使用中观察到模型在复杂异步任务中需要额外提示以避免提前结束。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_%28AI%29">Claude (AI) - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-1">Introducing Claude Fable 5 . 1 and Claude Mythos 5 . 1 \ Anthropic</a></li>
<li><a href="https://kie.ai/blog/what-is-claude-fable-5-1">What Is Claude Fable 5 . 1 ? Mythos -Class Claude Explained</a></li>

</ul>
</details>

**标签**: `#anthropic`, `#claude`, `#llm`, `#ai-models`, `#machine-learning`

---

<a id="item-tech-news-2"></a>
### [Dan Luu 对 Zitron AI 预测的细致评估](https://danluu.com/zitron/) ⭐️ 8.0/10

Dan Luu 发表了一篇系统性分析，逐一核对科技评论员 Ed Zitron 关于 AI 的怀疑论预测，并对其准确度给出基于数据的细致评估。文章被看作对 AI 行业争论的重要补充，既非单纯炒作也非末日论。评论中的讨论显示，Zitron 的预测主要涉及模型能力是否见顶、AI 实验室用户与收入增长是否停滞，以及泡沫是否破裂等问题。由于原文未提供完整细节，文章的具体结论与每条预测的判定仍需以原始内容为准。

hackernews · jatins · 9月1日 18:35 · [社区讨论](https://news.ycombinator.com/item?id=49526069)

**「背景」** Ed Zitron 是一位知名的 AI 怀疑论者，经常批评科技行业对 AI 的过度炒作，并做出许多关于模型能力见顶、AI 公司增长停滞的预测。Dan Luu 在文章中逐条核查这些预测，并指出即使一些 AI 狂热者的预测也常出错，但这并不能证明 Zitron 的预测就正确。该分析基于具体数据和注释，与社区中关于 Zitron 立场与 AI 行业宣传的讨论形成对照。

**「影响」** 根据外部评估，Ed Zitron 关于 AI 能力达到顶峰和用户/收入增长停滞的具体预测大多未能实现，甚至他在效率提升问题上公开承认过一次错误，这削弱了他作为 AI 怀疑论声音的公信力；但他关于 AI 投资回报不足的经济学批评仍在技术社区引发广泛讨论。

**「社区讨论」** 评论区对评估方法存在明显分歧：有读者认为 Luu 仅以“错误”回应“能力见顶”等主张，说服力不足；另一些人则认为 Zitron 已变成他所批评的 AI 鼓吹者的镜像，受众让他难以承认失误。还有评论建议对 Altman、Amodei 等业界领袖做类似预测审计，并指出文章未讨论大型云厂商把对 Anthropic/OpenAI 的投资增值计入“其他收入”的问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49526069">How accurate have Ed Zitron&#x27;s AI skeptic predictions been? | Hacker News</a></li>
<li><a href="http://danluu.com/zitron/">How accurate have Ed Zitron&#x27;s AI skeptic predictions been?</a></li>
<li><a href="https://www.drjoshcsimmons.com/writing/ed-zitron-ai-predictions">Ed Zitron &#x27;s AI Predictions : What He Got Wrong · Josh C. Simmons</a></li>
<li><a href="https://aiuntethered.com/news/ed-zitron-ai-return-on-investment-debate/">Ed Zitron Claims AI Lacks Return on Investment—Is He... | AiUntethered</a></li>

</ul>
</details>

**标签**: `#AI skepticism`, `#AI progress`, `#prediction accuracy`, `#technology analysis`, `#Ed Zitron`

---

<a id="item-tech-news-3"></a>
### [1.5 小时训练的小 Transformer 在 ARC 基准上超越许多 LLM](https://mvakde.github.io/blog/44-on-arc-1/) ⭐️ 8.0/10

一位作者发布博客称，仅用 1.5 小时从头训练的小型自回归 Transformer，在 ARC 推理基准上取得了超过许多大型语言模型的结果。作者强调这并非 LLM，而是一个小型 Transformer，并认为极其复杂的问题不一定需要 LLM 来解决。该结果引发关于样本效率和架构选择的讨论，作者将性能提升归因于现代架构（如 SwiGLU、RMSNorm）、更多数据多样性、更好的数据混洗以及将层数从 4 层扩展到 8 层。该实验表明，在不依赖大规模训练计算的前提下，小模型可能在特定基准上具备竞争力。

hackernews · porridgeraisin · 9月1日 09:52 · [社区讨论](https://news.ycombinator.com/item?id=49519939)

**「背景」** ARC（抽象与推理语料库）是一个视觉程序合成基准，用于测试机器的分布外泛化能力；它不依赖特定任务，而是根据少量演示（通常每个任务三个示例）解决未知任务。该基准被广泛用于衡量 AI 的抽象与推理能力，此前主要由 LLM 或其微调版本以巨大的训练成本参与竞争。围绕这一基准的讨论常涉及样本效率：现代 LLM 的样本效率很低，而小模型若能以极低计算成本超越它们，将挑战对算力和架构的既有假设。

**「影响」** 对 AI/ML 从业者而言，这一结果意味着在特定推理任务上，小型 Transformer 可能以极低的训练成本匹敌或超越更大模型，促使社区重新审视“越大越好”的假设以及训练数据与架构设计的重要性。

**「社区讨论」** 在 Hacker News 讨论中，作者澄清这不是 LLM，并解释 ARC 是元学习基准，因此从评估谜题中学习并不等于“在测试标签上训练”。一些评论者认可作者提出的样本效率问题，但也有观点认为“挤柠檬”式的架构调优是最后手段，建议先证明新方法本身能接近最先进水平，再进行细节优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lab42.global/arc/">About ARC – Lab42</a></li>
<li><a href="https://arc-visualizations.github.io/">H- ARC</a></li>
<li><a href="https://www.emergentmind.com/topics/abstraction-and-reasoning-corpus-arc">Abstraction and Reasoning Corpus ( ARC )</a></li>

</ul>
</details>

**标签**: `#transformer`, `#LLM`, `#efficiency`, `#ARC benchmark`, `#machine learning`

---

<a id="item-tech-news-4"></a>
### [Python 3.15.0 RC2 发布，进入最终测试阶段](https://simonwillison.net/2026/Sep/1/python-315-rc-2/) ⭐️ 8.0/10

Python 3.15.0 候选版本 2（RC2）已发布，由 Python 3.14 和 3.15 的发布经理 Hugo van Kemenade 宣布。这是 10 月正式版发布前的最后一个候选版本，进入该阶段后只允许明确的 bug 修复。官方强烈建议第三方 Python 项目在此期间进行兼容性测试，并在 PyPI 上发布 Python 3.15 wheel；基于 RC 构建的二进制 wheel 也将兼容未来的 Python 3.15 版本。目前 GitHub Actions 尚未提供该 RC 版本，但可通过 setup-python 的 allow-prereleases 和 check-latest 标志，在测试矩阵中自动跟随 RC1→RC2→正式版的更新。Simon Willison 提醒开发者应在 RC 阶段运行测试套件，以免像 Python 3.10 那样让已存在的 bug 进入正式发布。

rss · Simon Willison · 9月1日 14:59

**「背景」** Python 3.15 是 Python 3.14 之后的下一个主要版本，目前已进入最终发布候选阶段；这一阶段只允许合入经过审查的明确 bug 修复，第三方项目维护者被强烈建议在此期间准备好 3.15 兼容性，并在 PyPI 发布 3.15 wheel。根据官方时间表，3.15.0rc2 已于 2026 年 9 月 1 日发布，最终 3.15.0 计划于 10 月发布；基于 RC 构建的二进制 wheel 仍可兼容未来的 3.15 版本。新版本的主要变更包括 PEP 810 等对 3.14 的改进。

**「影响」** 第三方 Python 项目维护者应在本阶段针对 3.15 运行测试并发布 wheel，以确保 10 月正式发布时的生态兼容；使用 GitHub Actions 的用户可先通过 allow-prereleases 和 check-latest 配置自动跟踪测试版本，从而及时发现问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.python.org/3.15/whatsnew/3.15.html">What&#x27;s new in Python 3.15 — Python 3.15.0rc2 documentation</a></li>
<li><a href="https://www.python.org/downloads/release/python-3150rc1/">Python Release Python 3.15.0rc1 | Python.org</a></li>

</ul>
</details>

**标签**: `#Python`, `#release candidate`, `#software engineering`, `#programming`, `#ecosystem`

---

<a id="item-tech-news-5"></a>
### [Google Play 禁止 AnkiDroid 显示 Open Collective 捐赠链接](https://github.com/ankidroid/Anki-Android/issues/21656) ⭐️ 7.0/10

开源项目 AnkiDroid 的一项 GitHub issue 报告称，Google Play 已不再允许其应用页面显示 Open Collective 捐赠链接。这一政策变化引发了对应用商店控制权和开源项目筹资方式的讨论。社区评论提到，Google 过去也曾对 WireGuard 采取类似措施，并指出 Play 支付政策涉及“免税捐赠”的规定；但由于未提供原始政策文本，具体条款仍不明确。此事可能影响 AnkiDroid 通过 Play 商店触达用户并进行捐赠筹款的能力。

hackernews · hexa555 · 9月1日 10:11 · [社区讨论](https://news.ycombinator.com/item?id=49520022)

**「背景」** Google Play 对应用内捐赠有政策限制，通常只允许面向具有美国 501\(c\)\(3\) 免税身份的基金会进行捐赠。AnkiDroid 通过 Open Collective 接受捐赠，而 Open Collective 拥有的是 501\(c\)\(6\) 身份，不符合 Google Play 的要求，因此其捐赠链接被移除。该问题已在 AnkiDroid 的 GitHub Issue 中提出并引发社区讨论。

**「影响」** 对 AnkiDroid 这一定位于 Play 商店分发的开源项目而言，失去展示 Open Collective 捐赠链接的资格，可能直接削弱其从 Android 用户群体获得捐赠的渠道；这种政策也可能促使更多开源项目重新评估对单一应用商店分发和筹款通道的依赖。

**「社区讨论」** 评论中既有对 Google 应用商店垄断权力的批评（例如引用 2019 年 WireGuard 被下架的案例），也有对捐赠税务身份的技术性辨析：AnkiDroid 通过 Open Collective 的 501\(c\)\(6\) 组织运作，虽然组织本身免税，但捐赠对捐赠人而言并不可抵税，这与 Google 所说的“免税捐赠”可能并不一致。此外，有用户表达对 AnkiDroid 的感谢并表示会捐款，也有评论将话题引向 PWA 安装限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49520022">AnkiDroid : Google Play no longer allowing Open Collective ...</a></li>
<li><a href="https://github.com/ankidroid/Anki-Android/issues/21656">[Community Help Needed] Google Play : no longer allowing our Open ...</a></li>
<li><a href="https://www.drweb.de/google-play-ankidroid-spendenlink/">Warum blockiert Google Play den Spendenlink von AnkiDroid ?</a></li>

</ul>
</details>

**标签**: `#google-play`, `#open-source`, `#donations`, `#policy`, `#android`

---

<a id="item-tech-news-6"></a>
### [Jujutsu 作者 Martin 加入 ERSC](https://ersc.io/blog/martin-joins-ersc) ⭐️ 7.0/10

Jujutsu（jj）版本控制系统的创建者 Martin 已加入 ERSC，一个新兴的 GitHub 竞争平台。ERSC 官方博客发布了这一消息；jj 是一款与 Git 互操作的现代版本控制工具，以可撤销操作和更灵活的分支工作流著称。作者 Steve Klabnik 在评论中表示与 Martin 合作愉快，并称很快会有更多消息。此次人事加入使 ERSC 在开发者工具领域的意图更加明确，但具体产品方向尚未公布。

hackernews · steveklabnik · 9月1日 17:46 · [社区讨论](https://news.ycombinator.com/item?id=49525297)

**「背景」** Martin von Zweigbergk 是版本控制系统 Jujutsu（简称 jj）的创建者，曾在 Google 工作 15 年。他现已加入 East River Source Control（ERSC）并担任首席技术官，负责领导该公司下一代版本控制平台的工程工作。ERSC 是一家新兴的 GitHub 竞争对手，致力于提供替代性的代码托管和协作服务。

**「影响」** 目前公开信息仅确认 Martin 加入 ERSC，尚未披露具体职责或产品路线图，因此对 jj 用户和 ERSC 用户尚无直接可验证的功能影响。

**「社区讨论」** 评论中，有用户认为 jj 的撤销和变更管理体验比 Git 更顺手，也有人质疑在 Git 已覆盖所有能力的情况下 jj 只是新的交互层，并认为 ERSC 尚未说明如何解决 GitHub 的缺陷；Steve Klabnik 则回应称与 Martin 合作愉快，很快会有更多消息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ersc.io/blog/martin-joins-ersc">East River Source Control Names Jujutsu Creator Martin von... // ERSC</a></li>

</ul>
</details>

**标签**: `#jujutsu`, `#version-control`, `#developer-tools`, `#ersc`, `#open-source`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [质量调整后的 AI 推理价格指数：传统方法低估 87%降幅](https://arxiv.org/abs/2608.29843) ⭐️ 9.0/10

rss · arXiv q-fin \(Quantitative Finance\) · 9月1日 04:00

**「背景」** 作者指出，AI 推理服务的挂牌价格自 2024 年持续下降，但统计机构常用的匹配模型法只按相同模型比价，无法反映质量变化。

**「方案」** 为纠正这一点，作者用公开数据构建质量调整价格指数：面板包含 21,024 条报价、3,208 个模型和 86 家服务商，并接入 4,605 项基准评分，通过潜在质量指数把基准表现当作“质量阶梯”来替代传统产品特征。结果显示，匹配模型法测得价格每年下降 0.10 个对数点，质量调整后则下降 0.73 个对数点，意味着 87%的降幅被现行方法掩盖。若按完成任务计费，买家价格实际上已停止下降，因为推理模型消耗 token 的速度快于 token 单价下跌，买卖双方价格因而分化。作者还做了一组预注册有效性审计：剔除有污染风险的基准后，模型排序依然高度稳定（相关度 0.998），但价格指数每年变动 0.49 个对数点，说明基准排行榜的稳定性并不能为基于基准的经济统计提供辩护。全文所需数据均来自公开来源且零成本可复现。

**「启示」** 作者的结论是，AI 推理市场的真实价格下降远比传统统计显示的迅猛，而质量调整方式会从根本上改变对竞争、集中度和生产率的度量。

**标签**: `#AI economics`, `#quality-adjusted price index`, `#benchmarking`, `#inference pricing`, `#reproducibility`

---

<a id="item-tech-blog-2"></a>
### [现实摩擦下的比特币期权对冲：经典方法胜过深度对冲](https://arxiv.org/abs/2608.29025) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · 9月1日 04:00

**「背景」** 经典期权对冲方法（如 Black-Scholes delta）假设可以持续且无成本地再平衡，这在真实市场中并不成立。深度对冲通过神经网络直接处理交易成本等摩擦，此前的研究报告了不错的结果，但往往只与无摩擦的经典基线在模拟数据上比较，这种对比并不公平，也让人质疑其优势是否真实存在。

**「方案」** 作者使用 Deribit 上 2020 至 2024 年五年的真实比特币期权数据，在同一 5 个基点的交易成本下比较了六种策略：Black-Scholes delta、Leland 成本调整对冲、Whalley-Wilmott 无交易带，以及三种深度对冲设置（LSTM 和前馈网络，均使用 CVaR 损失，部分运行中加入交易频率惩罚）。在 2023 年 9 月至 2024 年 12 月的 11,546 个测试片段中，Whalley-Wilmott 相比小时级再平衡显著降低了交易成本，每个片段相对普通 BS delta 节约 1.79 美元（95% CI \[-2.21, -1.39\]，p&lt;0.0001），交易次数约为其八分之一；其 P&amp;L 和尾部风险指标也更好，但在该样本量下尚不显著。三种深度对冲模型在任何指标上都没有击败任何经典基线，而且无论惩罚权重如何，它们几乎每小时都在交易，即使权重变化二十倍也几乎没有改变行为。在较为平静的验证期内，Whalley-Wilmott 的 P&amp;L 优势缩小甚至消失，但成本优势仍然存在，说明结果依赖市场状态。作者认为可能的原因是训练集较小，以及所测试的架构缺乏“按兵不动”的内在机制。

**「启示」** 作者用一个不“华丽”但诚实的真实数据检验表明，在现实摩擦下经典 Whalley-Wilmott 无交易带仍然有效，而深度对冲的优势在这一真实市场环境中并未得到验证。评估对冲模型时应使用公平的经典基线和真实摩擦条件，并注意结果对市场状态的依赖。

**标签**: `#deep hedging`, `#bitcoin options`, `#transaction costs`, `#empirical study`, `#deribit`

---

<a id="item-tech-blog-3"></a>
### [无需交叉资产协方差的组合风险界与配置规则](https://arxiv.org/abs/2608.29692) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · 9月1日 04:00

**「背景」** 传统组合风险评估依赖对跨资产收益协方差矩阵的可靠估计，但在样本短、维度高的面板中，这类估计很难获得。作者试图绕过这一瓶颈，用企业层面的分布值特征来为组合风险提供单边证书。

**「方案」** 作者指出，在特征与系统性暴露、暴露与收益之间存在既定联系的条件下，多企业 Wasserstein-2 离散度可以给出系统性组合方差的尖锐上界，以及对标准化收益的相应界。通过加权两两松弛，目标函数在可检验条件下是凸的，并且只需要边际波动尺度，完全不需要跨资产收益协方差。在 2018—2022 年 52 家公司面板中，基于 Qwen3-Embedding-8B 新闻表示构建的配置，其样本内方差百分位落在四个预设封顶组合总体的 0.69 至 1.33 之间，而等风险加权的百分位在 21.1 至 28.6 之间；该优势在冻结语言模型表示下依然存在。作者还说明，当企业特定松弛为零时，公共映射尺度只会改变已认证的方差缩减量，不会改变归一化配置，后者仅由观测到的信息几何决定。

**「启示」** 作者的核心贡献是将分布值企业信息整合为一致的风险界和无需交叉资产协方差即可实施的配置规则，为短高维面板下的组合风险认证提供了新的可行路径。

**标签**: `#portfolio risk`, `#language models`, `#Wasserstein distance`, `#quantitative finance`, `#machine learning`

---

<a id="item-tech-blog-4"></a>
### [神经收缩不定相关矩阵，改善小市值组合](https://arxiv.org/abs/2608.30446) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · 9月1日 04:00

**「背景」** 包含小市值股票的股票池常有新上市和间歇交易证券，若强制统一回溯窗口会丢弃大量信息。成对完整估计能保留每对资产最长重叠，但不同样本计算的矩阵可能不定，无法直接用于 Markowitz 优化，也超出标准随机矩阵收缩的假设。

**「方案」** 作者提出适配该场景的旋转不变神经协方差估计器：模型先计算掩码感知的边际矩和成对相关代理，处理其带符号谱，并用双向 GRU 以因子对齐的有效样本长度（来自重叠矩阵和特征向量载荷）为条件，把所有特征值（包括负值）映射到正逆谱。重建的协方差矩阵正定，并以最小化五日已实现全局最小方差风险进行端到端训练。在 2000—2025 年的 26 年滚动外样本回测中，覆盖最多 1500 只美国股票、含收盘竞价撮合及佣金、融资、公司行动和市场冲击等摩擦，该估计器相较次优协方差估计器将年化五日波动率降低约 20%，夏普比率提高约 40%；99.9%的 Model Confidence Set 只保留该神经模型，说明改善在统计上显著且稳健。

**「启示」** 作者的核心结论是：用端到端学习直接修复成对完整相关矩阵的不定性，能以不丢弃信息的方式利用小市值数据，并显著优于传统协方差估计。

**标签**: `#covariance estimation`, `#neural networks`, `#portfolio optimization`, `#pairwise-complete correlation`, `#small-cap equities`

---

<a id="item-tech-blog-5"></a>
### [权威与推理分离：智能体金融的可执行边界](https://arxiv.org/abs/2608.30519) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · 9月1日 04:00

**「背景」** 作者指出，AI 智能体可以自行选择工具、交易对手和交易参数，但“推理”本身不应直接赋予执行金融操作的权力。现有依赖提示词约束的基线方案并不充分：在测试中，直接智能体基线接受了全部 36 个攻击效果，提示词策略基线也接受了 20 个。

**「方案」** 为此，作者提出“权威-推理分离”（AIS）架构，把金融行动意图作为控制对象：机器生成的提案只有在经过独立确定性控制平面验证后，才能获得临时可执行权威。验证内容包括已注册的智能体身份、可问责的所有者、授权与风险偏好来源、策略版本、状态、审批以及精确的经济语义。之后，区块链可以执行被授予权威的操作表示，并记录可移植的结算证据，而机构合法性、服务交付、会计分类和人员问责仍属于链下义务。评估采用四领域实例、BIS 与 MAS 官方案例、48 个固定测试的可执行原型，以及公共账本可观测性测试。结果显示，AIS 在 36 个合成授权攻击中零通过，同时接受了全部 8 个合法固定测试，拒绝了所有令牌重放和收款方/渠道替换，在服务交付失败时扣留完成操作，并填满了全部 13 个预定义证据字段；对 1700 笔 Base 交易的测试则表明，公共账本能够证明结算和部分授权参数，但无法确立机构授权、法律问责、服务交付或会计处理。

**「启示」** 作者的结论是，AIS 与区块链相辅相成：AIS 决定特定意图能否行动，区块链则让被授予的权威变得有界、可执行且可独立观察。将推理能力与执行权威彻底分离，是构建安全智能体金融系统的核心设计启示。

**标签**: `#agentic AI`, `#blockchain`, `#financial security`, `#authorization control`, `#intent architecture`

---

<a id="item-tech-blog-6"></a>
### [电池储能在英国平衡机制中的边际定价作用](https://arxiv.org/abs/2608.29818) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · 9月1日 04:00

**「背景」** 英国发电结构中可再生能源已占主导，但很少处于边际定价位置；随着燃气和抽水蓄能等传统调节手段逐渐被替代，实时价格形成由哪些灵活技术决定成为核心问题。作者通过重构英国平衡机制（BM）中按价格排序的合格报价/投标堆栈，研究 2023 至 2025 年 50,684 个半小时结算周期。

**「方案」** 研究将边际性区分为长期系统 bid-active 和短期系统 offer-active 两种情况，并保留共同边际的并列联系。数据显示，电池在投标侧边际活动占比从 0.8%升至 36.2%，在报价侧从 3.2%升至 26.9%，挤掉了联合循环燃气（投标侧）和抽水蓄能（报价侧）。按容量标准化的边际捕获率两侧均上升；机组-季度固定效应估计，每增加 100 MW 活跃容量，季度投标侧和报价侧边际份额分别提高 0.55 和 0.48 个百分点。到 2025 年，同一阶梯上电池动作比数量匹配的非电池替代方案每 MWh 便宜约 9 至 10 英镑，但在短期系统价格最高的 5%时段，电池占比仍低 12.9 个百分点。作者认为单个电池仍符合价格接受者行为，而整个电池舰队已内生于日常平衡定价过程。

**「启示」** 作者的核心结论是，电池储能已不再只是被动的灵活性资源，而是英国平衡机制中举足轻重的边际定价者；其对边际报价的参与系统性地压低了实时平衡价格，但在极端短缺时段参与不足，提示高可再生能源系统中储能对价格形成的双重影响。

**标签**: `#battery storage`, `#balancing mechanism`, `#electricity price formation`, `#empirical analysis`, `#GB electricity market`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美联储理事巴尔：若通胀未缓解将支持加息](https://www.cnbc.com/2026/09/01/fed-governor-barr-says-hell-support-rate-hike-if-inflation-doesnt-ease.html) ⭐️ 8.0/10

美联储理事迈克尔·巴尔表示，如果通胀没有充分缓解，他将支持加息。市场目前预计本月加息概率约 66%，最新通胀同比上涨 3.7%（剔除食品和能源后为 3.3%）。

rss · CNBC Finance · 9月1日 14:01

**「背景」** 美联储 7 月将基准利率维持在 3.5%-3.75%区间，巴尔支持了这一决定；作为联邦公开市场委员会（FOMC）常任投票委员，他的表态与主席沃什上周被市场解读为倾向加息的讲话相呼应。

**标签**: `#monetary policy`, `#Federal Reserve`, `#inflation`, `#interest rates`, `#Michael Barr`

---

<a id="item-finance-news-2"></a>
### [全球债券收益率触及 2008 年以来最高水平](https://www.marketwatch.com/story/this-could-be-the-10-year-treasurys-tipping-point-into-the-danger-zone-891cd45d?mod=mw_rss_topstories) ⭐️ 8.0/10

全球债券市场持续遭抛售，债券收益率已触及 2008 年以来的最高水平。

rss · MarketWatch Top Stories · 9月1日 20:36

**「背景」** 10 年期美国国债收益率被广泛视为长期宏观经济预期和整体借贷成本的风向标。工具数据显示 2026 年 8 月 27 日该收益率约为 4.67%，处于 2008 年以来全球债券收益率的最高水平附近，意味着政府、企业和家庭的融资成本随之上升。

**「影响」** 这将推高家庭、企业和各国政府的借贷成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/United_States_Treasury_security">United States Treasury security - Wikipedia</a></li>
<li><a href="https://tradingeconomics.com/united-states/government-bond-yield">US 10 Year Treasury Note Yield - Quote - Chart - Historical Data - News</a></li>

</ul>
</details>

**标签**: `#Treasury yields`, `#global bonds`, `#borrowing costs`, `#interest rates`, `#market rout`

---

<a id="item-finance-news-3"></a>
### [美国打击霍尔木兹海峡伊朗目标 油价涨至六周高点](https://www.marketwatch.com/story/global-oil-prices-extend-move-over-90-after-report-of-two-tankers-struck-in-hormuz-0effd708?mod=mw_rss_topstories) ⭐️ 8.0/10

全球油价周二收于近六周高点，此前美国军方表示在霍尔木兹海峡打击了伊朗目标，以回应德黑兰对通行船只的夜间袭击。

rss · MarketWatch Top Stories · 9月1日 20:13

**「背景」** 霍尔木兹海峡是伊朗与阿曼之间的狭窄水道，全球大量石油经由这里运输。在周二美军发动打击前，已有商船在该海峡遇袭，美国政府也重新对伊朗石油出口实施制裁。

**「影响」** 油价上涨可能推高家庭和企业的燃料成本；分析人士警告，若冲突持续，能源供应中断可能给全球经济增长和通胀带来风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2026_Strait_of_Hormuz_crisis">2026 Strait of Hormuz crisis - Wikipedia</a></li>
<li><a href="https://www.ndtvprofit.com/world/us-launches-fresh-strikes-on-iran-hours-after-oil-tankers-in-hormuz-come-under-attack-brent-jumps-to-94-11988911">US Launches Fresh Strikes On Iran Hours After Oil Tankers In Hormuz Come Under Attack; Brent Jumps To $94</a></li>
<li><a href="https://corporate.vanguard.com/content/corporatesite/us/en/corp/articles/potential-impact-high-oil-prices-economies.html">The potential impact of high oil prices on economies</a></li>
<li><a href="https://theconversation.com/why-surging-oil-prices-are-a-shock-for-the-global-economy-but-not-yet-a-crisis-277228">Why surging oil prices are a shock for the global economy - but not yet ...</a></li>
<li><a href="https://www.niesr.ac.uk/blog/global-macroeconomic-impact-recent-surge-energy-prices">The Global Macroeconomic Impact of the Recent Surge in Energy Prices</a></li>

</ul>
</details>

**标签**: `#oil prices`, `#geopolitics`, `#Strait of Hormuz`, `#U.S.-Iran conflict`, `#energy markets`

---

<a id="item-finance-news-4"></a>
### [SEC 提议更新转账代理规则，并计划讨论美股 24 小时交易](https://www.coindesk.com/policy/2026/09/01/sec-proposes-transfer-agent-rule-sets-event-to-figure-out-round-the-clock-u-s-trading) ⭐️ 8.0/10

美国证券交易委员会（SEC）提出一项转账代理规则更新提案，以现代化自 1980 年代以来基本未变的规则，涉及区块链记录保存、代币化证券和自动化市场基础设施。同时，SEC 宣布将举办活动，探讨美国股市全天候交易的可能性。

rss · CoinDesk · 9月1日 23:55

**「背景」** 美国证券交易委员会（SEC）提出修订自 1970 年代末以来基本未变的过户代理规则，明确纳入区块链、代币化证券和智能合约等新技术，并考虑允许过户代理使用区块链作为正式记录。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://crypto.news/sec-proposes-transfer-agent-for-tokenized-securities/">SEC proposes transfer agent overhaul for tokenized securities</a></li>
<li><a href="https://www.binance.com/en/square/post/09-01-2026-sec-proposes-rule-update-to-include-blockchain-and-tokenized-securities-362057034344537">SEC Proposes Rule Update to Include Blockchain and Tokenized ...</a></li>
<li><a href="https://blocknews.com/sec-moves-to-modernize-transfer-agent-rules-here-is-what-could-change/">SEC Moves to Modernize Transfer Agent Rules – Here Is What Could...</a></li>

</ul>
</details>

**标签**: `#SEC`, `#regulation`, `#market structure`, `#transfer agent`, `#trading hours`

---

<a id="item-finance-news-5"></a>
### [Anthropic 350 亿美元 AI 交易包含 Hut 8 得州电力站点](https://www.coindesk.com/tech/2026/09/01/hut-8-s-texas-power-site-sits-inside-anthropic-s-usd35-billion-ai-deal) ⭐️ 8.0/10

据 CoinDesk 报道，Anthropic 一项 350 亿美元的 AI 交易包含了 Hut 8 位于得克萨斯州的电力站点。

rss · CoinDesk · 9月1日 12:11

**「背景」** 据报道，Anthropic 与英伟达支持的 Lambda 达成一项 350 亿美元的云计算容量协议，其中部分容量将运行于 Hut 8 在得克萨斯州的 Beacon Point 园区。该园区有两笔合计 196 亿美元的长期租约，远超 Hut 8 最近一个季度的营收，反映出 AI 公司争抢电力和数据中心容量的趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.coindesk.com/tech/2026/09/01/hut-8-s-texas-power-site-sits-inside-anthropic-s-usd35-billion-ai-deal">BTC news: Anthropic’s $35 billion AI deal runs through a bitcoin miner’s Texas campus</a></li>
<li><a href="https://coinspectator.com/other/2026/09/01/hut-8s-texas-power-site-sits-inside-anthropics-35-billion-ai-deal/">Hut 8’s Texas power site sits inside Anthropic’s $35 billion AI deal – CoinSpectator – Real-time Cryptocurrency News</a></li>

</ul>
</details>

**标签**: `#Hut 8`, `#Anthropic`, `#AI infrastructure`, `#data centers`, `#deal`

---

<a id="item-finance-news-6"></a>
### [特朗普二世关联公司据报牵头 Polymarket 10 亿美元融资，估值 210 亿美元](https://www.coindesk.com/business/2026/09/01/trump-jr-s-firm-leads-usd1-billion-polymarket-raise-at-usd21-billion-value-report) ⭐️ 8.0/10

据报道，与唐纳德·特朗普二世有关联的 1789 Capital 将牵头向预测市场平台 Polymarket 投资 10 亿美元，使该平台估值达到 210 亿美元，略低于竞争对手 Kalshi 的 220 亿美元。

rss · CoinDesk · 9月1日 04:19

**「背景」** Polymarket 是一个基于加密货币的预测市场，用户可就体育、政治等未来事件结果下注；1789 Capital 则是与唐纳德·特朗普 Jr.关联、投资保守派事业的风险投资公司。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Polymarket">Polymarket - Wikipedia</a></li>
<li><a href="https://www.aol.com/news/anti-esg-venture-capital-firm-101701819.html">This is the anti-ESG venture capital firm that Donald Trump Jr .... - AOL</a></li>

</ul>
</details>

**标签**: `#Polymarket`, `#venture capital`, `#prediction markets`, `#cryptocurrency`, `#funding round`

---

<a id="item-finance-news-7"></a>
### [习近平密集外访：出席上合、金砖峰会并预计访美](https://www.cnbc.com/2026/08/31/china-xi-us-trump-visit-sco-brics-modi-india.html) ⭐️ 7.0/10

中国国家主席习近平本周将出席在吉尔吉斯斯坦举行的上合组织峰会，并访问埃及，随后预计出席 9 月 12 日至 13 日的新德里金砖峰会，还可能在 9 月 24 日到华盛顿与特朗普会晤。

rss · CNBC Finance · 9月1日 18:51

**「背景」** 习近平今年此前仅出访朝鲜一次，而上半年有 20 多位外国领导人访问北京；此行正值美中贸易紧张、伊朗战争和 AI 安全风险上升，被视为中国扩大全球角色的信号。

**「影响」** 美国正关注两场峰会；若众议院通过 Graham 法案，继续购买俄罗斯石油的印度可能被征收最高 100%关税，该国近期约 43%的原油仍来自俄罗斯。

**标签**: `#China`, `#Diplomacy`, `#Trade`, `#Oil`, `#Summits`

---

<a id="item-finance-news-8"></a>
### [戴尔财报亮眼，AI 服务器需求推动订单积压至 950 亿美元](https://www.marketwatch.com/story/dells-ai-servers-drive-a-stellar-earnings-performance-and-a-raised-outlook-86476ace?mod=mw_rss_topstories) ⭐️ 7.0/10

戴尔公布强劲财报并上调业绩展望，原因是 AI 服务器需求加速，相关未完成订单（积压订单）已达 950 亿美元。

rss · MarketWatch Top Stories · 9月2日 00:19

**「背景」** 戴尔公布的 2027 财年第二季度业绩显示，调整后每股收益为 7.04 美元，优于预期；公司同时将全年营收指引上调至 1920 亿美元。管理层称，截至季末 AI 服务器积压订单已达 950 亿美元，相当于未来多个季度的产能已被预先锁定，这得益于 AI 服务器需求加速。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://247wallst.com/cards/dell-technologies-q2-2027-earnings-dell-01m1f9r5egqcdb5ba3h8b408w5">Dell Q2 2027: $95 Billion AI Backlog and an Earnings Beat | 24/7 Wall St.</a></li>
<li><a href="https://www.investing.com/news/company-news/dell-q2-fy27-slides-ai-server-backlog-hits-95b-revenue-up-58-93CH-4884718">Dell Q2 FY27 slides: AI server backlog hits $95B, revenue up 58% By Investing.com</a></li>

</ul>
</details>

**标签**: `#Dell`, `#Earnings`, `#AI servers`, `#Outlook`, `#Backlog`

---