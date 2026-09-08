---
layout: default
title: "Horizon Summary: 2026-09-08 (EN)"
date: 2026-09-08
lang: en
---

> From 72 items, 14 important content pieces were selected

---

**Technology News**
1. [Interactive map shows age of LA&\#x27;s surviving buildings, 1880–2026](#item-tech-news-1) ⭐️ 6.0/10
2. [Scraper traffic outweighs legitimate access on git.kernel.org](#item-tech-news-2) ⭐️ 6.0/10
3. [OpenAI Chief Scientist Calls for Aligned AI for Defense Without Reckless Racing](#item-tech-news-3) ⭐️ 6.0/10
4. [Browser-based video compressor using FFMPEG WebAssembly](#item-tech-news-4) ⭐️ 6.0/10

**Technology Blog**
1. [Optimal Stratified Allocation for Rare-Event Forecasting](#item-tech-blog-1) ⭐️ 8.0/10
2. [AI in Equity and Crypto Markets: Progress Without Proven Net Alpha](#item-tech-blog-2) ⭐️ 8.0/10
3. [Milstein Discretisation Improves Multilevel Monte Carlo Variance Convergence](#item-tech-blog-3) ⭐️ 8.0/10
4. [Scoring Every Fill Against Your Own Rules Exposes Execution Drift](#item-tech-blog-4) ⭐️ 8.0/10
5. [Compatibility, Not Realism, Drives Synthetic Hedging Performance](#item-tech-blog-5) ⭐️ 6.0/10
6. [Agent-to-Agent Finance: Blockchain Payments and Trust Infrastructure for Autonomous Agents](#item-tech-blog-6) ⭐️ 5.0/10

**Financial News**
1. [Exchanges Hit by $320 Million Exploit on Bitcoin Network](#item-finance-news-1) ⭐️ 8.0/10
2. [China injects $54 billion into state banks and insurers](#item-finance-news-2) ⭐️ 7.0/10
3. [Ethereum Commits to Allowing Gas Fee Payments Without Holding ETH](#item-finance-news-3) ⭐️ 7.0/10
4. [Oil rises and bitcoin falls after U.S. strikes Iranian crude carriers](#item-finance-news-4) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Interactive map shows age of LA&\#x27;s surviving buildings, 1880–2026](https://lax-skyline.parcelscope.net/) ⭐️ 6.0/10

An interactive map visualizes Los Angeles buildings by their construction date across a timeline from 1880 to 2026, letting viewers watch the city&\#x27;s current building stock appear over time. Commenters caution that the map really shows the age of surviving buildings rather than the city&\#x27;s complete construction history, because neighborhoods whose original structures were fully replaced appear dark. The data appears to draw on LA County Assessor parcel records, and discussion links the pattern to Los Angeles&\#x27;s 1980s downzoning and to the city&\#x27;s former streetcar network. The project offers a striking civic-technology example but has limited technical depth.

hackernews · rustywasm · Sep 7, 18:52 · [Discussion](https://news.ycombinator.com/item?id=49601655)

**「Background」** Los Angeles is the most populous city in California, with an estimated 3.87 million residents in 2025. This interactive Parcelscope visualization shows one box for every building still standing in the city today, with each box appearing in the year that building was built. The site notes that what was torn down along the way is not included, so the map depicts the surviving city rather than the complete historical built environment.

**「Community Discussion」** Commenters generally found the visualization impressive but warned that it shows the age of extant buildings, not total construction, pointing to Palms as a neighborhood that had a 19th-century downtown whose buildings no longer survive. The discussion extended into policy debates, with one commenter blaming 1980s downzoning for LA&\#x27;s unaffordable housing and another noting the city once had the largest US public transit network before it was paved over.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Los_Angeles">Los Angeles - Wikipedia</a></li>
<li><a href="https://lax-skyline.parcelscope.net/">Every building in Los Angeles</a></li>

</ul>
</details>

**Tags**: `#visualization`, `#los-angeles`, `#urban-data`, `#geospatial`, `#civic-tech`

---

<a id="item-tech-news-2"></a>
### [Scraper traffic outweighs legitimate access on git.kernel.org](https://simonwillison.net/2026/Sep/7/creepy-crawlies/) ⭐️ 6.0/10

Konstantin Ryabitsev reports that abusive scraper traffic now consumes more CPU on git.kernel.org—the official Git repository for the Linux kernel—than all legitimate access combined, including git clones. Across the service&\#x27;s five geo-distributed nodes, 14 CPU cores are continuously rendering git commits as HTML solely for scrapers. Simon Willison highlights the report and connects it to his own concern about Datasette, which serves many crawlable web pages. The finding underlines how much infrastructure cost background crawler traffic can impose on public code-repository and data-heavy web services.

rss · Simon Willison · Sep 7, 23:08

**「Background」** git.kernel.org is the official home for Linux kernel Git repositories, where users can clone code and also view commits as rendered HTML pages. Web scrapers and automated crawlers fetch those pages at high volume, forcing the service to spend CPU cycles generating responses even though the requests are not from humans or conventional development tooling.

**「Impact」** For Linux kernel infrastructure operators, crawler load has become a dominant CPU cost, and operators of similarly public, crawlable code or data services should expect comparable background radiation from scrapers.

**Tags**: `#crawlers`, `#git.kernel.org`, `#infrastructure`, `#web scraping`

---

<a id="item-tech-news-3"></a>
### [OpenAI Chief Scientist Calls for Aligned AI for Defense Without Reckless Racing](https://simonwillison.net/2026/Sep/7/jakub-pachocki/) ⭐️ 6.0/10

OpenAI Chief Scientist Jakub Pachocki published a statement arguing that continuing to train much smarter models quickly is justified by the need to build defensive systems against dangers posed by other AI. He wrote that powerful, aligned AI will be needed to secure infrastructure, protect against rogue agents in real time, and invent new protective measures, and said this will be a primary focus of OpenAI’s deployment efforts. At the same time, Pachocki cautioned that the need for defensive systems must not become an excuse for recklessness, calling the idea of racing forward at all costs &quot;absurd&quot; given the seriousness of the stakes. The remarks come from the OpenAI post &quot;An Alien Mind&quot; and were shared by Simon Willison, but include no new technical details or specific deployment timelines.

rss · Simon Willison · Sep 7, 22:26

**「Background」** Jakub Pachocki is OpenAI&\#x27;s Chief Scientist, and the quoted text comes from his post &quot;An Alien Mind&quot; published on September 6. In the post&\#x27;s &quot;Scalable defense&quot; section, he argues that continuing to train much smarter models is justified by the need to build aligned defensive systems against dangers posed by other AI, such as cyberattacks, while warning that this is not an excuse for reckless racing. OpenAI says these defensive systems will be a primary focus of its deployment efforts.

**「Impact」** The statement publicly signals OpenAI&\#x27;s intention to prioritize defensive aligned AI in its deployment strategy while rejecting all-costs racing, though it offers no concrete technical specifics or measurable commitments.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/an-alien-mind/">An Alien Mind | OpenAI</a></li>
<li><a href="https://www.lesswrong.com/posts/8E6ng6CseuzafSxQR/an-alien-mind-jakub-pachocki-warns-us">OpenAI Chief Scientist Jakub Pachocki is dropping truth bombs. …</a></li>
<li><a href="https://cryptobriefing.com/openai-chief-scientist-ai-risks-warning/">OpenAI &#x27;s chief scientist warns that advanced AI models are...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#OpenAI`, `#AI ethics`, `#Artificial Intelligence`

---

<a id="item-tech-news-4"></a>
### [Browser-based video compressor using FFMPEG WebAssembly](https://simonwillison.net/2026/Sep/7/video-compressor/) ⭐️ 6.0/10

Simon Willison published a browser-based &quot;Video compressor&quot; tool at tools.simonwillison.net/video-compressor, built from FFMPEG&\#x27;s WebAssembly build and generated with Claude Fable 5.1 in Claude Code for web, after recording a phone demo video for his Equal Earth animation post. The tool supports five presets \(Largest to Smallest\) with output resolutions of 854×370 or 640×276, CRF quality settings from 22 to 28, audio bitrates from 128 to 64 kbps, plus options such as encoder speed, H.264 profile, 30 fps limit, metadata stripping, dropping audio, and limiting encoding to the first 10 seconds. In the screenshot example, generating five versions took 11.8 seconds, producing files of 145 KB \(48% of original\), 241 KB \(79%\), and 264 KB \(87%\) for the smallest sizes, each with an individual Download .mp4 button and a collapsible ffmpeg command. It is an incremental convenience rather than a major technical breakthrough.

rss · Simon Willison · Sep 7, 18:29

**「Background」** FFMPEG is a widely used command-line tool for transcoding and compressing video. WebAssembly builds of FFMPEG let that processing happen entirely in the user&\#x27;s browser, avoiding the need for a server-side encoding job and keeping source videos off remote machines.

**「Impact」** Users who want optimized MP4 versions for web publishing can now compress videos directly in their browser with selectable presets and inspect the underlying ffmpeg commands, which is immediately useful for Simon Willison&\#x27;s audience of web technologists. The tool remains an incremental convenience rather than a novel compression breakthrough needing broader ecosystem changes.

**Tags**: `#ffmpeg`, `#webassembly`, `#video-compression`, `#tools`, `#simon-willison`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Optimal Stratified Allocation for Rare-Event Forecasting](https://arxiv.org/abs/2609.04420) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Sep 7, 04:00

**「Background」** When forecasting rare events, estimating total risk from a small subsample is complicated by class imbalance. A finite population of n labeled examples has a rare positive class weighted by the imbalance ratio, and we must allocate K0 and K1 draws to the positive and negative strata.

**「Solution」** The author derives exact finite-population variance for the weighted risk estimator under class-conditional sampling without replacement and solves for the optimal allocation. The key finding is that the class multiplier inflates positive-stratum dispersion by the imbalance ratio, causing that ratio to cancel from the optimal allocation. Equal allocation, rather than proportional allocation, becomes the natural default. Simple random sampling is dominated by an explicit between-stratum term, while an exact bias identity shows that cluster-representative selection has no general unbiasedness guarantee. A Serfling bound transfers the allocation result to selection error over a finite candidate set. Under the implemented truncation, the realized allocation ratio is independent of n, yielding a parameter-free efficiency prediction. The author tests this on forecasting explosive price-regime onsets in 350 U.S. equities from 2004-2011 with under 1% positive rows. The predicted ordering of four designs holds, and at the 10-day horizon the five design points are ordered exactly as predicted \(Spearman rho=1, exact p=0.0167\). The predicted dependence on pi across horizons did not hold, and the author identifies channels lying outside the design-based argument.

**「Takeaway」** The core message is that class imbalance cancels in optimal stratified allocation, making equal allocation the natural default for rare-event risk estimation. The empirical confirmation of design ordering supports the theory, while the failed pi-dependence highlights its boundary conditions.

**Tags**: `#stratified sampling`, `#rare-event forecasting`, `#finite-population inference`, `#design-based estimation`, `#explosive price regimes`

---

<a id="item-tech-blog-2"></a>
### [AI in Equity and Crypto Markets: Progress Without Proven Net Alpha](https://arxiv.org/abs/2609.04917) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Sep 7, 04:00

**「Background」** Artificial intelligence now touches every stage of investing, from data and prediction to portfolios and execution, but the author&\#x27;s starting point is that technical capability is not evidence of profitability. Reviewing public research on listed equities, ETFs, crypto spot, perpetual futures, and on-chain markets through 31 August 2026, they frame the question as whether research findings can travel along an alpha-translation chain.

**「Solution」** The chain requires point-in-time information to become a stable signal, a feasible position, an executable order, and risk-adjusted returns after costs. Across machine learning, time-series foundation models, financial language models, reinforcement learning, and agents, the author finds real but mostly upstream progress in prediction, text processing, portfolio design, and workflow integration, with thinner evidence for durable net performance. Temporal contamination, repeated selection, survivorship, weak benchmarks, implementation costs, venue mechanics, and capacity can break translation to net alpha. Strong historical results coexist with predictor decay, corrected look-ahead failures, mixed prospective evidence, and few audited live-capital records. Crypto markets add informative state but require separate treatment of spot, perpetual, decentralized cash flows, and execution. Within the public evidence, no general AI architecture has demonstrated persistent, cross-regime, capacity-aware net alpha.

**「Takeaway」** The author&\#x27;s conclusion is methodological: credible profitability claims require point-in-time data and models, decision-aligned objectives, joint portfolio-execution evaluation, controlled adaptation, prospective tests, and authority-matched governance. Meeting these conditions can improve evidence quality, but it guarantees no profit.

**Tags**: `#artificial-intelligence-investing`, `#alpha-translation`, `#financial-machine-learning`, `#evidence-evaluation`, `#crypto-markets`

---

<a id="item-tech-blog-3"></a>
### [Milstein Discretisation Improves Multilevel Monte Carlo Variance Convergence](https://arxiv.org/abs/1302.4676) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Sep 7, 04:00

**「Background」** Multilevel Monte Carlo \(MLMC\) path simulation estimates expectations of stochastic differential equations by combining simulations at different levels of resolution, exploiting strong convergence to reduce computational cost. The original method used the Euler-Maruyama discretisation, whose strong-convergence order limits how quickly the multilevel variance shrinks as mesh levels are refined.

**「Solution」** The authors analyse replacing Euler-Maruyama with the Milstein discretisation, which has a better order of strong convergence. They prove that this improved strong convergence translates into an improved convergence order for the variance of the multilevel estimator, meaning fewer fine-level samples are needed for a given accuracy and the overall computational complexity is reduced. The analysis is rigorous rather than merely heuristic, clarifying the theoretical link between strong convergence and multilevel variance decay. Numerical results on basket options are included to demonstrate the practical relevance of the proved variance improvement. Because the available source is only the abstract, detailed constants, proof structure, and full experimental settings are not presented here.

**「Takeaway」** The paper shows that choosing a higher-order strong discretisation like Milstein can provably improve the variance convergence of multilevel Monte Carlo, extending Giles&\#x27; original method and offering a more efficient path simulation strategy for applications such as option pricing.

**Tags**: `#multilevel Monte Carlo`, `#Milstein discretisation`, `#strong convergence`, `#variance analysis`, `#computational finance`

---

<a id="item-tech-blog-4"></a>
### [Scoring Every Fill Against Your Own Rules Exposes Execution Drift](https://www.reddit.com/r/algotrading/comments/1wa1drh/scored_every_fill_against_what_my_rules_said_and/) ⭐️ 8.0/10

reddit · r/algotrading · /u/david19790 · Sep 7, 19:10

**「Background」** The author had a period where the backtest looked fine but the live account did not, and initially assumed there was a bug in the strategy. In the end, the strategy was fine—he was simply not trading it as written, and he wanted to quantify how much that drift actually cost.

**「Solution」** He describes an audit built from three mechanical questions, all run on the same trade log. First, replay every trade with exits forced back to the original stop or target, keeping the same entries, and compare the two equity curves: in his case, the gap from discretionary interventions was bigger than his worst losing month, mostly from cutting trades that went green and then stalled. Second, examine MAE \(maximum adverse excursion\) on winners only: half of his winners on one instrument routinely travelled about 80% of the stop distance, which meant the stop sat inside normal noise. Widening the stop while cutting size to keep dollar risk flat moved win rate more than any entry filter he had built. Third, for every trade moved to breakeven, check what it did afterwards against the original target: 41% of those trades would have hit target, so the breakeven move was not protection but a leak that felt like discipline. None of this appeared in monthly P&amp;L totals, which looked only mildly disappointing; the signal showed up only in the distributions. The audit needs just four log columns—entry, exit, MAE, and planned stop per trade—and the author shared the code on his profile, while acknowledging he still cannot cleanly separate a genuine regime change from his own execution drift when live results trail the tester.

**「Takeaway」** The author&\#x27;s core point is that execution drift can be invisible in monthly totals yet cost more than the worst losing month, so the gap between backtest and live performance is often found in distribution-level checks rather than in a strategy bug. The broader lesson is that mechanical audits of fills against your own rules can reveal costly discretion that feels like discipline.

**Tags**: `#algorithmic trading`, `#trade execution audit`, `#MAE analysis`, `#risk management`, `#backtest vs live`

---

<a id="item-tech-blog-5"></a>
### [Compatibility, Not Realism, Drives Synthetic Hedging Performance](https://arxiv.org/abs/2608.20842) ⭐️ 6.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Sep 7, 04:00

**「Background」** Deep hedging learns strategies by training on synthetic price paths, because real market data is often too limited. The authors argue that existing approaches judge these generators by statistical realism, but leave unclear whether realism actually improves downstream hedging performance.

**「Solution」** They propose a decision-centric perspective based on compatibility, which asks whether strategies trained on synthetic scenarios remain effective in the true market. Theoretically, they show that hedging performance decomposes into a learning error and a compatibility gap, and that realism and compatibility can diverge. Empirically, they report that performance is governed not by realism alone, but by alignment between the generator and the hedger, together with task structure. This reframing suggests synthetic-data design should target the downstream decision rather than general data-quality benchmarks.

**「Takeaway」** The authors&\#x27; central point is that synthetic scenario generators for deep hedging should be evaluated by task compatibility, not statistical fidelity. This offers a principled basis for decision-aligned synthetic data generation in finance.

**Tags**: `#deep hedging`, `#synthetic data`, `#financial machine learning`, `#scenario generation`, `#decision-centric evaluation`

---

<a id="item-tech-blog-6"></a>
### [Agent-to-Agent Finance: Blockchain Payments and Trust Infrastructure for Autonomous Agents](https://arxiv.org/abs/2607.00245) ⭐️ 5.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Sep 7, 04:00

**「Background」** As AI agents evolve from analytical tools into transacting counterparties that can negotiate, pay, and record actions, financial markets need infrastructure for identity, authorisation, payment, verification, reputation, and accountability. Hui Gong argues these coordination frictions are not solved by treating agents as ordinary users or by assuming existing payment rails suffice.

**「Solution」** Drawing on recent developments in blockchain-based agent-to-agent payments, ERC-8004 agent registries, provenance-based wallets, deterministic inference, DeFi intent mining, and adoption evidence, Gong frames agent-to-agent finance as a machine-mediated layer for discovering counterparties, purchasing services, expressing transaction intent, executing payments, and generating auditable evidence. The core insight is targeted, not universal: programmable settlement, smart wallets, decentralised registries, and verifiable computation address specific frictions created by autonomous agents, but blockchain is not positioned as a universal financial substrate. Gong identifies bounded autonomy as the decisive design question—how to expand the set of actions agents may safely perform without making markets more opaque, fragile, or unaccountable. Because the chapter is at the conceptual level, the concrete mechanisms and their evaluation remain largely open.

**「Takeaway」** Agent-to-agent finance is best understood as emerging financial market infrastructure whose central design problem is bounded autonomy—not whether agents can act economically, but how to let them act without sacrificing transparency and accountability.

**Tags**: `#agent-to-agent finance`, `#blockchain`, `#autonomous agents`, `#trust infrastructure`, `#DeFi`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Exchanges Hit by $320 Million Exploit on Bitcoin Network](https://www.coindesk.com/markets/2026/09/07/bitcoin-network-used-by-exchanges-hit-by-usd320-million-exploit-hackers-claim-they-re-the-good-guys) ⭐️ 8.0/10

A reported $320 million exploit hit a Bitcoin-related network used by exchanges, and the hackers described the attack as a &\#x27;good guy&\#x27; operation.

rss · CoinDesk · Sep 7, 03:43

**「Background」** Liquid Network is a Bitcoin sidechain — a separate ledger developed by Blockstream — that exchanges and financial institutions use to settle bitcoin payments faster than on Bitcoin&\#x27;s main network, with funds held in a federation wallet controlled by multiple parties.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theregister.com/security/2026/09/07/hackers-drain-320m-in-bitcoin-from-liquid-network-claim-theyre-the-good-guys/5294770">Hackers drain $320M in Bitcoin from Liquid Network, claim ...</a></li>
<li><a href="https://www.ibtimes.com/bitcoin-network-lost-320-million-hack-attackers-say-theyre-good-guys-3807199">A Bitcoin Network Lost $320 Million In A Hack. The Attackers ...</a></li>

</ul>
</details>

**Tags**: `#Bitcoin`, `#cryptocurrency exchange`, `#security breach`, `#market impact`, `#hacking`

---

<a id="item-finance-news-2"></a>
### [China injects $54 billion into state banks and insurers](https://www.cnbc.com/2026/09/07/china-state-banks-lenders-insurers-capital-solvency-bankrupt-nim-.html) ⭐️ 7.0/10

China&\#x27;s finance ministry is leading a 360 billion yuan \($53.6 billion\) capital injection into three state banks and five insurers, a package Citibank said was smaller than markets had expected, and Hong Kong-listed shares of the institutions fell Monday.

rss · CNBC Finance · Sep 7, 23:23

**「Background」** The move follows a 500 billion yuan injection into four major state banks last year and a March pledge to issue 300 billion yuan in special treasury bonds this year; it comes as lenders&\#x27; net interest margins, the spread between income from loans and cost of deposits, have fallen to record lows as Beijing pressed banks to keep credit cheap.

**「Impact」** Analysts cited in the report say the larger capital cushion gives banks room to write off non-performing loans and helps prepare them to fund future priorities such as AI, though some economists expect only limited short-term economic impact because credit demand is weak.

**Tags**: `#China`, `#state banks`, `#capital injection`, `#insurers`, `#financial policy`

---

<a id="item-finance-news-3"></a>
### [Ethereum Commits to Allowing Gas Fee Payments Without Holding ETH](https://www.coindesk.com/tech/2026/09/07/ethereum-commits-to-letting-users-pay-gas-fees-without-having-to-hold-eth) ⭐️ 7.0/10

Ethereum has committed to letting users pay network gas fees without having to hold ETH, according to a report from CoinDesk. This is a roadmap commitment rather than an immediate market event, and it is intended to remove a key usability barrier for new users.

rss · CoinDesk · Sep 7, 13:54

**「Background」** Ethereum developers have scheduled the Hegotá hard fork, expected in 2027, to introduce &\#x27;Frame Transactions&\#x27;—a mechanism that lets apps or other accounts pay a user&\#x27;s gas fees in ether on their behalf, so users don&\#x27;t need to hold ETH. Vitalik Buterin is one of the proposal&\#x27;s authors.

**「Potential effect」** If the planned 2027 Hegotá upgrade is implemented, Ethereum users could pay gas fees with ERC-20 tokens instead of holding ETH, potentially lowering the barrier for new users and making token holders less dependent on ETH.

<details><summary>References</summary>
<ul>
<li><a href="https://cryptobriefing.com/ethereum-gas-fees-without-eth-2027/">Ethereum set to enable gas fee payments without holding ETH ...</a></li>
<li><a href="https://www.coindesk.com/tech/2026/09/07/ethereum-commits-to-letting-users-pay-gas-fees-without-having-to-hold-eth">ETH news: Ethereum commits to letting users pay gas fees ...</a></li>
<li><a href="https://coinlaw.io/ethereum-frame-transactions-gas-fees/">Ethereum Locks In Plan to Let Users Pay Gas Without ETH</a></li>
<li><a href="https://cryptobriefing.com/ethereum-gas-fees-without-eth-2027/">Ethereum set to enable gas fee payments without holding ETH in...</a></li>

</ul>
</details>

**Tags**: `#Ethereum`, `#gas fees`, `#cryptocurrency`, `#blockchain`, `#protocol development`

---

<a id="item-finance-news-4"></a>
### [Oil rises and bitcoin falls after U.S. strikes Iranian crude carriers](https://www.coindesk.com/markets/2026/09/07/oil-up-bitcoin-down-as-u-s-strikes-iranian-crude-carriers) ⭐️ 7.0/10

U.S. strikes on Iranian crude carriers were followed by higher oil prices and lower bitcoin prices, reflecting heightened geopolitical risk. No specific price figures or comparison baselines were included in the available report.

rss · CoinDesk · Sep 7, 04:44

**「Background」** On Saturday, U.S. Central Command confirmed it had struck three Iranian oil tankers near Kharg Island, escalating the U.S.-Iran conflict. Following those strikes, crude oil prices rose while bitcoin fell.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coindesk.com/markets/2026/09/07/oil-up-bitcoin-down-as-u-s-strikes-iranian-crude-carriers">Oil up, bitcoin down as U.S. strikes Iranian crude carriers</a></li>
<li><a href="https://bitcoinethereumnews.com/bitcoin/oil-up-bitcoin-down-as-us-strikes-iranian-crude-carriers/">Oil up, Bitcoin down as US strikes Iranian Crude carriers</a></li>
<li><a href="https://www.fxstreet.com/cryptocurrencies/news/oil-up-bitcoin-down-as-us-strikes-iranian-crude-carriers-202609071018">Oil up, Bitcoin down as US strikes Iranian Crude carriers | FXStreet</a></li>

</ul>
</details>

**Tags**: `#oil prices`, `#bitcoin`, `#Iran`, `#geopolitical risk`, `#markets`

---