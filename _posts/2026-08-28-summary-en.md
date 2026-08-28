---
layout: default
title: "Horizon Summary: 2026-08-28 (EN)"
date: 2026-08-28
lang: en
---

> From 113 items, 20 important content pieces were selected

---

**Technology News**
1. [Cloudflare saves 100 TB by optimizing 1.1.1.1 DNS cache](#item-tech-news-1) ⭐️ 8.0/10
2. [Prompt Injection Breaks Claude Code Auto Mode via Zip Import](#item-tech-news-2) ⭐️ 8.0/10
3. [Small Language Models Arrive](#item-tech-news-3) ⭐️ 7.0/10
4. [Gemini-3.5-Transcribe leads in STT accuracy but trails in latency](#item-tech-news-4) ⭐️ 7.0/10
5. [Data analysis flags Claude&\#x27;s overused PR vocabulary](#item-tech-news-5) ⭐️ 7.0/10
6. [Stripe, Advent Said to Drop $50B PayPal Pursuit](#item-tech-news-6) ⭐️ 7.0/10

**Technology Blog**
1. [A Pairs Screener and the Lookahead Bias That Killed Its Edge](#item-tech-blog-1) ⭐️ 9.0/10
2. [Regime-Robust Bayesian Optimisation for Tabular Trading Signal Generation](#item-tech-blog-2) ⭐️ 8.0/10
3. [Tail-Weighted Maximal Deficit and Optimal Reserve Allocation](#item-tech-blog-3) ⭐️ 8.0/10
4. [Scalable Adjoint-Guided Recovery for Constrained Dynamic Portfolio Choice](#item-tech-blog-4) ⭐️ 8.0/10
5. [Interpretable hybrid credit scoring with fairness audit for thin-file borrowers](#item-tech-blog-5) ⭐️ 7.0/10
6. [Reading the Labor Market Pulse from 750M Chinese Job Ads](#item-tech-blog-6) ⭐️ 7.0/10

**Financial News**
1. [Nvidia, Salesforce, Okta jump on earnings beats in midday stock moves](#item-finance-news-1) ⭐️ 8.0/10
2. [Salesforce stock jumps 20% after earnings, lifting software sector](#item-finance-news-2) ⭐️ 8.0/10
3. [Nvidia shares rise 8% after earnings beat, boosting tech stocks and bitcoin](#item-finance-news-3) ⭐️ 8.0/10
4. [Fed&\#x27;s Schmid: Inflation sticky, policy rate may not be restrictive](#item-finance-news-4) ⭐️ 7.0/10
5. [Premarket stock movers: Nvidia and Salesforce surge after earnings, HP drops](#item-finance-news-5) ⭐️ 7.0/10
6. [Judge: Trump administration&\#x27;s blacklist of Anthropic violated First Amendment](#item-finance-news-6) ⭐️ 7.0/10
7. [Mirae Asset Acquires Digital X, Targets $109B Crypto Business](#item-finance-news-7) ⭐️ 7.0/10
8. [Solana Governance Vote Advances Faster Supply Cuts; Daily Burn Plan Trails](#item-finance-news-8) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Cloudflare saves 100 TB by optimizing 1.1.1.1 DNS cache](https://blog.cloudflare.com/dns-cache-memory-optimization-1111/) ⭐️ 8.0/10

Cloudflare described how it saved 100 terabytes of memory by optimizing the DNS cache of its 1.1.1.1 resolver. The engineering post details concrete techniques such as reducing per-entry allocations, improving data structure layout and alignment, and lowering per-record overhead in the Rust-based cache implementation. The result is a dramatic memory reduction that directly lowers infrastructure costs and increases capacity for one of the world&\#x27;s largest public DNS services. The work shows that careful systems-level tuning of data representation and memory allocation can yield huge savings when applied at scale, despite the optimizations being individually modest.

hackernews · TangerineDream · Aug 27, 17:17 · [Discussion](https://news.ycombinator.com/item?id=49468083)

**「Background」** The 1.1.1.1 service is Cloudflare&\#x27;s public DNS resolver, which stores recently resolved domain names in a cache to answer queries quickly. Cloudflare&\#x27;s DNS server, called Big Pineapple, is written in Rust, and because it can hold roughly 250 billion cache entries, even a one-byte saving per entry translates to roughly 250 GB of memory across the fleet. The optimization work focused on reducing the per-entry memory footprint of the DNS cache by reworking data structures and allocation patterns, which is what allowed Cloudflare to eventually free about 100 TB of memory and improve performance.

**「Impact」** Cloudflare&\#x27;s optimization frees roughly 100 TB of memory across its DNS infrastructure, lowering operational costs and improving headroom for 1.1.1.1&\#x27;s global user base. For systems programmers, the write-up offers concrete, evidence-backed examples of how allocation strategy and struct layout affect real-world memory usage at scale.

**「Community discussion」** Commenters generally praised Cloudflare&\#x27;s approach of validating the product before optimizing, with one noting that optimization is the easiest part once the system works. Some suggested further improvements, such as embedding record data directly after CacheEntry members instead of using separate allocations, while another cited a similar single-malloc optimization in MaraDNS that cut blacklist memory from 237 MB to 9.5 MB. A few expressed concern that merging distinct lists into a shared structure could weaken Rust&\#x27;s memory safety guarantees.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/dns-cache-memory-optimization-1111/">How we saved 100 terabytes of memory by optimizing 1.1.1.1’s DNS cache | Cloudflare Blog</a></li>
<li><a href="https://x.com/Cloudflare/status/2093031959106580956">Cloudflare (@Cloudflare) on X</a></li>

</ul>
</details>

**Tags**: `#DNS`, `#memory-optimization`, `#systems-programming`, `#Cloudflare`, `#performance`

---

<a id="item-tech-news-2"></a>
### [Prompt Injection Breaks Claude Code Auto Mode via Zip Import](https://simonwillison.net/2026/Aug/27/breaking-claude-code-opus-5-auto-mode/) ⭐️ 8.0/10

Prompt injection researcher Johann Rehberger found a practical attack against Claude Code&\#x27;s default auto mode that reportedly succeeds 80% of the time. The attack tricks Claude Code into downloading and uncompressing a zip archive, then executing code that imports base64 without noticing that a local struct.py file extracted from the archive will be imported and executed instead. In several runs, Claude detected the compromise and tried to terminate the malicious process, but auto mode blocked the cleanup command, meaning the safety mechanism itself became part of the failure. Anthropic had recently made auto mode the default and made bold claims about its effectiveness. Rehberger and Simon Willison conclude that the only safe way to run agents at risk of adversarial attack is to use a container, VM, or OS sandbox, restrict network egress, monitor agents, and avoid exposing home directories, SSH keys, and cloud credentials to the agent runtime.

rss · Simon Willison · Aug 27, 22:50

**「Background」** Claude Code is Anthropic&\#x27;s coding agent, and auto mode is a safety feature intended to automatically approve or deny actions based on a classifier, protecting users from prompt injection attacks that manipulate the agent into executing harmful commands. Prompt injection attacks work by embedding adversarial instructions in content the agent reads, and this attack exploits Python&\#x27;s import behavior so that a malicious local file runs without the agent recognizing the substitution.

**「Impact」** Users of Claude Code in auto mode should not rely solely on its built-in protections and should run unattended coding agents in a sandbox, restrict network egress, monitor activity, and keep sensitive credentials out of the agent&\#x27;s environment.

**Tags**: `#prompt injection`, `#security`, `#AI agents`, `#Claude`, `#vulnerability`

---

<a id="item-tech-news-3"></a>
### [Small Language Models Arrive](https://calv.info/small-models-have-arrived) ⭐️ 7.0/10

An analysis argues that small language models have now become practically useful and predicts that demand for fast, cheap, good-enough models is about to take off, with significant implications for startups and consumer AI. The piece contrasts frontier labs&\#x27; ambitions to dominate the market with the opportunity for contrarian founders to build products and services that address specific consumer needs. Community commenters connect this shift to early 2024 experiences with 7B local models, such as using Guidance to drive test-generation and coding workflows before thinking models existed. They also observe that large parameter counts bundle world knowledge, language skills, and reasoning primitives, and that many applications do not need all of that capability, creating room for smaller models.

hackernews · tosh · Aug 27, 15:56 · [Discussion](https://news.ycombinator.com/item?id=49466917)

**「Background」** Small language models are compact AI models designed to run locally or at low cost, in contrast to frontier large-parameter models such as Fable 5 or 5.6 Sol, which are the most expensive and capable options for coding work. The article argues that recent progress has made small models surprisingly capable and affordable, with costs around $0.10 per interaction, reducing inference costs and making consumer AI applications more viable. The Hacker News discussion draws a parallel to compute, suggesting inference is becoming an integrated part of products rather than a distinguishing feature.

**「Impact」** For startups and product builders, the growing viability of small models lowers deployment costs and opens space for consumer AI applications that compete on specific, practical value rather than raw model scale.

**「Community Discussion」** Commenters largely agree with the analysis, sharing concrete experiences with 7B local models in code-generation loops and framing large parameter counts as a mix of world knowledge, language skills, and reasoning primitives that is unnecessary for many tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://calv.info/small-models-have-arrived">Small Models Have Arrived</a></li>
<li><a href="https://news.ycombinator.com/item?id=49466917">Small Models Have Arrived | Hacker News</a></li>
<li><a href="https://hn.today/s/small-models-have-arrived">Small Models Have Arrived · hn.today</a></li>

</ul>
</details>

**Tags**: `#small language models`, `#AI startups`, `#local models`, `#inference efficiency`, `#consumer AI`

---

<a id="item-tech-news-4"></a>
### [Gemini-3.5-Transcribe leads in STT accuracy but trails in latency](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-5-transcribe/) ⭐️ 7.0/10

Google announced Gemini-3.5-Transcribe, a new speech-to-text model focused on high transcription accuracy. Early community testing indicates it beats other speech-to-text models on accuracy, but several developers report that latency remains a critical weakness for real-time applications. One developer comparing models for a real-time translator found Soniox STT v5 still preferable on latency, while another benchmark across multilingual, industry-specific meetings favored Voxtral Mini 3b locally and ElevenLabs&\#x27; paid API. The release shows Google pushing to lead STT accuracy, but practical deployments may still need to weigh accuracy against response time.

hackernews · k9294 · Aug 27, 18:03 · [Discussion](https://news.ycombinator.com/item?id=49468818)

**「Background」** Gemini 3.5 Transcribe is Google&\#x27;s newly announced speech-to-text model in the Gemini 3.5 family, promoted as a more intelligent transcription engine that can produce polished text by removing filler words such as &\#x27;ums&\#x27; and self-corrections. It is part of Google DeepMind&\#x27;s Gemini Audio work and is also positioned for multilingual transcription and translation. The release continues the Gemini model line&\#x27;s expansion beyond text and multimodal chat into dedicated audio and voice processing tasks.

**「Impact」** For real-time speech-to-text use cases, developers may still choose lower-latency options such as Soniox STT v5, while Gemini-3.5-Transcribe&\#x27;s accuracy advantage matters most where batch transcription is acceptable. On-device testing on the Pixel 11 Pro also suggests the model can simplify precise wording and alter intended meaning, so exact-language tasks may still require human review.

**「Community Discussion」** Commenters largely agree Gemini-3.5-Transcribe sets an accuracy benchmark, but they emphasize latency and real-world precision as differentiators. One multi-model benchmark found local Voxtral Mini 3b and ElevenLabs&\#x27; paid API better for mixed-language, industry-specific audio; another tester on the Pixel 11 Pro reported the model sometimes drops qualifying phrases that change meaning.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-5-transcribe/">Introducing Gemini 3.5 Transcribe - The Keyword</a></li>
<li><a href="https://deepmind.google/models/gemini-audio/ai-transcription/">Gemini Audio – AI transcription — Google DeepMind</a></li>
<li><a href="https://arstechnica.com/ai/2026/08/google-announces-gemini-3-5-transcribe-for-ai-powered-speech-to-text/">Google announces Gemini 3.5 Transcribe for AI-powered speech ...</a></li>

</ul>
</details>

**Tags**: `#speech-to-text`, `#Gemini`, `#AI models`, `#Google`, `#latency`

---

<a id="item-tech-news-5"></a>
### [Data analysis flags Claude&\#x27;s overused PR vocabulary](https://louisabraham.github.io/load-bearing/) ⭐️ 7.0/10

An analysis of Claude&\#x27;s responses, built from large-scale pull-request review data, identifies &\#x27;load-bearing&\#x27; as part of a repeated vocabulary the model leans on in software workflows. The project publishes a daily-updated dataset and page via GitHub Actions, with the author planning to expand collection to 1,000 pull requests per day and add search. It highlights how AI-assisted code review can drift toward clichéd phrasing that signals insight rather than explaining mechanisms. The presentation is intentionally concise, contrasting with verbose LLM output, and has drawn broad developer discussion.

hackernews · Labo333 · Aug 27, 08:59 · [Discussion](https://news.ycombinator.com/item?id=49461817)

**「Background」** Claude is Anthropic&\#x27;s AI assistant commonly used in software development, and its code-review comments are known for distinctive stock phrases. This project clustered 461,121 GitHub pull requests by vocabulary alone and found that one writing style—marked by terms like &quot;load-bearing,&quot; &quot;the crux,&quot; and &quot;first-class citizen&quot;—grew from 0.7% to 39% over eighteen months. The result is presented as an interactive, daily-updated dictionary of Claude&\#x27;s characteristic language, highlighting how AI-generated text has become a measurable part of developer communication.

**「Impact」** Developers who rely on Claude for code review can use the list to recognize and prompt away from clichéd feedback, though the effect is stylistic rather than a correctness issue.

**「Community discussion」** Commenters shared prompt-level mitigations, such as adding Orwell&\#x27;s rule against familiar metaphors to their global prompt, and noted Claude explicitly acknowledged the instruction conflicts with its system prompt. Others observed the pattern seems to be worsening across models and speculated that training on AI-generated text may be compounding the style.

<details><summary>References</summary>
<ul>
<li><a href="https://topaihubs.com/articles/claude-s-load-bearing-vocabulary-unpacking-the-ai-s-core-language-insights">Claude&#x27;s &quot;Load-Bearing Vocabulary&quot;: Unpacking the AI&#x27;s Core ...</a></li>
<li><a href="https://boingboing.net/2026/08/27/claudes-load-bearing-vocabulary-charted.html">Claude&#x27;s &quot;load-bearing&quot; vocabulary charted - Boing Boing</a></li>
<li><a href="https://ai-tldr.dev/releases/louisabraham-load-bearing-vocabulary/">The load-bearing vocabulary of Claude — 461,121… | AI/TLDR</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#Claude`, `#data-analysis`, `#software-engineering`

---

<a id="item-tech-news-6"></a>
### [Stripe, Advent Said to Drop $50B PayPal Pursuit](https://www.bloomberg.com/news/articles/2026-08-28/advent-stripe-consortium-is-said-to-drop-pursuit-of-paypal) ⭐️ 7.0/10

Bloomberg reported that Stripe and Advent have abandoned a roughly $50 billion pursuit of PayPal, ending takeover speculation that had pushed PayPal&\#x27;s shares up more than 40% this quarter to a market value of about $52.6 billion. The collapse removes the prospect of a transformative acquisition in U.S. digital payments and leaves PayPal to compete as a standalone company. Neither Stripe, Advent, nor PayPal has publicly confirmed the talks, so the report is based on unnamed sources.

hackernews · 1986 · Aug 28, 01:57 · [Discussion](https://news.ycombinator.com/item?id=49473483)

**「Background」** PayPal is a longtime fintech pioneer that processes online payments, but it has faced slowing growth and increased competition in recent years. In July 2026, buyout firm Advent International and payment processor Stripe reportedly made a joint offer to acquire PayPal for $60.50 per share, valuing the company at more than $53 billion, which sent PayPal&\#x27;s stock up more than 40%. The consortium has now abandoned that pursuit, according to Bloomberg News.

**「Impact」** PayPal shareholders lose the takeover premium that deal speculation had built into the stock, and PayPal will face continued pressure to modernize its payments platform without an acquirer.

**「Community Discussion」** Commenters were skeptical of PayPal&\#x27;s long-term prospects: several called its technology dated or questioned its innovation, one said leaks made the target too expensive, and another raised U.S. antitrust obstacles to a deal.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-28/advent-stripe-consortium-is-said-to-drop-pursuit-of-paypal">PayPal Deal Talks End as Advent, Stripe Group Abandons Acquisition Effort - Bloomberg</a></li>
<li><a href="https://www.cnbc.com/2026/07/15/stripe-advent-offer-to-buy-paypal-for-more-than-53-billion-reuters.html">Stripe, Advent make $53 billion takeover offer for PayPal, sending stock soaring</a></li>

</ul>
</details>

**Tags**: `#fintech`, `#acquisitions`, `#payments`, `#tech industry`, `#Stripe`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [A Pairs Screener and the Lookahead Bias That Killed Its Edge](https://www.reddit.com/r/algotrading/comments/1w06uxd/made_a_pairs_screener_for_us_equities_17_million/) ⭐️ 9.0/10

reddit · r/algotrading · /u/Finance\_\_broski · Aug 27, 21:18

**「Background」** Pairs trading depends on finding equity pairs whose prices stay cointegrated, but a backtest can quietly lean on the future. The author built a weekly screener for roughly 1,900 liquid US names, comparing every pair across about 1.7 million combinations using two-way Engle-Granger tests, walk-forward hedge ratios, false-discovery controls, and dollar-volume capacity checks.

**「Solution」** Before shipping, the author reran the accept/reject decision inside each test year so nothing could know the year it was judged on, and the apparent edge vanished: accepted pairs stopped beating correlation-matched rejects, no column predicted the year ahead, and pairs that the full-sample run approved were winners only because that run already knew the future—by 13.9 points a year. Synthetic controls showed why: a relationship that reverted for years and then died still gets accepted 78–88% of the time, because a decade of history can outvote a recent regime change. The cointegration test finds relationships that existed, not ones that still do. What survived honest measurement was more structural: same-industry pairs cleared every null with a 2.3–2.8x lift versus roughly 1.0 for unrelated names, median capacity was about $2.7 million at 5% of ADV, and the accepted list turned over only 3.3% weekly. The author stripped backtest scores out of the register entirely, so users cannot rank by them, and defaults to acceptance strength and today&\#x27;s z-score.

**「Takeaway」** The article&\#x27;s central lesson is that statistical cointegration tests certify historical relationships, not live ones, and any screener using full-sample decisions can hide a hindsight edge. Robust screens need honest out-of-sample decision boundaries, and durable signals may be more structural—industry membership and capacity—than the raw spread score.

**Tags**: `#pairs trading`, `#cointegration`, `#lookahead bias`, `#backtesting`, `#quantitative finance`

---

<a id="item-tech-blog-2"></a>
### [Regime-Robust Bayesian Optimisation for Tabular Trading Signal Generation](https://arxiv.org/abs/2608.27076) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Aug 28, 04:00

**「Background」** Algorithmic trading is now a market exceeding $20 billion, where even small gains in signal robustness are economically significant, yet existing evaluations of equity prediction models do not explicitly target regime robustness during hyperparameter selection.

**「Solution」** The author trained five model classes on daily observations from roughly 300 large-cap US equities over eleven years, using Bayesian optimisation configured to target trading performance across three statistically different market regimes. This regime-robust hyperparameter selection was associated with out-of-sample generalisation: signal precision stayed above the random baseline across all four quarters of the test period, and portfolio performance degraded slowly under simulated input noise before collapsing beyond a defined threshold. No individual tabular deep learning architecture outperformed gradient-boosted trees, but combining XGBoost and TabNet using rank aggregation produced a Hybrid ensemble with an annualised return of 51.26%, a Sharpe ratio of 2.44, and a statistically significant CAPM alpha of 0.423 \(p = 0.011\). A near-zero beta indicated the outperformance was driven by stock selection, not market exposure. Alternative data played a secondary role once technical and fundamental features were accounted for, contributing more strongly on the short side than the long and varying by model class. An interactive application makes these results explorable in real time, with live data integration the remaining step toward practical deployment.

**「Takeaway」** The author concludes that explicitly optimising for regime robustness during hyperparameter selection, combined with a hybrid XGBoost-TabNet ensemble, yields strong out-of-sample equity signal performance driven by stock selection rather than market exposure.

**Tags**: `#algorithmic trading`, `#tabular deep learning`, `#Bayesian optimization`, `#ensemble models`, `#regime robustness`

---

<a id="item-tech-blog-3"></a>
### [Tail-Weighted Maximal Deficit and Optimal Reserve Allocation](https://arxiv.org/abs/2605.16448) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Aug 28, 04:00

**「Background」** Allocating a reserve budget among units requires measuring the largest cumulative loss over the horizon, since interim peaks can be more damaging than final losses. To capture such tail-weighted extremes, the authors introduce monetary risk measures built from a distortion function applied to the survivor function of the maximum cumulative loss.

**「Solution」** For a cumulative net-loss process L\_s and its supremum M\_t, the authors define D\_g^\{\(t\)\}\(u\) = ∫\_u^∞ g\(P\(M\_t&gt;v\)\) dv, where a concave distortion g emphasizes tail losses. They derive three monetary risk measures: the value at zero reserve, and measures based on fixed and proportional deficit tolerances. Under a concave distortion, the zero-reserve and proportional-tolerance measures are coherent, while the fixed-tolerance measure is convex. With a reserve budget split among units, they analyze two allocation criteria: the sum of unit-level distorted deficits, depending only on marginal distributions, and a distorted expectation of the largest residual unit deficit, which uses joint dependence. They characterize optimal and near-optimal allocations, show with a two-unit exponential benchmark that the optimum can be unique and unequal, and apply both criteria to the Building, Contents, and loss-of-Profits components of Danish large-fire data, finding interior allocations and localized 0.5%-optimal regions. Sensitivity analyses illustrate model uncertainty, and the authors also provide Monte Carlo estimators, conditional counterparts, and a review-date allocation formulation.

**「Takeaway」** The authors argue that distortion-based tail-deficit measures offer a flexible and theoretically grounded way to set reserve allocations, balancing tail sensitivity with dependence among units.

**Tags**: `#risk measures`, `#reserve allocation`, `#distortion functions`, `#Monte Carlo estimation`, `#insurance analytics`

---

<a id="item-tech-blog-4"></a>
### [Scalable Adjoint-Guided Recovery for Constrained Dynamic Portfolio Choice](https://arxiv.org/abs/2608.15667) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Aug 28, 04:00

**「Background」** Continuous-time multi-asset portfolio choice and consumption under smooth pointwise constraints—including state-dependent feasible sets—is computationally challenging, and finite-budget direct policy optimization leaves residual Pontryagin/KKT errors. The author&\#x27;s approach separates dynamic information acquisition from local constrained recovery.

**「Solution」** A pointwise-feasible neural actor generates reference rollouts; after training, its latent outputs are frozen and first- and second-order adjoints are harvested from a fixed-latent open-loop backpropagation-through-time graph. This lets feedback produce the reference path without restricting the adjoint formulation to Markov controls. At deployment, the harvested adjoints define a local generalized Pontryagin-Hamiltonian problem: quadratic-affine portfolio blocks are recovered exactly by a quadratic program, while a log barrier approximates more general regular KKT branches. The author provides local chart representations, an OL-BPTT-to-adjoint correspondence with orthogonal martingale residuals, and an end-to-end error bound, then validates the adjoints on analytical benchmarks and shows that recovery reduces residual PMP/KKT error under a state-dependent consumption cap and with up to 100 risky assets.

**「Takeaway」** The author&\#x27;s core thesis is that separating neural reference generation from adjoint-based local recovery makes constrained dynamic portfolio choice scalable—limiting complexity to the constrained action block—and that this recovery can sharpen optimality-condition fidelity beyond direct policy optimization.

**Tags**: `#portfolio optimization`, `#adjoint methods`, `#neural networks`, `#Pontryagin&\#x27;s principle`, `#constrained optimization`

---

<a id="item-tech-blog-5"></a>
### [Interpretable hybrid credit scoring with fairness audit for thin-file borrowers](https://arxiv.org/abs/2608.26837) ⭐️ 7.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Aug 28, 04:00

**「Background」** Credit scoring for thin-file and underbanked populations forces a trade-off: opaque machine learning can improve accuracy, but regulators and borrowers need explanations, while simpler scorecards are interpretable yet weaker. The authors extend a residual-learning hybrid approach that aims to offer both.

**「Solution」** Their framework pairs a logistic-regression scorecard with a gradient-boosting correction on its residuals, then decomposes each prediction into an interpretability ratio ρ\(x\) measuring how much is attributable to the linear branch. They instantiate it on the Zindi Financial Inclusion in Africa dataset \(Kenya, Rwanda, Tanzania, Uganda\), implement a fairness audit across the framework&\#x27;s three interpretability regions, and conduct a thin-file segmentation analysis. On the Taiwan Credit Default benchmark, the calibrated hybrid reaches AUC 0.776 \(+0.057 vs. standalone logistic regression, +0.001 vs. XGBoost\), cuts Brier Score by 23%, and places 69.5% of the highest-default-rate borrowers in the fully interpretable region. On Zindi, it reaches AUC 0.869 \(+0.015 vs. logistic regression, p &lt; 0.001\), reduces Brier from 0.158 to 0.085 \(a 46% reduction\), and replicates the regional routing pattern. The fairness audit detects severe routing into the opaque ML-driven region along socioeconomic lines—rural respondents 18 percentage points more than urban, primary-or-less-educated 32 points more than secondary-and-above, Ugandans 22 points more than Kenyans—while gender shows essentially no disparity. The authors argue this audit pipeline surfaces subgroup-routing violations that aggregate fairness metrics miss, in a form usable by African central-bank supervisors of digital credit.

**「Takeaway」** The authors conclude that an interpretable hybrid can match or exceed standalone ML accuracy while making fairness disparities visible at the subgroup level. For thin-file and underbanked populations, this supports more accountable oversight of digital credit.

**Tags**: `#credit scoring`, `#interpretable ML`, `#fairness audit`, `#financial inclusion`, `#residual learning`

---

<a id="item-tech-blog-6"></a>
### [Reading the Labor Market Pulse from 750M Chinese Job Ads](https://arxiv.org/abs/2608.26924) ⭐️ 7.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Aug 28, 04:00

**「Background」** The author argues that defining an occupation by its job title is misleading: the same title at different firms can demand different credentials and involve different work. Official directories like O\*NET offer only one national average per occupation, updated every few years, while job postings are timely but unstructured. Existing research built on postings tends to blur what is asked of a candidate into what a candidate is asked to do.

**「Solution」** To separate requirements from tasks, the authors analyze 752.6 million job ads posted on China&\#x27;s five leading recruitment platforms between 2022 and 2026. They extract the phrases employers write, unify those that name the same thing, and validate the mapping from text back to entry. This yields two catalogs: 20,721 requirements a candidate must meet and 44,479 tasks the hire will do. Each task also receives a score for how far a language model could absorb it. Matching the catalogs back onto every ad lets the authors read the labor market month by month. Two examples show the value of this layer beneath the job title: official registries record one accountant, but ads reveal a staircase from junior to intermediate certificates; and counting occupations suggests the work most exposed to language models is disappearing, while counting tasks shows far less of it is.

**「Takeaway」** The authors conclude that separating occupational requirements from tasks reveals a much finer and more current pulse of the labor market than official directories, and that the distinction changes substantive conclusions about labor market shifts.

**Tags**: `#labor market analysis`, `#NLP`, `#job postings`, `#occupational classification`, `#text mining`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Nvidia, Salesforce, Okta jump on earnings beats in midday stock moves](https://www.cnbc.com/2026/08/27/stocks-making-the-biggest-moves-midday-nvda-okta-hrl-veev.html) ⭐️ 8.0/10

Nvidia, Salesforce, and Okta led midday gains after their quarterly results beat expectations: Nvidia jumped 9% on adjusted earnings of $2.22 per share and revenue of $96.22 billion, ahead of analyst estimates, and forecast third-quarter revenue of $108 billion.

rss · CNBC Finance · Aug 27, 20:09

**「Background」** The moves came as several companies reported quarterly earnings and updated forecasts; investors also reacted to analyst downgrades, margin warnings, and a Reuters report that Trian Fund Management would not bid for Wendy&\#x27;s.

**Tags**: `#earnings`, `#stock movers`, `#technology`, `#retail`, `#guidance`

---

<a id="item-finance-news-2"></a>
### [Salesforce stock jumps 20% after earnings, lifting software sector](https://www.marketwatch.com/story/salesforce-stock-is-jumping-what-wall-street-is-saying-about-its-earnings-and-its-anthropic-relationship-853ada85?mod=mw_rss_topstories) ⭐️ 8.0/10

Salesforce shares rose about 20% after its earnings report, giving the software sector a major lift and signaling that AI is not displacing traditional software vendors.

rss · MarketWatch Top Stories · Aug 27, 22:51

**「Background」** Salesforce reported strong fiscal second-quarter results and announced an AI partnership with Anthropic, launching &quot;Claudeforce.&quot; The news helped calm investor fears that AI adoption would hurt traditional software companies, a concern that had weighed on the sector.

**「Impact」** The rally helped boost software stocks broadly, as investors took the results as evidence that legacy software companies can thrive alongside AI and may partner with major AI model operators.

<details><summary>References</summary>
<ul>
<li><a href="https://cryptobriefing.com/salesforce-stock-earnings-anthropic-partnership/">Salesforce stock jumps 10% premarket on earnings and Anthropic ...</a></li>
<li><a href="https://finance.yahoo.com/markets/live/stock-market-today-thursday-august-27-dow-sp-500-nasdaq-082144520.html">Stock market today: Dow, S&amp;P 500, Nasdaq futures rise as Nvidia...</a></li>

</ul>
</details>

**Tags**: `#Salesforce`, `#earnings`, `#software sector`, `#AI partnership`, `#stock surge`

---

<a id="item-finance-news-3"></a>
### [Nvidia shares rise 8% after earnings beat, boosting tech stocks and bitcoin](https://www.coindesk.com/markets/2026/08/27/nvidia-shares-surge-8-on-earnings-beat-lifting-technology-stocks-and-bitcoin) ⭐️ 8.0/10

Nvidia reported an earnings beat, sending its shares up 8% and helping lift technology stocks and bitcoin, according to CoinDesk.

rss · CoinDesk · Aug 27, 09:19

**「Background」** Nvidia, the leading AI-chip maker, reported quarterly earnings that beat Wall Street estimates and gave a strong outlook, prompting an 8% share gain. The company has beaten consensus earnings estimates in 22 of the past quarters, according to The Motley Fool, and its results are widely watched as a bellwether for AI-related technology stocks.

**「Market impact」** Nvidia’s earnings beat helped lift technology stocks, bitcoin and AI infrastructure companies, with the tech-heavy Nasdaq Composite rising 1.6%, the S&amp;P 500 0.7% and the Dow 0.2% on the day, according to Investopedia.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coindesk.com/markets/2026/08/27/nvidia-shares-surge-8-on-earnings-beat-lifting-technology-stocks-and-bitcoin">Nvidia shares surge 8% on earnings beat, lifting technology ...</a></li>
<li><a href="https://www.fool.com/investing/2026/08/25/nvda-stock-earnings-q2-date-aug-26/">Nvidia Earnings on August 26: What History Tells Us About ...</a></li>
<li><a href="https://www.coindesk.com/markets/2026/08/27/nvidia-shares-surge-8-on-earnings-beat-lifting-technology-stocks-and-bitcoin">Nvidia earnings beat lifts markets as chipmaker reportedly agrees $12.9 billion deal</a></li>
<li><a href="https://www.investopedia.com/stock-market-today-dow-jones-s-and-p-500-08272026-12069234">Markets News, Aug. 27, 2026: Nvidia Stock Powers Higher After Earnings, Driving Tech Gains; Nasdaq Closes Sharply Higher</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#earnings`, `#technology stocks`, `#bitcoin`, `#market impact`

---

<a id="item-finance-news-4"></a>
### [Fed&\#x27;s Schmid: Inflation sticky, policy rate may not be restrictive](https://www.cnbc.com/2026/08/27/kansas-city-feds-schmid-says-inflation-stubborn-and-sticky-policy-rate-not-restrictive.html) ⭐️ 7.0/10

Kansas City Fed President Jeffrey Schmid said at Jackson Hole that inflation remains &\#x27;stubborn&\#x27; and &\#x27;sticky&\#x27; and that the Fed&\#x27;s current policy rate target of 3.5%-3.75% may not be restrictive, citing core inflation at 3.3% against the Fed&\#x27;s 2% target. He stopped short of calling for an interest rate hike and said he wants more information.

rss · CNBC Finance · Aug 27, 14:11

**「Background」** The FOMC, the Federal Reserve&\#x27;s rate-setting committee, currently holds its policy rate in that range; Schmid is not a voting member this year.

**Tags**: `#Federal Reserve`, `#inflation`, `#monetary policy`, `#interest rates`, `#Jackson Hole`

---

<a id="item-finance-news-5"></a>
### [Premarket stock movers: Nvidia and Salesforce surge after earnings, HP drops](https://www.cnbc.com/2026/08/27/stocks-making-the-biggest-moves-premarket-nvda-hp-crm-dg-p.html) ⭐️ 7.0/10

Several major companies moved sharply in premarket trading after reporting quarterly results: Nvidia rose over 7% after second-quarter revenue more than doubled to $96.22 billion, beating the $92.17 billion consensus, and Salesforce jumped nearly 12% after adjusted earnings of $5.90 per share beat the $3.27 estimate. Dollar General added 12% after raising full-year profit guidance to $7.80-$8.00 per share, while HP fell nearly 11% despite beating fiscal third-quarter estimates.

rss · CNBC Finance · Aug 27, 14:45

**「Background」** Most of the moves follow earnings reports released after the previous close, with consensus figures from LSEG as the benchmark for analyst expectations.

**Tags**: `#premarket`, `#earnings`, `#Nvidia`, `#Salesforce`, `#guidance`

---

<a id="item-finance-news-6"></a>
### [Judge: Trump administration&\#x27;s blacklist of Anthropic violated First Amendment](https://www.marketwatch.com/story/judge-says-trump-administrations-blacklist-of-anthropic-was-illegal-5d3411e7?mod=mw_rss_topstories) ⭐️ 7.0/10

A federal judge ruled late Thursday that the Trump administration&\#x27;s blacklisting of Anthropic earlier this year was illegal, saying it violated the AI company&\#x27;s First Amendment rights.

rss · MarketWatch Top Stories · Aug 28, 03:16

**「Background」** Anthropic, the maker of the Claude AI models, was blacklisted by the Trump administration earlier this year and designated a national security risk. A federal judge ruled Thursday that the blacklist and related ban violated Anthropic&\#x27;s First Amendment rights and denied due process, after previously pausing the designation in March.

<details><summary>References</summary>
<ul>
<li><a href="https://www.politico.com/news/2026/08/27/judge-rules-trump-administrations-anthropic-blacklisting-is-illegal-01053855">Judge rules Trump administration ’s Anthropic blacklisting is illegal</a></li>
<li><a href="https://www.kucoin.com/news/flash/federal-judge-blocks-trump-s-anthropic-blacklist-and-ban">Federal Judge Blocks Trump &#x27;s Anthropic Blacklist and Ban | KuCoin</a></li>
<li><a href="https://www.nytimes.com/2026/08/27/technology/anthropic-government-blacklisting-ruling.html">Trump Administration ’s Blacklisting of Anthropic Was Illegal...</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#AI regulation`, `#First Amendment`, `#court ruling`, `#tech policy`

---

<a id="item-finance-news-7"></a>
### [Mirae Asset Acquires Digital X, Targets $109B Crypto Business](https://www.coindesk.com/business/2026/08/27/mirae-asset-eyes-usd109-billion-crypto-empire-after-acquiring-digital-x) ⭐️ 7.0/10

Mirae Asset, a large South Korean financial group, is acquiring crypto firm Digital X and aims to build a $109 billion cryptocurrency asset-management business, according to the report.

rss · CoinDesk · Aug 27, 11:37

**「Background」** Mirae Asset Financial Group, a South Korean financial giant, completed its acquisition of a 97% stake in the cryptocurrency exchange Korbit in July and renamed its operator Digital X. The group now plans to build a 150 trillion won \($109 billion\) digital asset business around Digital X, aiming for profitability by 2027.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coindesk.com/business/2026/08/27/mirae-asset-eyes-usd109-billion-crypto-empire-after-acquiring-digital-x">Mirae Asset founder unveils $109 billion vision for former Korbit exchange</a></li>
<li><a href="https://www.theblock.co/news/business/2026-08-27-mirae-asset-109-billion-digital-asset-push-412883">Mirae Asset maps out $109 billion digital asset push with Digital X: report | The Block</a></li>
<li><a href="https://www.hokanews.com/2026/08/mirae-asset-targets-150-trillion-won.html">Mirae Asset Targets 150 Trillion Won Digital Asset Business Through Digital X - Hokanews</a></li>

</ul>
</details>

**Tags**: `#Mirae Asset`, `#Digital X`, `#acquisition`, `#cryptocurrency`, `#asset management`

---

<a id="item-finance-news-8"></a>
### [Solana Governance Vote Advances Faster Supply Cuts; Daily Burn Plan Trails](https://www.coindesk.com/tech/2026/08/28/solana-s-faster-supply-cuts-lead-vote-while-usd800-000-daily-burn-plan-trails) ⭐️ 6.0/10

Solana&\#x27;s governance vote is advancing a proposal that would speed up reductions in token supply, while a separate plan to burn about $800,000 worth of SOL per day is trailing in support. The proposal&\#x27;s outcome is still pending a vote.

rss · CoinDesk · Aug 28, 06:22

**「Background」** Solana holders are voting on governance proposals to reduce new SOL creation and burn more tokens. All three proposals have cleared quorum, but the plan to slow new SOL issuance is only narrowly passing while a separate daily burn plan trails.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coindesk.com/tech/2026/08/28/solana-s-faster-supply-cuts-lead-vote-while-usd800-000-daily-burn-plan-trails">SOL news: Solana’s faster supply cuts lead vote while ...</a></li>

</ul>
</details>

**Tags**: `#Solana`, `#Cryptocurrency`, `#Governance`, `#Token Burn`, `#Inflation`

---