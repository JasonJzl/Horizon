---
layout: default
title: "Horizon Summary: 2026-09-11 (EN)"
date: 2026-09-11
lang: en
---

> From 110 items, 20 important content pieces were selected

---

**Technology News**
1. [Forgejo 16.0.4 fixes critical remote code execution in versions through 16.0.3](#item-tech-news-1) ⭐️ 8.0/10
2. [Microsoft Elevates Rust to Tier-1 Language Status](#item-tech-news-2) ⭐️ 8.0/10
3. [OpenAI Navier-Stokes Release Included Lean 4 Formal Proof](#item-tech-news-3) ⭐️ 8.0/10
4. [TryNix boots any Nix package in a browser via QEMU-WASM](#item-tech-news-4) ⭐️ 8.0/10
5. [Calif Research demos WeWorm zero-click WeChat worm](#item-tech-news-5) ⭐️ 8.0/10
6. [Shopify moves mobile app from React Native to Swift and Kotlin](#item-tech-news-6) ⭐️ 7.0/10

**Technology Blog**
1. [Non-Mandatory DDI Information Reduces Prescription Errors](#item-tech-blog-1) ⭐️ 7.0/10
2. [Reconstructing Large-Scale Firm-to-Firm Production Networks](#item-tech-blog-2) ⭐️ 7.0/10
3. [The Log S-fBM model: Statistical analysis](#item-tech-blog-3) ⭐️ 6.0/10
4. [Do wind and solar curtail at negative electricity prices? Incentives and evidence across two decades of German renewable support schemes](#item-tech-blog-4) ⭐️ 6.0/10
5. [Signal Correlation, IC, and PnL Dependence](#item-tech-blog-5) ⭐️ 6.0/10
6. [Arbitrage on Decentralized Exchanges](#item-tech-blog-6) ⭐️ 6.0/10

**Financial News**
1. [Kalshi launches CFTC-approved gold and silver perpetual futures](#item-finance-news-1) ⭐️ 8.0/10
2. [Nasdaq invests $100 million in Kraken parent Payward at $21 billion valuation](#item-finance-news-2) ⭐️ 8.0/10
3. [Federal banking agencies expand 18-month exam cycle eligibility for community banks](#item-finance-news-3) ⭐️ 7.0/10
4. [Liquid Network resumes block production after $320M exploit](#item-finance-news-4) ⭐️ 7.0/10
5. [The iPhone Duo enters China’s crowded foldable market — and faces a price test](#item-finance-news-5) ⭐️ 6.0/10
6. [OpenAI targets work of Wall Street junior bankers with new ChatGPT for Financial Services](#item-finance-news-6) ⭐️ 6.0/10
7. [Stocks making the biggest moves premarket: Macy&\#x27;s, Meta, Apple, Novartis and more](#item-finance-news-7) ⭐️ 6.0/10
8. [BIS chief warns AI capex arms race relies on opaque debt, posing systemic risks](#item-finance-news-8) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Forgejo 16.0.4 fixes critical remote code execution in versions through 16.0.3](https://codeberg.org/forgejo/forgejo/src/branch/forgejo/release-notes-published/16.0.4.md) ⭐️ 8.0/10

Forgejo 16.0.4 fixes a critical remote code execution vulnerability affecting Forgejo versions up to 16.0.3, according to the release notes linked by the submission. The critical change prevents template expansion from interfering with git repository initialization when a new repository is generated from a template repository. In that flow, Forgejo clones the template repository, removes the \`.git\` folder, performs variable template expansion on files listed in \`.forgejo/template\`, and initializes a new git repository. Community members noted the release notes were temporarily unreadable because of Codeberg rate limits and shared underlying pull request and milestone links, while the supplied discussion does not provide full exploit details. A Gitea project leader said Gitea is protected against both issues, underscoring that affected Forgejo operators should patch promptly.

hackernews · weierstass · Sep 10, 15:57 · [Discussion](https://news.ycombinator.com/item?id=49645907)

**「Background」** Forgejo is a self-hosted Git forge, a web application for hosting and managing Git repositories. The critical issue affects template repositories: when a user generates a new repository from a template, Forgejo clones the template, deletes its \`.git\` directory, performs variable expansion on files listed in \`.forgejo/template\`, and initializes a fresh Git repository, a process that a crafted template can subvert. Public vulnerability records identify the resulting remote code execution as CVE-2026-89094 and a related symlink attack as CVE-2025-68937, both addressed in Forgejo 16.0.4.

**「Impact」** Administrators of self-hosted Forgejo instances running version 16.0.3 or earlier must upgrade to the fixed 16.0.4 release — or 15.0.8 on the older maintained branch — because the vulnerability lets attackers write to unintended files and potentially gain shell access on the forge host. Vulnerability databases track the issue as CVE-2025-68937.

**「Community discussion」** Commenters focused on access to the release notes, which were unreadable due to Codeberg rate limits, and on the underlying critical fix for template expansion during repository initialization. A Gitea project leader stated that Gitea is protected against both issues, and another commenter argued that Forgejo&\#x27;s restrictions on LLM contributions leave it at a disadvantage because attackers can still use AI to search for vulnerabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2025-68937/">CVE-2025-68937: Forgejo RCE Vulnerability - SentinelOne</a></li>
<li><a href="https://www.rapid7.com/db/vulnerabilities/cve-2026-89094/">CVE-2026-89094: Forgejo: Forgejo before 16.0.4 allows remote ...</a></li>
<li><a href="https://newzino.com/story/forgejo-16-0-3-critical-rce-fa98b4">Forgejo patches critical RCE affecting versions through 16.0.3</a></li>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2025-68937/">CVE-2025-68937: Forgejo RCE Vulnerability</a></li>
<li><a href="https://noise.getoto.net/2026/09/10/forgejo-16-0-4-and-15-0-8-address-critical-security-vulnerability/">Forgejo 16.0.4 and 15.0.8 address critical security vulnerability | Noise</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#Forgejo`, `#open-source`, `#RCE`

---

<a id="item-tech-news-2"></a>
### [Microsoft Elevates Rust to Tier-1 Language Status](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 8.0/10

Microsoft has elevated Rust to tier-1 language status, according to a guest post published by the Rust Foundation. The designation is a notable adoption milestone for Rust and for the broader open source systems-programming ecosystem. The available item does not include the original source content, so it does not specify the exact support scope, versions, timelines, or engineering commitments behind the tier-1 label. Community discussion treats the move as evidence that Rust has matured into a serious competitor to established languages such as C++ and C\#.

hackernews · mmastrac · Sep 10, 13:39 · [Discussion](https://news.ycombinator.com/item?id=49643546)

**「Background」** Microsoft&\#x27;s tier-1 designation signals that a language receives first-class support in its platform and tooling strategy; Rust now sits at that level alongside C++ and C\#, although C++ still dominates after decades of development. Production software at Microsoft moves through extensive security and quality workflows, which shapes how new languages are adopted for native platform work. The announcement has also focused attention on practical tooling questions, such as when Rust will receive tier-1 debugging support in Visual Studio.

**「Impact」** For developers and organizations targeting Microsoft&\#x27;s platforms, the tier-1 designation signals that Rust is being treated as a first-class option for systems and greenfield work, though the available item does not specify concrete tooling, support guarantees, or timelines.

**「Community Discussion」** Commenters broadly welcomed the news as confirmation that Rust has matured into a serious competitor to C++ and C\#, with one professional Rust developer saying they see no technical reason to choose another language for high-level application work and another citing Microsoft&\#x27;s memory-safety CVE record as strategic motivation. They also pointed to related efforts such as a reported Microsoft goal to convert 1 billion lines of code to Rust by 2030 through automated tooling, DARPA-funded C-to-Rust conversion work, and rumors of MSVC integration, while noting that newer alternatives like Zig and Odin still have more rough edges.

<details><summary>References</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier - 1 Language at Microsoft</a></li>
<li><a href="https://news.ycombinator.com/item?id=49643546">Rust Is Tier - 1 Language at Microsoft | Hacker News</a></li>
<li><a href="https://www.drweb.de/microsoft-rust-tier-1-sprache/">Warum macht Microsoft Rust zur Tier - 1 -Sprache? | Dr. Web</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#Microsoft`, `#programming languages`, `#systems programming`, `#open source`

---

<a id="item-tech-news-3"></a>
### [OpenAI Navier-Stokes Release Included Lean 4 Formal Proof](https://www.johndcook.com/blog/2026/09/09/formal-method-revolution/) ⭐️ 8.0/10

OpenAI’s Navier-Stokes-related release shipped with a Lean 4 formal proof, according to a commentary post and Hacker News discussion about the announcement. The item treats this as a potentially major AI-for-mathematics development because the proof is machine-checkable, while cautioning that the supplied material is a blog commentary rather than the primary paper or artifact. Commenters focused less on the mathematical result itself than on verification cost, proof automation, and the significance of AI-generated mathematics. They cited Lean verification demands—including a claimed 15-hour, 230 GB Fermat’s Last Theorem verification versus 11 days to generate the Lean code—and debated whether such comparisons to human proof effort are meaningful.

hackernews · ibobev · Sep 10, 21:22 · [Discussion](https://news.ycombinator.com/item?id=49650326)

**「Background」** The Navier–Stokes equations describe fluid motion and are central to one of the Clay Mathematics Institute&\#x27;s Millennium Prize Problems, which concerns whether smooth solutions always exist in three dimensions or can break down. OpenAI&\#x27;s release reportedly claimed to settle a long-standing Navier–Stokes question and included a formal proof in Lean 4, a proof assistant used to mechanically check mathematical arguments. The claimed result has been described as a 166-page manuscript with a public Lean project and is awaiting independent assessment, which is why commentary has focused on verification cost, proof automation, and the significance of AI-generated mathematics.

**「Impact」** For mathematicians and formal-verification tooling developers, the reported pairing of an AI-generated Navier–Stokes solution with a Lean-verified proof points to machine-checkable verification—one source puts the Lean step at 17 hours—becoming the practical trust anchor and cost bottleneck for AI-produced mathematics. Because the supplied material is a commentary post and discussion thread rather than the primary paper or artifact, the specifics of the underlying proof and verification figures remain second-hand and unconfirmed here.

**「Community Discussion」** Commenters debated the economics and limits of formal verification: one compared an estimated $40 million agent cost with roughly $132 million for 880,000 human hours at $150 per hour, while others challenged the “forty hours per page” heuristic as outdated and cited Lean’s slowness and resource use as a practical obstacle. Concerns also included whether AI can handle more direct or inductive proofs and what happens if a solution is too difficult for humans to verify independently.

<details><summary>References</summary>
<ul>
<li><a href="https://www.johndcook.com/blog/2026/09/09/formal-method-revolution/">The part of Navier - Stokes no one is talking about</a></li>
<li><a href="https://emergent.sh/news/openai-claims-navier-stokes-millennium-prize">OpenAI Claims Navier - Stokes Millennium Prize Solution</a></li>
<li><a href="https://kingy.ai/blog/navier-stokes-ai-proof-claims-dispute/">OpenAI ’s Navier – Stokes Proof Claim: Evidence and Dispute</a></li>
<li><a href="https://emergent.sh/news/openai-claims-navier-stokes-millennium-prize">OpenAI Claims Navier - Stokes Millennium Prize Solution</a></li>
<li><a href="https://www.johndcook.com/blog/2026/09/09/formal-method-revolution/">The part of Navier - Stokes no one is talking about</a></li>
<li><a href="https://www.1950.ai/post/openai-s-navier-stokes-breakthrough-what-a-90-year-old-mathematics-problem-reveals-about-ai">OpenAI’s Navier - Stokes Breakthrough: What a 90-Year-Old...</a></li>

</ul>
</details>

**Tags**: `#Lean 4`, `#formal verification`, `#AI for mathematics`, `#theorem proving`, `#Navier-Stokes`

---

<a id="item-tech-news-4"></a>
### [TryNix boots any Nix package in a browser via QEMU-WASM](https://simonwillison.net/2026/Sep/10/trynix/) ⭐️ 8.0/10

Farid Zakaria&\#x27;s trynix.dev provides a qemu-wasm-powered x86\_64 Linux virtual machine that runs entirely in the browser through WebAssembly. The VM can boot any Nix package from the past 13 years, and those environments are URL-addressable; for example, https://trynix.dev/?pkg=python3%403.6.2 lets a user click &quot;Load&quot; to get an interactive shell against a VM running Python 3.6.2 from 2017. Zakaria is building additional tools on top of the service, including trynix-preview, a GitHub Action that comments a link on a pull request so the PR&\#x27;s build can be booted in the browser via trynix.dev. The project makes historical Nix environments interactively shareable and URL-addressable without servers, with the browser acting as the runtime.

rss · Simon Willison · Sep 10, 23:44

**「Background」** Nix is a package manager and build system whose nixpkgs repository keeps every historical revision addressable, and trynix draws on that record by browsing over 310,083 package versions spanning 13 years of nixpkgs history. The tool works because ktock&\#x27;s qemu-wasm compiles QEMU to Emscripten/WebAssembly, including the wasm TCG JIT and a virtio-9p port that lets the host fetch a package closure from cache.nixos.org and expose it inside an emulated x86\_64 Linux guest. Building on tomberek&\#x27;s fastpkgs fake-derivation approach for a fast resolution path and ghostty-web for terminal emulation, trynix turns each package version into a reproducible, URL-addressable shell session that requires no server.

**「Impact」** Nix package consumers and maintainers can now run any of the past 13 years&\#x27; packages, and a pull request&\#x27;s build, directly in a browser without installing Nix or provisioning a server, since the trynix-preview GitHub Action comments a bootable link on each PR. This makes historical reproduction and review interactive and URL-shareable, though the source presents it as a pointer rather than a benchmarked production guarantee.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/fzakaria/trynix">fzakaria/ trynix : Boot anything nixpkgs ever shipped, in your browser .</a></li>
<li><a href="https://trynix.dev/">trynix</a></li>
<li><a href="https://fzakaria.com/2026/09/04/any-nix-package-live-in-your-browser">Any Nix package , live in your browser | Farid Zakaria ’s Blog</a></li>
<li><a href="https://fzakaria.com/2026/09/09/review-a-pull-request-by-booting-it">Review a pull request by booting it | Farid Zakaria’s Blog</a></li>
<li><a href="https://github.com/fzakaria/trynix">GitHub - fzakaria/trynix: Boot anything nixpkgs ever shipped, in your browser. · GitHub</a></li>

</ul>
</details>

**Tags**: `#Nix`, `#WebAssembly`, `#QEMU`, `#reproducible builds`, `#browser VMs`

---

<a id="item-tech-news-5"></a>
### [Calif Research demos WeWorm zero-click WeChat worm](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 8.0/10

Calif Research announced the release of a demo of WeWorm, which it describes as the first zero-click worm to spread through WeChat calls across both iOS and Android. According to the announcement, the victim does not need to answer the call or interact with the phone at all; even if they answer, they hear nothing and the exploit still succeeds. The team says that, working with AI, it found the bug and wrote the first remote code execution \(RCE\) exploit in about two days, then spent one more week building the worm, and it argues that a worm at this scale previously would have taken a larger team months, with AI now doing most of the work while the team supplied judgment about what to target and how to test safely. The item as supplied is only a short quoted announcement and demo link, with no independent verification or technical detail, so the claims should be treated with caution. No community comments accompanied the item.

rss · Simon Willison · Sep 10, 00:56

**「Background」** WeChat, Tencent&\#x27;s messaging platform, handles voice calls through a Voice-over-IP \(VoIP\) stack; a &quot;zero-click&quot; attack means the target device is compromised without the user answering or interacting. According to reporting on the research, Calif Research says WeWorm exploits a memory corruption vulnerability in that VoIP stack, that the bug was reported to Tencent in July, and that Tencent has since mitigated the exploit for users. The claimed significance rests less on the worm mechanism itself than on the development process: Calif says AI assistance let its team find the bug and write a first remote code execution \(RCE\) exploit in about two days, with the worm taking roughly one more week, work it says previously required a larger team over months.

**「Impact」** If the demo holds up under independent scrutiny, WeChat users on both iOS and Android could be exposed to a zero-click worm that spreads through incoming calls without the victim answering or touching their phone, a risk affecting a messaging user base reported to number in the billions. The disclosure remains an unverified demo without technical detail or third-party reproduction, and at least one report describes the flaw as patched, so the real-world exposure of current WeChat users is not yet confirmed.

<details><summary>References</summary>
<ul>
<li><a href="https://cybersecuritynews.com/weworm-first-0-click-worm/">WeWorm - First 0-Click Worm Spreading Through WeChat Calls Across iOS ...</a></li>
<li><a href="https://cyberinsider.com/zero-click-worm-spreads-on-iphones-and-android-via-wechat-calls/">Zero-click worm spreads on iPhones and Android via WeChat calls</a></li>
<li><a href="https://www.theregister.com/security/2026/09/09/wechat-worm-could-pwn-a-friend-before-they-even-answered-the-call/5295234">WeChat worm could pwn a friend before they even answered the call</a></li>
<li><a href="https://www.techtimes.com/articles/327153/20260910/wechat-zero-click-worm-built-ai-days-voip-bug-put-billion-accounts-risk.htm">WeChat Zero - Click Worm Built by AI in Days: VoIP Bug Put Billion...</a></li>
<li><a href="https://fourweekmba.com/ai-wechat-zero-click-worm-ai-cost-curve/">WeChat &#x27;s Patched Zero - Click Worm and the... - FourWeekMBA</a></li>

</ul>
</details>

**Tags**: `#ai-security`, `#mobile-security`, `#zero-click-worm`, `#exploit-development`, `#wechat`

---

<a id="item-tech-news-6"></a>
### [Shopify moves mobile app from React Native to Swift and Kotlin](https://shopify.engineering/back-to-native) ⭐️ 7.0/10

Shopify Engineering has documented its decision to move the company&\#x27;s mobile app from React Native back to separate native Swift and Kotlin codebases. Shopify says it originally switched from native to React Native in 2020 to stop building the same features twice, let developers work across the stack, and address other reasons that were truncated in the supplied excerpt. The move matters as a first-party data point in the long-running native-versus-cross-platform debate, and it drew an unusually large Hacker News discussion of 746 points and roughly 499 comments. Commenters debated whether LLM code assistance has made native rewrites more economically feasible, with some sharing firsthand migration accounts and others disputing that LLMs were decisive. Specific release dates, performance metrics, and implementation details were not available in the supplied source excerpt.

hackernews · fnthawar2 · Sep 10, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49643982)

**「Background」** React Native is a cross-platform framework that lets developers build iOS and Android apps from a shared JavaScript codebase, while Swift and Kotlin are Apple&\#x27;s and Google&\#x27;s native languages for those platforms respectively. Shopify had adopted React Native in 2020 and as recently as January 2025 published a &quot;Five years of React Native at Shopify&quot; post describing continued investment, making its return to native codebases a reversal of a prominent public commitment. External coverage frames the shift around coding agents reducing the cost of building and maintaining separate native apps.

**「Impact」** For mobile teams evaluating React Native against native Swift and Kotlin, Shopify&\#x27;s move offers a high-profile case study in the trade-offs of a shared codebase versus platform-specific development, though it remains one company&\#x27;s architecture decision rather than proof that native rewrites are universally cheaper.

**「Community discussion」** The thread broadly welcomed Shopify&\#x27;s move, with one iOS engineer calling it validation for long-standing skepticism toward shared codebases and another arguing that debugging crashes across JavaScript, C++, and native threads costs more than maintaining two codebases. A counterpoint came from a developer who said they did most of a similar React Native-to-Swift/Kotlin migration before January 2026 without LLM assistance, disputing the idea that LLMs made the rewrite economically viable, while another described using Codex to migrate a 15–20 screen app to 90% overnight before spending days on polish, and one commenter noted the irony of the &quot;Native is now the future&quot; title given React Native&\#x27;s name.

<details><summary>References</summary>
<ul>
<li><a href="https://shopify.engineering/back-to-native">Native is now the future of mobile at Shopify (2026) - Shopify</a></li>
<li><a href="https://dev.to/jamilxt/shopify-is-moving-its-mobile-apps-back-to-native-coding-agents-made-it-cheaper-to-build-twice-than-4bf9">Shopify Is Moving Its Mobile Apps Back to Native. Coding ...</a></li>
<li><a href="https://iipoman.com/blog/why-shopify-left-react-native-for-native-mobile-apps">Why Shopify Left React Native for Native Mobile Apps</a></li>

</ul>
</details>

**Tags**: `#react-native`, `#mobile-development`, `#swift`, `#kotlin`, `#cross-platform`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Non-Mandatory DDI Information Reduces Prescription Errors](https://arxiv.org/abs/2609.09673) ⭐️ 7.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Sep 10, 04:00

**「Background」** Drug-drug interaction \(DDI\) errors pose serious patient safety risks. Existing decision-support systems often require physicians to respond to alerts, which disrupts workflows and contributes to high override rates.

**「Solution」** The authors report a randomized field experiment on India&\#x27;s largest electronic medical record platform to test whether non-mandatory information can reduce DDI errors and foster learning. Analyzing 2.81 million prescriptions from 1,700 physicians with a difference-in-differences design, treatment physicians received real-time information highlighting DDI errors without being required to respond, while control physicians received no such information. The intervention reduced DDI errors by 8.6%, an effect the authors associate with an estimated US$4.8 million in annual hospitalization cost savings and approximately 134 lives potentially saved. They identify two mechanisms: reactive correction, where physicians remove errors after they are flagged, and proactive learning, where they avoid errors before alerts occur. Early reductions are driven mainly by correction, but physicians increasingly avoid errors over time, become less likely to repeat previously flagged errors, and reduce new errors, suggesting learning generalizes beyond specific drug pairs. Effects were consistent across physician types and did not compromise productivity or care quality, though the abstract provides no implementation detail or limitations.

**「Takeaway」** The authors conclude that non-mandatory information interventions can improve patient safety through both immediate error correction and persistent, generalizable learning.

**Tags**: `#clinical decision support`, `#drug-drug interactions`, `#randomized field experiment`, `#healthcare operations`, `#physician learning`

---

<a id="item-tech-blog-2"></a>
### [Reconstructing Large-Scale Firm-to-Firm Production Networks](https://arxiv.org/abs/2512.02362) ⭐️ 7.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Sep 10, 04:00

**「Background」** Firm-to-firm production networks matter for aggregate propagation, but they are rarely observed. This paper reconstructs national-scale, weighted buyer-seller networks from two public objects: a sectoral input-output table and the distribution of firm sizes by sector.

**「Solution」** The authors first draw a binary buyer-seller backbone from a sector-aware gravity model and then assign weights with a minimum-energy program, using a Markov closure that makes the reconstructed network primitive and gives it a unique stationary distribution. The weighting keeps one-step firm balances and sectoral flows close to the data, and the ex post stationary money vector remains close in aggregate. For the United States, they reconstruct about 6.5 million firms and 340 million links in roughly four hours on a single workstation; they also reconstruct networks for Japan, the United Kingdom, Australia, Finland, and Denmark. Built without any link data, the Japanese reconstruction reproduces the heavy-tailed degree regime documented in the country&\#x27;s observed production network, and the reconstructed networks exhibit customer tails heavier than supplier tails even though the algorithm treats the two sides symmetrically. In computational experiments on individual firm failures, the authors find that neither firm size nor degree nor sectoral position is a good proxy for the aggregate losses generated.

**「Takeaway」** The paper argues that for systemic-risk questions, there is no good substitute for the complete weighted buyer-seller network it reconstructs, since common firm-level proxies can mislead. Its broader significance is a scalable, public-data method for building the missing network itself.

**Tags**: `#production networks`, `#network reconstruction`, `#input-output models`, `#systemic risk`, `#gravity models`

---

<a id="item-tech-blog-3"></a>
### [The Log S-fBM model: Statistical analysis](https://arxiv.org/abs/2609.09405) ⭐️ 6.0/10

An arXiv abstract presenting statistical analysis and testing tools for the Log S-fBM stochastic volatility model, valuable mainly to specialists in rough and multifractal volatility.

rss · arXiv q-fin \(Quantitative Finance\) · Sep 10, 04:00

**Tags**: `#stochastic volatility`, `#rough volatility`, `#multifractal processes`, `#fractional Brownian motion`, `#statistical inference`

---

<a id="item-tech-blog-4"></a>
### [Do wind and solar curtail at negative electricity prices? Incentives and evidence across two decades of German renewable support schemes](https://arxiv.org/abs/2609.10053) ⭐️ 6.0/10

A concise abstract of a study on whether German wind and solar generators curtail at negative prices, finding that incentives and actual behavior diverge by technology and support scheme.

rss · arXiv q-fin \(Quantitative Finance\) · Sep 10, 04:00

**Tags**: `#renewable curtailment`, `#negative electricity prices`, `#feed-in tariffs`, `#German energy policy`, `#power market incentives`

---

<a id="item-tech-blog-5"></a>
### [Signal Correlation, IC, and PnL Dependence](https://arxiv.org/abs/2609.09588) ⭐️ 6.0/10

An arXiv abstract presenting an exact decomposition and non-identifiability theorem showing that signal correlation and PnL correlation need not bound or order each other.

rss · arXiv q-fin \(Quantitative Finance\) · Sep 10, 04:00

**Tags**: `#quantitative-finance`, `#signal-correlation`, `#information-coefficient`, `#pnl-dependence`, `#portfolio-construction`

---

<a id="item-tech-blog-6"></a>
### [Arbitrage on Decentralized Exchanges](https://arxiv.org/abs/2507.08302) ⭐️ 6.0/10

An arXiv abstract presenting a game-theoretic model of gas-fee competition among DEX-CEX arbitrageurs under different transaction reversion settings, with claimed empirical validation using Binance and Uniswap V2 data.

rss · arXiv q-fin.TR \(Trading &amp; Microstructure\) · Sep 10, 04:00

**Tags**: `#decentralized exchanges`, `#automated market makers`, `#arbitrage`, `#gas fees`, `#market microstructure`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Kalshi launches CFTC-approved gold and silver perpetual futures](https://www.cnbc.com/2026/09/10/kalshi-launches-perps-for-gold-and-silver-following-cftc-approval-expanding-futures-offerings.html) ⭐️ 8.0/10

Kalshi began listing perpetual futures tied to gold and silver on Thursday, after the Commodity Futures Trading Commission approved the contracts this week — the first non-crypto perpetual futures approved in the U.S., following the platform&\#x27;s crypto perps launched in late May. Kalshi Klear chief risk officer Udesh Jha attributed the move to demand tied to inflation, and the company said its commodity-related event contracts surpassed $400 million in trading volume over seven months.

rss · CNBC Finance · Sep 10, 14:00

**「Background」** Perpetual futures are futures-style contracts with no expiration date that track an asset&\#x27;s price without requiring the buyer to own it. The CFTC&\#x27;s approval makes these the first non-crypto perpetuals cleared for U.S. trading, after Kalshi — originally a prediction-markets platform — listed crypto-linked perpetuals in late May.

**「Impact」** The CFTC-approved gold and silver perpetuals put Kalshi into direct competition with established futures exchanges such as CME Group and CBOE, whose shares fell after the launch on investor concerns that the contracts could take business from their traditional metals futures; CME has sued the CFTC to block the approval.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/commodities/articles/kalshi-launches-gold-silver-perpetual-175449558.html">Kalshi launches gold and silver perpetual futures with CFTC approval</a></li>
<li><a href="https://cryptobriefing.com/kalshi-launches-gold-and-silver-perps-after-cftc-approval/">Kalshi launches gold and silver perps after CFTC approval</a></li>
<li><a href="https://www.cnbc.com/2026/08/18/kalshi-wants-to-launch-perps-tied-to-equity-indexes.html">Kalshi seeks to launch ‘perps’ on equity indexes as it moves in on traditional exchanges&#x27; turf</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/cboe-cme-ice-ndaq-stocks-183845986.html">CBOE, CME, ICE, NDAQ Stocks Take A Hit After Kalshi&#x27;s Bitcoin Perps Approval – TD Cowen Sees Real Risk, But RBC Says It&#x27;s ‘Manageable’</a></li>

</ul>
</details>

**Tags**: `#Kalshi`, `#perpetual futures`, `#CFTC approval`, `#gold and silver`, `#derivatives market structure`

---

<a id="item-finance-news-2"></a>
### [Nasdaq invests $100 million in Kraken parent Payward at $21 billion valuation](https://www.coindesk.com/business/2026/09/10/nasdaq-invests-usd100-million-in-kraken-parent-company-payward-at-usd21-billion-valuation) ⭐️ 8.0/10

Nasdaq has invested $100 million in Payward, the parent company of crypto exchange Kraken, at a $21 billion valuation, according to CoinDesk. The report describes the deal as a financing event in which the $21 billion figure represents Payward&\#x27;s valuation rather than a disclosed financial result.

rss · CoinDesk · Sep 10, 11:21

**「Background」** Kraken, legally named Payward, Inc., is a US-based cryptocurrency exchange founded in 2011 that began allowing non-US customers to trade tokenized equities in 2025, and Nasdaq&\#x27;s investment expands a strategic partnership to bring tokenized, voting-enabled equities to the crypto exchange.

**「Impact」** Beyond the stake, Nasdaq and Payward plan to launch an &quot;Equity Token \(NET\)&quot; framework by the second quarter of 2027, which would put Nasdaq&\#x27;s market infrastructure behind tokenized equity trading — a change relevant to brokers and investors — though the framework&\#x27;s details and regulatory treatment were not disclosed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coindesk.com/business/2026/09/10/nasdaq-invests-usd100-million-in-kraken-parent-company-payward-at-usd21-billion-valuation">Nasdaq backs Kraken parent Payward with $100 million ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kraken_%28cryptocurrency_exchange%29">Kraken (cryptocurrency exchange) - Wikipedia</a></li>
<li><a href="https://cointelegraph.com/news/nasdaq-invests-100m-kraken-parent-21b-valuation">Nasdaq Invests $100M in Kraken Parent at $21B Valuation: Report</a></li>
<li><a href="https://www.thestreet.com/crypto/markets/nasdaq-invests-100m-in-fintech-giant-at-21b-valuation">Nasdaq invests $100 million in Kraken parent.</a></li>

</ul>
</details>

**Tags**: `#crypto exchange`, `#venture investment`, `#Nasdaq`, `#Kraken`, `#valuation`

---

<a id="item-finance-news-3"></a>
### [Federal banking agencies expand 18-month exam cycle eligibility for community banks](https://www.federalreserve.gov/newsevents/pressreleases/bcreg20260910a.htm) ⭐️ 7.0/10

Federal banking agencies announced they are reducing regulatory burden on community banks by expanding eligibility for the 18-month supervisory examination cycle. The announcement did not specify the new eligibility thresholds or timing.

rss · Federal Reserve Press Releases · Sep 10, 20:00

**「Background」** The rule implements the 21st Century ROAD to Housing Act, which raised the total asset threshold for certain supervised institutions to qualify for an extended 18-month on-site exam cycle from $3 billion to $6 billion, meaning eligible banks can qualify for on-site examinations every 18 months.

**「Who is affected」** Community banks that become eligible under the interim final rule will move to a supervisory examination every 18 months instead of every 12, cutting the time and cost they spend preparing for and responding to those reviews.

<details><summary>References</summary>
<ul>
<li><a href="https://www.federalreserve.gov/newsevents/pressreleases/bcreg20260910a.htm">Federal Reserve Board - Agencies reduce regulatory burden for ...</a></li>
<li><a href="https://www.occ.gov/news-issuances/bulletins/2026/bulletin-2026-45.html">Expanded Examination Cycle Eligibility: Interim Final Rule</a></li>
<li><a href="https://www.crowdfundinsider.com/2026/09/308981-agencies-reduce-regulatory-burden-for-community-banks-increase-eligibility-for-18-month-exam-cycle/">Agencies Reduce Regulatory Burden For Community Banks ...</a></li>

</ul>
</details>

**Tags**: `#banking regulation`, `#community banks`, `#Federal Reserve`, `#regulatory relief`, `#supervisory exams`

---

<a id="item-finance-news-4"></a>
### [Liquid Network resumes block production after $320M exploit](https://cointelegraph.com/news/liquid-network-resumes-block-production-after-320m-exploit?utm_source=rss_feed&amp;utm_medium=rss&amp;utm_campaign=rss_partner_inbound) ⭐️ 7.0/10

Liquid Network resumed block production after a reported $320M exploit, while transactions and peg operations remain suspended.

rss · Cointelegraph · Sep 10, 16:38

**Tags**: `#Liquid Network`, `#crypto exploit`, `#Bitcoin sidechain`, `#blockchain security`, `#peg operations`

---

<a id="item-finance-news-5"></a>
### [The iPhone Duo enters China’s crowded foldable market — and faces a price test](https://www.cnbc.com/2026/09/11/the-iphone-duo-enters-chinas-crowded-foldable-market.html) ⭐️ 6.0/10

Apple&\#x27;s new folding iPhone Duo is entering China&\#x27;s established foldable market at a premium price against entrenched Huawei, Xiaomi and other domestic rivals, drawing a cautious early consumer response.

rss · CNBC Finance · Sep 11, 00:19

**Tags**: `#Apple`, `#foldable smartphones`, `#China market`, `#competition`, `#consumer pricing`

---

<a id="item-finance-news-6"></a>
### [OpenAI targets work of Wall Street junior bankers with new ChatGPT for Financial Services](https://www.cnbc.com/2026/09/10/openai-chatgpt-for-financial-services-targets-work-of-junior-bankers.html) ⭐️ 6.0/10

OpenAI announced ChatGPT for Financial Services, an enterprise product built with Morgan Stanley and Evercore to automate investment-banking research and presentation tasks.

rss · CNBC Finance · Sep 10, 19:02

**Tags**: `#OpenAI`, `#ChatGPT`, `#financial services`, `#investment banking`, `#enterprise AI`

---

<a id="item-finance-news-7"></a>
### [Stocks making the biggest moves premarket: Macy&\#x27;s, Meta, Apple, Novartis and more](https://www.cnbc.com/2026/09/10/stocks-making-the-biggest-moves-premarket-.html) ⭐️ 6.0/10

A CNBC premarket roundup covering company-specific stock moves driven by earnings, guidance, analyst actions, an acquisition, and declining copper prices.

rss · CNBC Finance · Sep 10, 11:54

**Tags**: `#premarket-movers`, `#earnings`, `#guidance`, `#mergers-acquisitions`, `#market-reaction`

---

<a id="item-finance-news-8"></a>
### [BIS chief warns AI capex arms race relies on opaque debt, posing systemic risks](https://www.coindesk.com/business/2026/09/10/ai-s-rapid-rise-poses-global-financial-stability-risks-says-head-of-the-bis) ⭐️ 6.0/10

The BIS chief warns that an AI capital-expenditure arms race funded through opaque debt could pose systemic risks to financial stability.

rss · CoinDesk · Sep 10, 12:00

**Tags**: `#AI capex`, `#systemic risk`, `#debt`, `#financial stability`, `#BIS`

---