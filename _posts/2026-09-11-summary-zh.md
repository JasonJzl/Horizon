---
layout: default
title: "Horizon Summary: 2026-09-11 (ZH)"
date: 2026-09-11
lang: zh
---

> 从 110 条内容中筛选出 20 条重要资讯。

---

**科技新闻**
1. [Forgejo 16.0.3 及之前版本存在严重 RCE 漏洞](#item-tech-news-1) ⭐️ 8.0/10
2. [Rust 成为微软一级语言](#item-tech-news-2) ⭐️ 8.0/10
3. [OpenAI 的 Navier-Stokes 结果附带 Lean 4 证明](#item-tech-news-3) ⭐️ 8.0/10
4. [trynix.dev：在浏览器中运行任意 Nix 包](#item-tech-news-4) ⭐️ 8.0/10
5. [Calif Research 声称演示经微信通话传播的零点击蠕虫](#item-tech-news-5) ⭐️ 8.0/10
6. [Shopify 将移动应用从 React Native 迁回 Swift 和 Kotlin](#item-tech-news-6) ⭐️ 7.0/10

**科技博客**
1. [非强制信息干预减少处方 DDI 错误](#item-tech-blog-1) ⭐️ 7.0/10
2. [从公开数据重建大规模企业间生产网络](#item-tech-blog-2) ⭐️ 7.0/10
3. [The Log S-fBM model: Statistical analysis](#item-tech-blog-3) ⭐️ 6.0/10
4. [Do wind and solar curtail at negative electricity prices? Incentives and evidence across two decades of German renewable support schemes](#item-tech-blog-4) ⭐️ 6.0/10
5. [Signal Correlation, IC, and PnL Dependence](#item-tech-blog-5) ⭐️ 6.0/10
6. [Arbitrage on Decentralized Exchanges](#item-tech-blog-6) ⭐️ 6.0/10

**财经新闻**
1. [Kalshi 获 CFTC 批准，上线黄金和白银永续期货](#item-finance-news-1) ⭐️ 8.0/10
2. [纳斯达克向 Kraken 母公司 Payward 投资 1 亿美元，估值 210 亿美元](#item-finance-news-2) ⭐️ 8.0/10
3. [美国监管机构放宽社区银行监管负担，扩大 18 个月检查周期适用范围](#item-finance-news-3) ⭐️ 7.0/10
4. [Liquid Network resumes block production after $320M exploit](#item-finance-news-4) ⭐️ 7.0/10
5. [The iPhone Duo enters China’s crowded foldable market — and faces a price test](#item-finance-news-5) ⭐️ 6.0/10
6. [OpenAI targets work of Wall Street junior bankers with new ChatGPT for Financial Services](#item-finance-news-6) ⭐️ 6.0/10
7. [Stocks making the biggest moves premarket: Macy&\#x27;s, Meta, Apple, Novartis and more](#item-finance-news-7) ⭐️ 6.0/10
8. [BIS chief warns AI capex arms race relies on opaque debt, posing systemic risks](#item-finance-news-8) ⭐️ 6.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Forgejo 16.0.3 及之前版本存在严重 RCE 漏洞](https://codeberg.org/forgejo/forgejo/src/branch/forgejo/release-notes-published/16.0.4.md) ⭐️ 8.0/10

Forgejo 16.0.3 及更早版本被披露存在严重远程代码执行（RCE）漏洞，官方在 16.0.4 发布说明中提供修复。由于 Codeberg 限流，发布说明一度无法正常读取，社区成员转述的补丁内容显示关键修复是防止模板展开干扰 Git 仓库初始化。该流程会在从模板仓库生成新仓库时克隆模板仓库、删除.git 目录、对.forgejo/template 中列出的文件执行变量模板展开，然后初始化新的 Git 仓库。评论指出 Gitea 不受这两个问题影响，而漏洞影响广泛使用的自托管 Git 服务平台，用户应尽快升级。现有公开讨论尚未展开完整利用细节。

hackernews · weierstass · 9月10日 15:57 · [社区讨论](https://news.ycombinator.com/item?id=49645907)

**「背景」** Forgejo 是一款自托管的 Git 代码托管平台（Git forge，源自 Gitea 的分支），常被团队和开源项目用于自行部署仓库、议题与协作功能。其“模板仓库”功能在基于模板生成新仓库时，会克隆模板仓库、删除 .git 目录、对 .forgejo/template 中列出的文件执行变量模板展开，然后重新初始化一个 Git 仓库，而问题正出在这一流程对指向仓库之外的符号链接处理不当。公开漏洞库将相关缺陷记录为 CVE-2025-68937，描述为符号链接攻击，可写入非预期文件并可能导致攻击者获得服务器 shell 权限；另有 CVE-2026-89094 指出 16.0.4 之前的 Forgejo 可通过构造的模板仓库实现远程代码执行。

**「影响」** 运行 Forgejo 16.0.3 及更早版本的自托管实例管理员应尽快升级到 16.0.4（或 15.0.8），因为 CVE-2025-68937 可让攻击者写入非预期文件并可能获得 shell 访问权限。

**「社区讨论」** 评论中，Gitea 项目领导层成员表示 Gitea 不受这两个问题影响，并强调不应因安全事件羞辱报告者；另有用户抱怨 Codeberg 限流导致发布说明难以访问、建议改用里程碑链接，并讨论禁用 LLM 贡献后攻击者可能更易利用 AI 发现漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2025-68937/">CVE-2025-68937: Forgejo RCE Vulnerability - SentinelOne</a></li>
<li><a href="https://www.rapid7.com/db/vulnerabilities/cve-2026-89094/">CVE-2026-89094: Forgejo: Forgejo before 16.0.4 allows remote ...</a></li>
<li><a href="https://newzino.com/story/forgejo-16-0-3-critical-rce-fa98b4">Forgejo patches critical RCE affecting versions through 16.0.3</a></li>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2025-68937/">CVE-2025-68937: Forgejo RCE Vulnerability</a></li>
<li><a href="https://noise.getoto.net/2026/09/10/forgejo-16-0-4-and-15-0-8-address-critical-security-vulnerability/">Forgejo 16.0.4 and 15.0.8 address critical security vulnerability | Noise</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#Forgejo`, `#open-source`, `#RCE`

---

<a id="item-tech-news-2"></a>
### [Rust 成为微软一级语言](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 8.0/10

根据一篇发布在 Rust 基金会网站上的客座文章，微软已将 Rust 提升为一级语言（tier-1 language）。分析认为，这是 Rust 语言及系统编程生态的一项重要采用里程碑，但该消息本身不包含新的技术突破或版本发布。现有材料没有给出微软内部生效范围、具体产品、版本号或时间表等细节。社区讨论则提到微软有到 2030 年将 10 亿行代码转换为 Rust 的自动化目标，以及 DARPA 在自动化 C 到 Rust 转换方面的工作。

hackernews · mmastrac · 9月10日 13:39 · [社区讨论](https://news.ycombinator.com/item?id=49643546)

**「背景」** 在微软的语境中，Tier-1 语言意味着该语言获得与 C++、C\# 同等级别的官方支持与投入，覆盖工具链、调试和平台集成。Rust 以内存安全为核心设计，旨在减少 C/C++ 代码中常见的内存安全类漏洞，而这类漏洞长期在微软产品报告的 CVE 中占很大比例。尽管微软多年来持续探索将 Rust 用于系统级组件，C++ 凭借数十年的积累和庞大存量代码仍在微软内部占据主导地位。

**「影响」** 对使用微软工具链的开发者和系统编程生态而言，这一认定可能增强 Rust 在 C/C++ 之外用于新项目与既有代码维护的正当性，但实际影响仍取决于微软后续在 MSVC 工具链与具体产品中的落地。

**「社区讨论」** 评论区整体认为这是 Rust 成熟化的重要信号：i2talics 称 Rust 已是能与 C++、C\# 竞争且比 Zig、Odin 更成熟的严肃语言；apatheticonion 以 5 年专业 Rust 经验表示，高层应用开发已难看到其他语言的技术理由；pjmlp 还提到主要操作系统厂商都在为绿色项目多元化系统语言，并出现 MSVC 集成的公开传闻。gregw2 和 devy 则关注微软到 2030 年转换 10 亿行代码、DARPA 的 C 到 Rust 自动化工作，以及内存安全可帮助减少微软产品大量 CVE（评论称约 70% 属内存安全类）的动机。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier - 1 Language at Microsoft</a></li>
<li><a href="https://www.drweb.de/microsoft-rust-tier-1-sprache/">Warum macht Microsoft Rust zur Tier - 1 -Sprache? | Dr. Web</a></li>

</ul>
</details>

**标签**: `#Rust`, `#Microsoft`, `#programming languages`, `#systems programming`, `#open source`

---

<a id="item-tech-news-3"></a>
### [OpenAI 的 Navier-Stokes 结果附带 Lean 4 证明](https://www.johndcook.com/blog/2026/09/09/formal-method-revolution/) ⭐️ 8.0/10

一篇评论文章与 Hacker News 讨论聚焦 OpenAI 与 Navier-Stokes 相关的发布，该发布附带了 Lean 4 形式化证明。由于所给材料只转述该结果，具体证明了什么、证明的完整范围以及独立验证状态仍不明确。讨论的焦点不是单纯宣布数学突破，而是形式化验证的成本、Lean 4 的性能与可审计性，以及 AI 生成数学证明的意义。评论者还比较了智能体生成证明的成本与人类证明工时，并追问新模型能否处理更直接或归纳式的证明。

hackernews · ibobev · 9月10日 21:22 · [社区讨论](https://news.ycombinator.com/item?id=49650326)

**「背景」** 纳维–斯托克斯方程是描述流体运动的核心偏微分方程组，而三维情形下解是否会始终光滑、还是会在有限时间内“爆破”，是克莱数学研究所千禧年大奖难题之一。Lean 4 是一种证明助手，用机器逐行检验数学证明的正确性，因此随发布一同提供的 Lean 代码可用于形式化验证。据现有材料，OpenAI 发布了一篇 166 页的手稿和公开的 Lean 项目，声称解决了该千禧年难题中的 C 与 D 两种情形，相关结论仍待独立评估。

**「影响」** 若该结果成立，最直接的后果是：AI 生成的数学结论将更多以 Lean 4 等形式化验证器作为可信度锚点，从而把可机器检查性变成数学成果发布流程的一部分，而验证环节自身（据现有报道 Navier–Stokes 证明的 Lean 验证约需 17 小时）会成为新的算力与时间瓶颈，数学研究者与定理证明工具社区需据此调整工作流。需注意，所给材料对该成果的描述仍属二手转述，其证明范围与可复现性尚未经独立确认。

**「社区讨论」** 评论区对验证成本与意义看法不一：有人以费马大定理为例称 Lean 验证约需 15 小时和 230GB 内存，而智能体生成 Lean 代码约需 11 天，二者只差约一个数量级；也有人估算智能体成本约 4000 万美元，按 880,000 小时、150 美元/小时计算人类成本约 1.32 亿美元，因此认为“四个数量级”的说法被夸大。另有评论呼吁聚焦实际数学结果、质疑“每页四十小时”的旧经验、追问模型能否做更直接或归纳式证明，并担心未来 AI 证明可能因理解成本过高而无法被人类独立验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.johndcook.com/blog/2026/09/09/formal-method-revolution/">The part of Navier - Stokes no one is talking about</a></li>
<li><a href="https://emergent.sh/news/openai-claims-navier-stokes-millennium-prize">OpenAI Claims Navier - Stokes Millennium Prize Solution</a></li>
<li><a href="https://kingy.ai/blog/navier-stokes-ai-proof-claims-dispute/">OpenAI ’s Navier – Stokes Proof Claim: Evidence and Dispute</a></li>
<li><a href="https://emergent.sh/news/openai-claims-navier-stokes-millennium-prize">OpenAI Claims Navier - Stokes Millennium Prize Solution</a></li>
<li><a href="https://www.johndcook.com/blog/2026/09/09/formal-method-revolution/">The part of Navier - Stokes no one is talking about</a></li>
<li><a href="https://www.1950.ai/post/openai-s-navier-stokes-breakthrough-what-a-90-year-old-mathematics-problem-reveals-about-ai">OpenAI’s Navier - Stokes Breakthrough: What a 90-Year-Old...</a></li>

</ul>
</details>

**标签**: `#Lean 4`, `#formal verification`, `#AI for mathematics`, `#theorem proving`, `#Navier-Stokes`

---

<a id="item-tech-news-4"></a>
### [trynix.dev：在浏览器中运行任意 Nix 包](https://simonwillison.net/2026/Sep/10/trynix/) ⭐️ 8.0/10

Farid Zakaria 发布了 trynix.dev，他称其为自己在 Nix 工作上的“代表作”：该站点通过 qemu-wasm 在浏览器内以 WebAssembly 运行一台 x86\_64 Linux 虚拟机，并能用过去 13 年间的任意 Nix 包启动它。这些环境可以通过 URL 直接寻址，例如打开 https://trynix.dev/?pkg=python3%403.6.2 并点击“Load”，即可获得一个运行 2017 年 Python 3.6.2 的交互式 shell。在此基础上，他还推出了 trynix-preview GitHub Action，它会在 pull request 上评论一个链接，让评审者用 trynix.dev 在浏览器中启动该 PR 的构建，官方描述为“无需服务器，只需浏览器”。对 Nix 与 WebAssembly 生态而言，这使可复现环境变成可交互分享、可链接的对象；不过该帖只是简短的推介，其更广泛的影响仍有待观察。

rss · Simon Willison · 9月10日 23:44

**「背景」** Nix 及其软件包集合 nixpkgs 以可复现的方式构建软件，并保留了长达约 13 年的历史版本，总计超过 310,083 个软件包版本，这些构建产物通常存放在 cache.nixos.org 等二进制缓存中。trynix 把 QEMU 编译为 WebAssembly（即 qemu-wasm），在浏览器里启动一台 x86\_64 Linux 虚拟机，再将指定版本的闭包从缓存拉入虚拟机，从而给出一个带该软件包的 shell；它只是一个串行控制台，因此无法运行图形界面程序。其底层还依赖 emscripten、wasm TCG JIT、virtio-9p 端口以及 tomberek 的 fastpkgs 伪派生技巧来加速版本解析，终端界面则由编译为 WebAssembly 的 libghostty-vt 提供。

**「影响」** 对 Nix 开发者与代码审查者而言，这意味着可直接在浏览器中启动任意 nixpkgs 曾发布过的包，并借助 trynix-preview 这类 GitHub Action 在 PR 上自动贴出链接来启动该 PR 的构建，无需自备服务器。不过该工具仍属早期，其在大规模项目与日常审查流程中的实际效果尚待验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/fzakaria/trynix">fzakaria/ trynix : Boot anything nixpkgs ever shipped, in your browser .</a></li>
<li><a href="https://trynix.dev/">trynix</a></li>
<li><a href="https://fzakaria.com/2026/09/04/any-nix-package-live-in-your-browser">Any Nix package , live in your browser | Farid Zakaria ’s Blog</a></li>
<li><a href="https://fzakaria.com/2026/09/09/review-a-pull-request-by-booting-it">Review a pull request by booting it | Farid Zakaria’s Blog</a></li>
<li><a href="https://simonwillison.net/2026/Sep/10/trynix/">Any Nix package, live in your browser</a></li>
<li><a href="https://github.com/fzakaria/trynix">GitHub - fzakaria/trynix: Boot anything nixpkgs ever shipped, in your browser. · GitHub</a></li>

</ul>
</details>

**标签**: `#Nix`, `#WebAssembly`, `#QEMU`, `#reproducible builds`, `#browser VMs`

---

<a id="item-tech-news-5"></a>
### [Calif Research 声称演示经微信通话传播的零点击蠕虫](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 8.0/10

Calif Research 宣布发布 WeWorm 的演示，声称这是首个通过微信通话在 iOS 与 Android 上传播的零点击蠕虫。据其说法，受害者既不需要接听电话，也不需要与手机进行任何交互；即使接听，也听不到任何声音，而利用仍然成功。该团队表示，他们借助 AI 在大约两天内找到漏洞并写出首个远程代码执行（RCE）利用，随后又用约一周时间构建出蠕虫，并称这种规模的蠕虫过去需要更大团队耗时数月，如今 AI 已能完成大部分工作，人类团队只负责选择目标和安全测试。需要说明的是，目前这只是 Simon Willison 引用的简短公告与演示，没有独立验证或技术细节，相关说法与影响仍待核实。

rss · Simon Willison · 9月10日 00:56

**「背景」** 零点击蠕虫指无需受害者进行任何操作、甚至无需接听来电即可自动入侵并接管账号、再继续向联系人传播的恶意程序；微信语音通话依赖 VoIP 协议栈，一旦其中存在内存破坏类漏洞，攻击者就可能趁用户毫无察觉时执行代码。据网络安全媒体 CyberSecurityNews 与 CyberInsider 报道，Calif Research 称该概念验证攻击利用微信 VoIP 栈中的内存破坏漏洞，可在数秒内接管目标的微信账号，并称已于 7 月将漏洞报告给腾讯，腾讯随后为用户做了缓解。与此相关的另一层背景是，AI 辅助的漏洞挖掘与利用代码编写正在压缩此类攻击的开发成本，这正是该事件被视为警示信号的原因。

**「影响」** 若该演示所述成立，iOS 与 Android 上的微信用户无需接听来电或进行任何操作便可能受影响——有报道称风险涉及约十亿级账号，同时也有报道称该漏洞已被修复，实际暴露程度应以微信官方补丁状态为准。对防守方而言，AI 辅助下约两天写出首个 RCE 利用、再花约一周组装成蠕虫，意味着同类移动端零点击漏洞的发现与武器化门槛和时间成本被明显压低。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/weworm-first-0-click-worm/">WeWorm - First 0-Click Worm Spreading Through WeChat Calls Across iOS ...</a></li>
<li><a href="https://cyberinsider.com/zero-click-worm-spreads-on-iphones-and-android-via-wechat-calls/">Zero-click worm spreads on iPhones and Android via WeChat calls</a></li>
<li><a href="https://www.theregister.com/security/2026/09/09/wechat-worm-could-pwn-a-friend-before-they-even-answered-the-call/5295234">WeChat worm could pwn a friend before they even answered the call</a></li>
<li><a href="https://www.techtimes.com/articles/327153/20260910/wechat-zero-click-worm-built-ai-days-voip-bug-put-billion-accounts-risk.htm">WeChat Zero - Click Worm Built by AI in Days: VoIP Bug Put Billion...</a></li>
<li><a href="https://fourweekmba.com/ai-wechat-zero-click-worm-ai-cost-curve/">WeChat &#x27;s Patched Zero - Click Worm and the... - FourWeekMBA</a></li>

</ul>
</details>

**标签**: `#ai-security`, `#mobile-security`, `#zero-click-worm`, `#exploit-development`, `#wechat`

---

<a id="item-tech-news-6"></a>
### [Shopify 将移动应用从 React Native 迁回 Swift 和 Kotlin](https://shopify.engineering/back-to-native) ⭐️ 7.0/10

Shopify Engineering 发布文章，说明其移动应用将从 React Native 迁回 Swift 和 Kotlin 原生代码库，回归分别维护 iOS 与 Android 的原生技术栈。这一决定引发 Hacker News 上约 746 分、近 499 条评论的讨论，焦点是原生重写是否已变得更可行。评论中有人表示，跨 JS、C++ 和原生线程调试崩溃的成本高于维护两个代码库；也有开发者分享把约 15–20 个屏幕的应用迁移到 Android/iOS，称借助 Codex 和 Maestro 一夜完成约 90%，随后再花几天打磨细节。不过另一位参与过中型 React Native 应用迁移到 Swift/Kotlin 的评论者认为，“LLM 让原本过于昂贵的迁移变得可行”的说法不正确，因为其大部分工作发生在 2026 年 1 月之前且未使用 LLM 代码辅助。

hackernews · fnthawar2 · 9月10日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=49643982)

**「背景」** React Native 是 Meta 推出的跨平台移动开发框架，用一套 JavaScript 代码同时支撑 iOS 和 Android 应用；Shopify 曾在 2020 年宣布把 React Native 作为其移动端的方向，理由是避免同一功能重复开发、让开发者跨栈协作并控制投入。据后续报道，该团队在 2025 年 1 月还发布过《Five years of React Native at Shopify》，称框架前景良好并将继续投入，而同一团队又在 2026 年 9 月 10 日发文宣布改为分别维护 Swift 与 Kotlin 原生代码库。这次转向被描述为与编码智能体（coding agents）降低了“把应用写两遍”的成本有关，这也是外界讨论“原生重写是否重新变得划算”的直接背景。

**「影响」** 对正在 React Native 与原生之间做取舍的移动团队，这提供了一个大型电商公司的第一方迁移样本，强化需权衡跨栈调试与双代码库维护成本的信号，但单家公司决策不足以证明整个行业已转向原生。

**「社区讨论」** 社区整体对迁回原生表现出支持或共鸣，一位 iOS 工程师称这验证了自己长期反对单纯追求共享代码库的经历；主要分歧在于 LLM 是否让迁移在经济上可行，有实际迁移者以 2026 年 1 月前未用 LLM 的案例提出反例。另有评论批评文章用“Native is now the future of mobile at Shopify”来告别名称含 Native 的产品，认为标题别扭。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://shopify.engineering/back-to-native">Native is now the future of mobile at Shopify (2026) - Shopify</a></li>
<li><a href="https://dev.to/jamilxt/shopify-is-moving-its-mobile-apps-back-to-native-coding-agents-made-it-cheaper-to-build-twice-than-4bf9">Shopify Is Moving Its Mobile Apps Back to Native. Coding ...</a></li>
<li><a href="https://iipoman.com/blog/why-shopify-left-react-native-for-native-mobile-apps">Why Shopify Left React Native for Native Mobile Apps</a></li>

</ul>
</details>

**标签**: `#react-native`, `#mobile-development`, `#swift`, `#kotlin`, `#cross-platform`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [非强制信息干预减少处方 DDI 错误](https://arxiv.org/abs/2609.09673) ⭐️ 7.0/10

rss · arXiv q-fin \(Quantitative Finance\) · 9月10日 04:00

**「背景」** 药物-药物相互作用（DDI）错误威胁患者安全，但现有决策支持系统常要求医生对警报作出响应，打断工作流并造成高忽略率。作者试图检验：不强制响应的信息干预能否减少 DDI 错误，并促使医生学习。

**「方案」** 作者利用印度最大电子病历平台开展随机现场实验，以双重差分设计分析 1700 名医生的 281 万条处方。干预组医生实时收到突出 DDI 错误的信息，但无需回应；对照组不接受此类信息。结果显示，干预使 DDI 错误减少 8.6%，作者估算对应每年 480 万美元住院费用节省和约 134 名可能获救患者。机制上，作者区分反应性纠错与前瞻性学习：前者指错误被标记后医生将其移除，后者指医生在警报发生前就避免错误；早期下降主要来自纠错，随着时间推移医生越来越主动避免错误，也更少重复此前被标记的错误并减少新错误，说明学习可超越具体药物对。效果在不同医生类型间一致，且未损害生产率或护理质量。

**「启示」** 论文结论认为，非强制信息干预可通过即时纠错和持续、可泛化的学习提升患者安全。需要说明，现有材料仅为摘要，缺少方法细节与局限讨论，因此上述因果与成本收益判断仍应视为作者基于该实验的结论。

**标签**: `#clinical decision support`, `#drug-drug interactions`, `#randomized field experiment`, `#healthcare operations`, `#physician learning`

---

<a id="item-tech-blog-2"></a>
### [从公开数据重建大规模企业间生产网络](https://arxiv.org/abs/2512.02362) ⭐️ 7.0/10

rss · arXiv q-fin \(Quantitative Finance\) · 9月10日 04:00

**「背景」** 企业间的生产网络对冲击的总体传导至关重要，却极少被完整观测到，这一数据缺口是评估系统性风险时的核心约束。作者试图仅用公开数据重建国家级、带权的企业间网络。

**「方案」** 作者的方法以两个公开对象为输入：部门投入产出表，以及各部门的企业规模分布。算法先用一个部门感知的引力模型抽取二元的买卖主干，再通过最小能量规划（minimum-energy program）为连边赋权；马尔可夫闭合使重建网络成为本原网络，从而拥有唯一的平稳分布。赋权目标让一步企业平衡与部门流量尽量贴近数据，事后再检验平稳货币向量，其在总量上依然接近。作者为美国重建了约 650 万家企业、3.4 亿条连边的网络，在单台工作站上耗时约四小时，并同样重建了日本、英国、澳大利亚、芬兰和丹麦的网络。日本的重建完全未使用连边数据，却复现了该国观测生产网络中记录的厚尾度分布；重建网络还呈现出比供应商侧更厚的客户尾部，尽管算法对两侧是对称处理的。在重建网络上运行的计算实验显示，企业规模、度数或部门位置都不能良好代理某家企业倒闭所产生的总损失。作者发布了重建代码、生成的网络与 Python 库。

**「启示」** 作者的核心论点是：对于失败损失的总体传导这类问题，完整的加权买卖网络没有好的替代品，常用的企业级代理指标会系统性地误导判断。

**标签**: `#production networks`, `#network reconstruction`, `#input-output models`, `#systemic risk`, `#gravity models`

---

<a id="item-tech-blog-3"></a>
### [The Log S-fBM model: Statistical analysis](https://arxiv.org/abs/2609.09405) ⭐️ 6.0/10

An arXiv abstract presenting statistical analysis and testing tools for the Log S-fBM stochastic volatility model, valuable mainly to specialists in rough and multifractal volatility.

rss · arXiv q-fin \(Quantitative Finance\) · 9月10日 04:00

**标签**: `#stochastic volatility`, `#rough volatility`, `#multifractal processes`, `#fractional Brownian motion`, `#statistical inference`

---

<a id="item-tech-blog-4"></a>
### [Do wind and solar curtail at negative electricity prices? Incentives and evidence across two decades of German renewable support schemes](https://arxiv.org/abs/2609.10053) ⭐️ 6.0/10

A concise abstract of a study on whether German wind and solar generators curtail at negative prices, finding that incentives and actual behavior diverge by technology and support scheme.

rss · arXiv q-fin \(Quantitative Finance\) · 9月10日 04:00

**标签**: `#renewable curtailment`, `#negative electricity prices`, `#feed-in tariffs`, `#German energy policy`, `#power market incentives`

---

<a id="item-tech-blog-5"></a>
### [Signal Correlation, IC, and PnL Dependence](https://arxiv.org/abs/2609.09588) ⭐️ 6.0/10

An arXiv abstract presenting an exact decomposition and non-identifiability theorem showing that signal correlation and PnL correlation need not bound or order each other.

rss · arXiv q-fin \(Quantitative Finance\) · 9月10日 04:00

**标签**: `#quantitative-finance`, `#signal-correlation`, `#information-coefficient`, `#pnl-dependence`, `#portfolio-construction`

---

<a id="item-tech-blog-6"></a>
### [Arbitrage on Decentralized Exchanges](https://arxiv.org/abs/2507.08302) ⭐️ 6.0/10

An arXiv abstract presenting a game-theoretic model of gas-fee competition among DEX-CEX arbitrageurs under different transaction reversion settings, with claimed empirical validation using Binance and Uniswap V2 data.

rss · arXiv q-fin.TR \(Trading &amp; Microstructure\) · 9月10日 04:00

**标签**: `#decentralized exchanges`, `#automated market makers`, `#arbitrage`, `#gas fees`, `#market microstructure`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [Kalshi 获 CFTC 批准，上线黄金和白银永续期货](https://www.cnbc.com/2026/09/10/kalshi-launches-perps-for-gold-and-silver-following-cftc-approval-expanding-futures-offerings.html) ⭐️ 8.0/10

Kalshi 已获得美国商品期货交易委员会（CFTC）批准，于周四上线挂钩黄金和白银的永续期货合约，这是该公司首个获批的非加密类永续合约产品。据 Kalshi 网站数据，其加密永续合约自 5 月底获批上线以来已累计成交 440 亿美元名义金额。

rss · CNBC Finance · 9月10日 14:00

**「背景」** 永续期货是没有到期日、通过资金费率机制跟踪标的资产价格的合约，投资者无需持有标的资产即可获得价格敞口。Kalshi 今年 5 月底已获准上线与加密货币挂钩的永续合约，而此次是 CFTC 首次批准与加密货币无关（即挂钩黄金、白银）的永续合约。

**「影响」** 若此类受监管永续合约被市场接受，CME、CBOE 等传统期货交易所将直接面临竞争压力——在早前美国首批永续合约获批后，这些交易所的股价曾因担忧新合约冲击其现有期货业务而下跌。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/commodities/articles/kalshi-launches-gold-silver-perpetual-175449558.html">Kalshi launches gold and silver perpetual futures with CFTC approval</a></li>
<li><a href="https://www.binance.com/en/square/post/09-10-2026-kalshi-wins-cftc-approval-for-gold-and-silver-perpetual-contracts-365192942307804">Kalshi Wins CFTC Approval for Gold and Silver Perpetual Contracts</a></li>
<li><a href="https://www.cnbc.com/2026/08/18/kalshi-wants-to-launch-perps-tied-to-equity-indexes.html">Kalshi seeks to launch ‘perps’ on equity indexes as it moves in on traditional exchanges&#x27; turf</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/cboe-cme-ice-ndaq-stocks-183845986.html">CBOE, CME, ICE, NDAQ Stocks Take A Hit After Kalshi&#x27;s Bitcoin Perps Approval – TD Cowen Sees Real Risk, But RBC Says It&#x27;s ‘Manageable’</a></li>

</ul>
</details>

**标签**: `#Kalshi`, `#perpetual futures`, `#CFTC approval`, `#gold and silver`, `#derivatives market structure`

---

<a id="item-finance-news-2"></a>
### [纳斯达克向 Kraken 母公司 Payward 投资 1 亿美元，估值 210 亿美元](https://www.coindesk.com/business/2026/09/10/nasdaq-invests-usd100-million-in-kraken-parent-company-payward-at-usd21-billion-valuation) ⭐️ 8.0/10

纳斯达克（Nasdaq）向加密货币交易所 Kraken 的母公司 Payward 投资 1 亿美元，此次投资对 Payward 的估值为 210 亿美元。

rss · CoinDesk · 9月10日 11:21

**「背景」** Kraken（法定名称为 Payward）成立于 2011 年，是一家美国加密货币交易所，近年也向非美国客户提供代币化股票的代币化证券交易服务。据雅虎财经报道，纳斯达克这笔 1 亿美元投资属于一轮新融资，Payward 此前寻求的估值为 200 亿美元，最终以 210 亿美元（美国）估值完成。

**「影响」** 两家公司还宣布合作，计划在 2027 年第二季度推出名为 NET 的“股权代币”框架，若如期落地，股票等传统资产将可能以代币形式在相关平台上交易，从而影响希望以加密方式买卖股票的投资者与券商；目前这仍是计划，而非已实现的产品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/crypto/articles/nasdaq-invests-100-million-kraken-135200836.html?fr=sycsrp_catchall">Nasdaq Invests $100 Million In Kraken Parent Company</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kraken_%28cryptocurrency_exchange%29">Kraken (cryptocurrency exchange) - Wikipedia</a></li>
<li><a href="https://cointelegraph.com/news/nasdaq-invests-100m-kraken-parent-21b-valuation">Nasdaq Invests $100M in Kraken Parent at $21B Valuation: Report</a></li>
<li><a href="https://www.thestreet.com/crypto/markets/nasdaq-invests-100m-in-fintech-giant-at-21b-valuation">Nasdaq invests $100 million in Kraken parent.</a></li>

</ul>
</details>

**标签**: `#crypto exchange`, `#venture investment`, `#Nasdaq`, `#Kraken`, `#valuation`

---

<a id="item-finance-news-3"></a>
### [美国监管机构放宽社区银行监管负担，扩大 18 个月检查周期适用范围](https://www.federalreserve.gov/newsevents/pressreleases/bcreg20260910a.htm) ⭐️ 7.0/10

美国联邦银行监管机构宣布放宽社区银行的监管负担，扩大符合 18 个月一次现场检查周期资格的银行范围；公告未说明具体门槛、适用范围或生效时间。

rss · Federal Reserve Press Releases · 9月10日 20:00

**「背景」** 美国银行监管机构通常每 12 个月对银行进行一次现场检查，符合条件的机构可延长至 18 个月。此次调整依据《21 世纪住房之路法案》（21st Century ROAD to Housing Act），把享受 18 个月检查周期的资产门槛从 30 亿美元提高到 60 亿美元，美联储、联邦存款保险公司和货币监理署据此联合发布了这项临时最终规则。

**「影响」** 被纳入 18 个月检查周期的社区银行，接受监管现场检查的频率将从每 12 个月一次降至大约每 18 个月一次，从而减少配合检查所耗费的人力和合规成本。不过该公告未披露适用机构的资产门槛与生效时间，具体覆盖范围仍不明确。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.federalreserve.gov/newsevents/pressreleases/bcreg20260910a.htm">Federal Reserve Board - Agencies reduce regulatory burden for ...</a></li>
<li><a href="https://www.occ.gov/news-issuances/bulletins/2026/bulletin-2026-45.html">Expanded Examination Cycle Eligibility: Interim Final Rule</a></li>
<li><a href="https://www.crowdfundinsider.com/2026/09/308981-agencies-reduce-regulatory-burden-for-community-banks-increase-eligibility-for-18-month-exam-cycle/">Agencies Reduce Regulatory Burden For Community Banks ...</a></li>

</ul>
</details>

**标签**: `#banking regulation`, `#community banks`, `#Federal Reserve`, `#regulatory relief`, `#supervisory exams`

---

<a id="item-finance-news-4"></a>
### [Liquid Network resumes block production after $320M exploit](https://cointelegraph.com/news/liquid-network-resumes-block-production-after-320m-exploit?utm_source=rss_feed&amp;utm_medium=rss&amp;utm_campaign=rss_partner_inbound) ⭐️ 7.0/10

Liquid Network resumed block production after a reported $320M exploit, while transactions and peg operations remain suspended.

rss · Cointelegraph · 9月10日 16:38

**标签**: `#Liquid Network`, `#crypto exploit`, `#Bitcoin sidechain`, `#blockchain security`, `#peg operations`

---

<a id="item-finance-news-5"></a>
### [The iPhone Duo enters China’s crowded foldable market — and faces a price test](https://www.cnbc.com/2026/09/11/the-iphone-duo-enters-chinas-crowded-foldable-market.html) ⭐️ 6.0/10

Apple&\#x27;s new folding iPhone Duo is entering China&\#x27;s established foldable market at a premium price against entrenched Huawei, Xiaomi and other domestic rivals, drawing a cautious early consumer response.

rss · CNBC Finance · 9月11日 00:19

**标签**: `#Apple`, `#foldable smartphones`, `#China market`, `#competition`, `#consumer pricing`

---

<a id="item-finance-news-6"></a>
### [OpenAI targets work of Wall Street junior bankers with new ChatGPT for Financial Services](https://www.cnbc.com/2026/09/10/openai-chatgpt-for-financial-services-targets-work-of-junior-bankers.html) ⭐️ 6.0/10

OpenAI announced ChatGPT for Financial Services, an enterprise product built with Morgan Stanley and Evercore to automate investment-banking research and presentation tasks.

rss · CNBC Finance · 9月10日 19:02

**标签**: `#OpenAI`, `#ChatGPT`, `#financial services`, `#investment banking`, `#enterprise AI`

---

<a id="item-finance-news-7"></a>
### [Stocks making the biggest moves premarket: Macy&\#x27;s, Meta, Apple, Novartis and more](https://www.cnbc.com/2026/09/10/stocks-making-the-biggest-moves-premarket-.html) ⭐️ 6.0/10

A CNBC premarket roundup covering company-specific stock moves driven by earnings, guidance, analyst actions, an acquisition, and declining copper prices.

rss · CNBC Finance · 9月10日 11:54

**标签**: `#premarket-movers`, `#earnings`, `#guidance`, `#mergers-acquisitions`, `#market-reaction`

---

<a id="item-finance-news-8"></a>
### [BIS chief warns AI capex arms race relies on opaque debt, posing systemic risks](https://www.coindesk.com/business/2026/09/10/ai-s-rapid-rise-poses-global-financial-stability-risks-says-head-of-the-bis) ⭐️ 6.0/10

The BIS chief warns that an AI capital-expenditure arms race funded through opaque debt could pose systemic risks to financial stability.

rss · CoinDesk · 9月10日 12:00

**标签**: `#AI capex`, `#systemic risk`, `#debt`, `#financial stability`, `#BIS`

---