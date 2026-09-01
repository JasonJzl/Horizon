---
layout: default
title: "Horizon Summary: 2026-09-01 (EN)"
date: 2026-09-01
lang: en
---

> From 81 items, 20 important content pieces were selected

---

**Technology News**
1. [Google Removes MV2 Extensions, Including uBlock Origin](#item-tech-news-1) ⭐️ 8.0/10
2. [ChatGPT Work Tool Reference Highlights Playwright Browser Skill](#item-tech-news-2) ⭐️ 7.0/10
3. [Wrapture: Python library combines monkeypatching, testing, and tracing](#item-tech-news-3) ⭐️ 7.0/10
4. [Turning Security Cameras Into an Automatic Bird Identification System](#item-tech-news-4) ⭐️ 6.0/10
5. [Walkable ASCII Cyberpunk City in One HTML File](#item-tech-news-5) ⭐️ 6.0/10
6. [RavynOS: Pre-alpha Open-Source macOS-like OS on FreeBSD](#item-tech-news-6) ⭐️ 6.0/10

**Technology Blog**
1. [Rough Bergomi Calibration for Bitcoin Inverse Options](#item-tech-blog-1) ⭐️ 8.0/10
2. [Leakage-safe evaluation of LLM trading strategy discovery](#item-tech-blog-2) ⭐️ 8.0/10
3. [Heston SLV Valuation of GMMB Riders with Surrender Shows Marginals Do Not Tame Model Risk](#item-tech-blog-3) ⭐️ 8.0/10
4. [Dual-Class Shares: Dynamic Valuation and Innovation Trade-Offs](#item-tech-blog-4) ⭐️ 8.0/10
5. [Internet-Use Frequency as a Marker of Labor-Market Stratification](#item-tech-blog-5) ⭐️ 7.0/10
6. [Customer Disclosures Shape Supplier Capital Allocation](#item-tech-blog-6) ⭐️ 6.0/10

**Financial News**
1. [Aon to buy USI Insurance Services for $17 billion to build middle-market platform](#item-finance-news-1) ⭐️ 8.0/10
2. [Warsh&\#x27;s Hawkish Jackson Hole Speech Boosts September Rate Hike Chances](#item-finance-news-2) ⭐️ 8.0/10
3. [Amazon Stock Slips as FTC Alleges Hidden Ad Fees](#item-finance-news-3) ⭐️ 8.0/10
4. [Cronos halts network after estimated $75M Tectonic exploit](#item-finance-news-4) ⭐️ 8.0/10
5. [California wildfire-liability vote hits PG&amp;E and Edison; Aon to buy USI for $17B](#item-finance-news-5) ⭐️ 7.0/10
6. [PG&amp;E drops 16% after California blocks wildfire-liability cap; Aon slips on $17B deal](#item-finance-news-6) ⭐️ 7.0/10
7. [Bitmine now holds 4.9% of Ethereum supply after 65-week buying streak](#item-finance-news-7) ⭐️ 7.0/10
8. [North Korean hackers reported moving tens of millions on Hyperliquid as Trump urges onshoring](#item-finance-news-8) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Google Removes MV2 Extensions, Including uBlock Origin](https://webiterate.dev/google-removed-extensions-ublock-origin-108/) ⭐️ 8.0/10

Google has removed Manifest V2 extensions from the Chrome Web Store, including uBlock Origin, according to webiterate.dev. The removal represents the latest step in Chrome&\#x27;s transition to Manifest V3, which introduces more restrictive extension APIs. Users who relied on uBlock Origin in Chrome can no longer find the extension in the store, prompting community backlash and renewed calls to switch to browsers like Firefox. The change highlights ongoing tensions over Google&\#x27;s control over browser extension infrastructure and ad-blocking capabilities.

hackernews · twapi · Aug 31, 21:10 · [Discussion](https://news.ycombinator.com/item?id=49514878)

**「Background」** Google is phasing out Manifest V2 \(MV2\) extensions in favor of Manifest V3 \(MV3\), a new extension framework that changes how extensions handle permissions and network requests. As part of this transition, Google has begun removing MV2 extensions from the Chrome Web Store and will disable them in Chrome, with uBlock Origin being a prominent casualty. Chrome has also removed the featured badge from MV2 apps, and while temporary workarounds exist to re-enable uBlock Origin until June 2025, the long-term solution is for users to switch to alternative browsers or extensions.

**「Impact」** Chrome users who depended on uBlock Origin and other Manifest V2 extensions are directly affected because they can no longer install these tools from the Chrome Web Store. Community members indicate that Firefox remains a practical alternative for users seeking full-featured ad blocking, though that is not affected by Chrome&\#x27;s decision.

**「Community Discussion」** Commenters expressed frustration, describing ad blocking as a safety issue for vulnerable users and criticizing Google&\#x27;s unilateral control over the web. Several recounted moving to Firefox and recommending it to others, noting that uBlock Origin has always worked best on Firefox.

<details><summary>References</summary>
<ul>
<li><a href="https://www.newsbytesapp.com/news/science/google-chrome-to-disable-ublock-origin-other-extensions/story">Your favorite Chrome extensions might disappear soon</a></li>
<li><a href="https://www.ghostery.com/blog/ublock-origin-not-supported-chrome">uBlock Origin No Longer Supported On Chrome : Best Fixes | Ghostery</a></li>

</ul>
</details>

**Tags**: `#chrome`, `#web-extensions`, `#manifest-v3`, `#ad-blocking`, `#firefox`

---

<a id="item-tech-news-2"></a>
### [ChatGPT Work Tool Reference Highlights Playwright Browser Skill](https://codex-tool-reference.simonw.chatgpt.site/) ⭐️ 7.0/10

A community-built reference site catalogues ChatGPT Work tools and skills, most notably a browser-control skill that instructs ChatGPT Work to launch Playwright through its Node.js REPL and run \`nodeRepl.write\(await browser.documentation\(\)\);\` to get the detailed browser usage guide. The resource gives developers a practical pattern for automating web interactions with ChatGPT Work, but it is a documentation collection rather than a new product or breakthrough. Community reaction highlights tradeoffs: some Work skills can slow workflows and consume many tokens, and one commenter questions how this differs from Codex, which can already perform similar tasks.

hackernews · ijidak · Aug 31, 14:07 · [Discussion](https://news.ycombinator.com/item?id=49510000)

**「Background」** ChatGPT Work is OpenAI&\#x27;s agentic work assistant within ChatGPT, capable of executing coding and browser tasks. Skills are a relatively new ChatGPT/Codex feature: reusable workflow packages containing a name and description, step-by-step instructions usually in a SKILL.md file, and supporting resources. The reference site documents these skills; its standout browser-control skill tells ChatGPT Work to launch a Playwright instance via its Node.js REPL and run \`nodeRepl.write\(await browser.documentation\(\)\);\` to obtain usage instructions.

**「Impact」** For developers exploring ChatGPT Work automation, the Playwright-based browser skill provides a ready-made pattern for controlling a real browser, though community reports indicate some Work tools add latency and token consumption.

**「Community Discussion」** One commenter highlighted the control-browser skill as the most interesting entry and pointed to a separate comment for background and creation prompt; others noted that some work tools can slow things down and waste tokens, or questioned how this differs from Codex. A separate meta-comment observed that AI-generated websites and artifacts tend to share a similar visual style, reminiscent of the Bootstrap era.

<details><summary>References</summary>
<ul>
<li><a href="https://academy.openai.com/public/clubs/work-users-ynjqu/resources/skills">Skills - Resource | OpenAI Academy</a></li>
<li><a href="https://openai.com/academy/skills/">Using skills | OpenAI</a></li>

</ul>
</details>

**Tags**: `#ChatGPT Work`, `#browser automation`, `#AI tooling`, `#reference`

---

<a id="item-tech-news-3"></a>
### [Wrapture: Python library combines monkeypatching, testing, and tracing](https://simonwillison.net/2026/Aug/31/introducing-wrapture/) ⭐️ 7.0/10

Wrapture is a new Python library from Graham Dumpleton, the creator of wrapt, mod\_wsgi, and New Relic&\#x27;s Python agent, extending wrapt-style monkeypatching to serve both testing and tracing. It can wrap any function or method so all access is traced or overridden to return a different value, acting as an alternative to unittest.mock and a way to trace existing projects. Wrapture includes OpenTelemetry support and a configuration-based TOML mechanism, e.g. a capture target \`domain:Calculator\` and a JSON-lines sink \`trace.jsonl\`. Dumpleton says the project is just a few weeks old and was his first large entirely agent-driven project: every line of code and documentation was written by an AI assistant under his direction, which he distinguishes from vibe coding. A follow-up post demonstrates testing patterns such as \`binding\(...\).on\_call.returns\(...\)\` stubbing and \`on\_call.transforms\_result\(...\)\` to modify an original method&\#x27;s return value.

rss · Simon Willison · Aug 31, 23:59

**「Background」** Monkeypatching allows a program to modify functions or methods at runtime, and wrapt is a popular Python library by Graham Dumpleton for doing this transparently. Wrapture builds on the same ideas to provide a unified mechanism for observing and overriding behavior in both test and production contexts.

**「Impact」** With Wrapture&\#x27;s configuration-based sinks, developers can instrument an existing Python project without code changes, and the context-manager bindings give tests a way to stub or transform return values as an alternative to unittest.mock.

**Tags**: `#Python`, `#testing`, `#tracing`, `#monkeypatching`, `#open source`

---

<a id="item-tech-news-4"></a>
### [Turning Security Cameras Into an Automatic Bird Identification System](https://jasontucker.blog/how-i-turned-my-security-cameras-into-an-automatic-bird-identification-system-with-birdnet-go/) ⭐️ 6.0/10

A hobbyist described using existing security cameras with BirdNET-Go to automatically detect and identify birds by sound, turning a typical surveillance setup into a nature-monitoring tool. BirdNET-Go analyzes audio captured from RTSP camera feeds, and the project attracted interest from others who had built similar systems. Commenters shared variations, including using a Unifi doorbell camera&\#x27;s RTSP feed, a portable Birdnet-Pi with an e-ink display, and a Raspberry Pi with an external microphone. One caveat noted that some cameras only support 16 kHz audio, while BirdNET expects 48 kHz samples, and wind noise can degrade results. The broader takeaway is that repurposing existing camera hardware can make bird identification accessible, but audio quality and sample-rate support are important constraints.

hackernews · speckx · Aug 31, 16:47 · [Discussion](https://news.ycombinator.com/item?id=49511856)

**「Background」** BirdNET-Go is a self-hosted, real-time soundscape analyzer that runs 24/7 on a Raspberry Pi, ingesting audio from soundcards or network streams and using local AI inference to identify birds, bats, and wildlife with a web UI for detections. This project builds on Cornell University&\#x27;s BirdNET species identification model, which has also become popular through the Merlin Bird ID app, and combines it with security cameras&\#x27; RTSP audio feeds so the system can automatically listen for and classify bird calls. The approach typically involves configuring camera audio streams for BirdNET-Go, though some users note limitations such as low sampling rates or wind noise in built-in camera microphones.

**「Impact」** Hobbyists with RTSP-capable security cameras can use BirdNET-Go to identify birds without additional dedicated hardware, though they may need to add an external microphone or choose cameras with 48 kHz audio support to get reliable results.

**「Community Discussion」** Several commenters shared successful implementations, such as a Unifi doorbell camera setup, a portable Birdnet-Pi with an e-ink display, and a Raspberry Pi with an external microphone. They also flagged practical issues like wind noise and 16 kHz sample-rate limits on some cameras, and one commenter recommended the Merlin Bird ID app as an alternative.

<details><summary>References</summary>
<ul>
<li><a href="https://jasontucker.blog/how-i-turned-my-security-cameras-into-an-automatic-bird-identification-system-with-birdnet-go/">How I Turned My Security Cameras Into an Automatic Bird Identification System with BirdNet-Go</a></li>
<li><a href="https://github.com/tphakala/birdnet-go">GitHub - tphakala/birdnet-go: Self-hosted realtime soundscape analyser for birds, bats and other wildlife. Multi-model local AI inference, runs 24/7 on a Raspberry Pi. · GitHub</a></li>
<li><a href="https://www.kyleniewiada.org/blog/2025/05/backyard-bird-tracking-with-ai/">Backyard Bird Tracking With AI-Powered BirdNET-Go</a></li>

</ul>
</details>

**Tags**: `#bird identification`, `#BirdNET`, `#security cameras`, `#machine learning`, `#DIY`

---

<a id="item-tech-news-5"></a>
### [Walkable ASCII Cyberpunk City in One HTML File](https://www.youtube.com/watch?v=3YtygAx_C6A) ⭐️ 6.0/10

A video shared on Hacker News by keithcarolus demonstrates a walkable ASCII cyberpunk city rendered entirely in a single HTML file, with follow-up videos showing added traffic, detail, interiors, elevation, and skyscrapers. Commenters praised the &\#x27;mood&\#x27; of the project and recommended browser-based fixed-width character art for predictable font and proportion rendering and better tooling than terminals. One viewer reported that running it locally did not look like the uploaded video and was hard to read, while another questioned whether the linked GitHub project matches the videos. The post does not include the HTML file itself, installation instructions, or performance details.

hackernews · keithcarolus · Aug 31, 18:21 · [Discussion](https://news.ycombinator.com/item?id=49512975)

**「Background」** ASCII art is a technique for creating images using fixed-width text characters, and some developers extend this approach to animated or interactive scenes by rendering characters in a web browser. The showcased project is a small custom engine built with JavaScript and Canvas that renders a grid-based city—complete with roads, buildings, trees, cars, and pedestrians—entirely from ASCII characters in a single HTML file, without using game engines, 3D models, textures, or shaders.

**「Community Discussion」** Commenters generally appreciated the technique and aesthetic, with aleyan recommending browser-based ASCII and Unicode art for easier rendering control and FpUser calling it moody. Practical concerns included naet&\#x27;s local rendering mismatch and jeffgreco&\#x27;s uncertainty about whether the GitHub project matches the videos, while SpyCoder77 flagged the post as a duplicate.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49512975">A walkable ASCII cyberpunk city in one HTML file... | Hacker News</a></li>

</ul>
</details>

**Tags**: `#ASCII art`, `#HTML`, `#creative coding`, `#cyberpunk`, `#web development`

---

<a id="item-tech-news-6"></a>
### [RavynOS: Pre-alpha Open-Source macOS-like OS on FreeBSD](https://ravynos.com/) ⭐️ 6.0/10

RavynOS is a pre-alpha open-source operating system built on Darwin and FreeBSD that aims to deliver a macOS-like desktop experience with some compatibility with macOS applications. The project is still in early development, so it is not yet production-ready or suitable as a stable daily driver. It follows in the footsteps of compatibility-focused open-source projects such as ReactOS, GNUstep, and Darling, which seek to reimplement or provide compatibility layers for established operating systems. The project has attracted repeated attention on Hacker News, with discussions dating back to 2022, indicating moderate but ongoing community interest. As a pre-alpha effort, its focus is on exploring the feasibility of a BSD-based, macOS-inspired operating system rather than providing a complete alternative to macOS.

hackernews · Bluestein · Aug 31, 16:19 · [Discussion](https://news.ycombinator.com/item?id=49511534)

**「Background」** RavynOS is an early-stage pre-alpha open-source operating system built from Darwin \(the open-source core of Apple&\#x27;s macOS\), FreeBSD, and Apple&\#x27;s released open-source code, aiming to provide a macOS-like user experience and eventual compatibility with macOS applications while also supporting FreeBSD and Linux binaries. Darwin itself is based on BSD Unix components and the Mach microkernel, but macOS&\#x27;s proprietary GUI frameworks are not open-source, so projects like RavynOS rely on open implementations such as GNUstep. The project has been discussed repeatedly on Hacker News and covered by outlets like Hackaday, with recent release &quot;Hyperpop Hyena&quot; \(0.6.1\) available for download.

**「Community Discussion」** Commenters questioned what practical advantages Darwin offers beyond the potential to run macOS applications, and some noted that the website lacks a screenshot, making it harder to evaluate the project. Others cited the FAQ comparing RavynOS to ReactOS, GNUstep, and Darling to address legal concerns, while one user complained about the project using Discord for communication due to server limits.

<details><summary>References</summary>
<ul>
<li><a href="https://ravynos.com/">ravynOS - Finesse of macOS. Freedom of Open Source.</a></li>
<li><a href="https://hackaday.com/2025/11/22/ravynos-open-source-macos-with-same-bsd-pedigree/">RavynOS: Open Source MacOS With Same BSD Pedigree | Hackaday</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#operating-systems`, `#FreeBSD`, `#Darwin`, `#macOS-compatibility`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Rough Bergomi Calibration for Bitcoin Inverse Options](https://arxiv.org/abs/2608.27575) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Aug 31, 04:00

**「Background」** Bitcoin inverse options traded on Deribit are settled in cryptocurrency rather than fiat, giving them a nonlinear payoff structure and interacting with Bitcoin&\#x27;s genuinely rough volatility dynamics. The author argues that standard pricing and calibration approaches are insufficient for these instruments, motivating a framework built on the rough Bergomi \(rBergomi\) model.

**「Solution」** The paper adapts rBergomi dynamics to the inverse payoff max\(S\_T - K, 0\)/S\_T and compares three computational pipelines that differ in how they simulate the driving fractional Brownian motion and in their Monte Carlo estimator. Using thirty implied volatility surfaces from Deribit trade data between May 2022 and March 2025, spanning seven market-stress events and nine baseline volatility regimes, the author calibrates the model with each pipeline. The Hybrid and Mixed pipeline is both the most accurate, with a mean unweighted RMSE of 22.83 percentage points versus 41.76 for the Cholesky and Euler benchmark, and the fastest, completing each snapshot in 17 seconds—a 20-fold speed-up. The calibrated Hurst exponent is consistently near the lower bound of the search space, around 0.01 to 0.06 in most regimes, which the author interprets as confirming that Bitcoin volatility is genuinely rough. Calibration error also scales approximately linearly with at-the-money implied volatility, with a Pearson correlation of 0.89.

**「Takeaway」** The author&\#x27;s evidence indicates that the rough Bergomi model, calibrated through a Hybrid and Mixed Monte Carlo pipeline, offers both accuracy and practical speed for Bitcoin inverse options while reinforcing the view that Bitcoin&\#x27;s volatility is genuinely rough, with calibration error tied closely to the prevailing level of implied volatility.

**Tags**: `#Bitcoin options`, `#Rough Bergomi`, `#Option pricing`, `#Calibration`, `#Monte Carlo simulation`

---

<a id="item-tech-blog-2"></a>
### [Leakage-safe evaluation of LLM trading strategy discovery](https://arxiv.org/abs/2608.27734) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Aug 31, 04:00

**「Background」** Large language models are increasingly used to discover trading strategies, yet much of this literature shares a methodological weakness: researchers generate many candidates, report the best, and then neglect both look-ahead bias and the search intensity behind the reported result. The author argues that standard practice needs structural correction, not just procedural fixes.

**「Solution」** The paper presents a strategy-discovery system in which both corrections are built into the architecture. The agent can only act through registry-validated tools whose feature space excludes look-ahead by construction, and the author shows this guardrail is not redundant with statistical correction: a deliberately leaky oracle posting a Sharpe ratio of 35 survives Deflated Sharpe and probability-of-backtest-overfitting testing completely. In addition, the system records every strategy evaluation its search performs and deflates all reported performance by that trial count, tracing how the best in-sample Sharpe ratio climbs with each trial while the deflation threshold, driven by the agent&\#x27;s own search, climbs faster. Across a 453-stock point-in-time US equity universe and a 39-ETF multi-asset universe with realistic transaction, impact, and borrow costs, honest evaluation certifies passive benchmarks with out-of-sample confidence intervals excluding zero and rejects every LLM-discovered strategy across two frontier models, search budgets up to one hundred candidates, and five repeated runs. The same instruments are applied to a human trader&\#x27;s production rule system, and the framework formalizes why pre-registered hypotheses earn lower evidential bars than brute search, quantifying the sample sizes needed for credible certification of moderate edges.

**「Takeaway」** The author concludes that honest evaluation of LLM-driven trading discovery requires structural guardrails and search-aware statistical deflation as complementary mechanisms, because even extreme leakage can survive conventional corrections. Without such built-in safeguards, reported LLM strategy performance is not trustworthy.

**Tags**: `#LLM`, `#trading strategies`, `#backtest overfitting`, `#evaluation methodology`, `#leakage`

---

<a id="item-tech-blog-3"></a>
### [Heston SLV Valuation of GMMB Riders with Surrender Shows Marginals Do Not Tame Model Risk](https://arxiv.org/abs/2608.28397) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Aug 31, 04:00

**「Background」** Valuing guaranteed minimum maturity benefit \(GMMB\) riders embedded in variable annuities requires modeling the fee-deducted account value, stochastic volatility, and policyholders&\#x27; rational surrender choices. Because one-factor local-volatility \(LV\) models struggle to capture conditional dynamics and surrender, the authors propose a market-informed Heston stochastic-local volatility \(SLV\) framework whose leverage function is calibrated so that SLV and LV share the same vanilla-implied marginals.

**「Solution」** The authors derive backward pricing equations for the Heston SLV model with a calibrated leverage function and propose a hybrid tree/finite-difference algorithm. In synthetic and market-informed tests, terminal-only guarantees yield numerically close SLV and LV values, consistent with the common marginal target. Once surrender is allowed, however, materially larger valuation differences emerge, affecting guarantee values, fair insurance fees, and volatility-dependent surrender regions. The article argues that matching one-date marginals implied by vanilla options does not eliminate model risk for insurance liabilities whose value depends on conditional continuation dynamics and endogenous surrender decisions.

**「Takeaway」** For quantitative insurance practitioners, the central lesson is that calibration to the same market surface can still leave large model risk in liabilities with optionality priced beyond terminal marginals. The authors show that a richer but still market-consistent SLV model materially changes GMMB values and surrender behavior.

**Tags**: `#quantitative finance`, `#insurance valuation`, `#stochastic-local volatility`, `#surrender option`, `#GMMB`

---

<a id="item-tech-blog-4"></a>
### [Dual-Class Shares: Dynamic Valuation and Innovation Trade-Offs](https://arxiv.org/abs/2608.25972) ⭐️ 8.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Aug 31, 04:00

**「Background」** Dual-class shares give founders control that can support valuable firm-specific investments, but they also separate control from ownership and create agency costs. Kim, Levit, and Michaely argue that this trade-off should be analyzed dynamically rather than as a static governance choice.

**「Solution」** Using new data on US dual-class firms spanning 52 years and difference-in-differences designs, the authors show that valuations rise after dual-class recapitalizations but decline over time, while innovative output increases persistently. The effects are concentrated in industries with greater firm-specific investments, and stock unifications show corresponding results. Mature dual-class firms have investment less sensitive to opportunities, and voting premia increase with maturity. These findings support dynamic treatment effects and yield new policy implications.

**「Takeaway」** The author&\#x27;s core conclusion is that the dual-class trade-off is time-varying: immediate valuation benefits erode while innovation gains persist, meaning governance evaluation and policy should account for dynamic effects and firm-specific investment intensity.

**Tags**: `#dual-class shares`, `#corporate governance`, `#difference-in-differences`, `#empirical finance`, `#innovation`

---

<a id="item-tech-blog-5"></a>
### [Internet-Use Frequency as a Marker of Labor-Market Stratification](https://arxiv.org/abs/2511.05294) ⭐️ 7.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Aug 31, 04:00

**「Background」** Surveys often ask how often people use the internet, but that simple frequency item is not the same as measuring the infrastructures, skills, and support systems that enable digital participation. The authors argue this distinction matters for studying inequality, because routine use may signal something deeper about economic status and labor-market attachment.

**「Solution」** Using the U.S. National Longitudinal Survey of Youth 1997 cohort, the authors compare internet-use frequency with labor income, employment attachment, and job seeking after 2010, focusing on comparable waves in 2011, 2013, and 2015 and using 2017 as later labor-market context. Across repeated cross sections, daily internet use consistently marks higher income and stronger employment attachment: relative to daily users, less-than-daily users earn roughly 11 to 20 percent less, while nonusers earn about 18 to 21 percent less in 2011 and 2013 and are 13 to 23 percentage points less likely to report full-year work. The job-search estimates show a distinct mechanism: active search is driven by employment status, search intensity, and application support, so a frequency item sorts respondents more sharply on durable labor-market attachment than on short-window search. Education explains a substantial share of the raw digital gradient, and pooled lagged-outcome and doubly robust transition estimates help separate durable stratification from positive adoption margins.

**「Takeaway」** The authors conclude that internet-use frequency is an informative behavioral marker of digitally mediated labor-market stratification, not a simple measure of digital access. This implies researchers and policymakers should treat routine use as a signal of economic attachment rather than equating it with connectivity.

**Tags**: `#digital divide`, `#internet use`, `#labor market`, `#income inequality`, `#job search`

---

<a id="item-tech-blog-6"></a>
### [Customer Disclosures Shape Supplier Capital Allocation](https://arxiv.org/abs/2608.27598) ⭐️ 6.0/10

rss · arXiv q-fin \(Quantitative Finance\) · Aug 31, 04:00

**「Background」** When firms disclose more about their major customers, suppliers should gain better visibility into downstream demand, but such disclosures can also erode a supplier&\#x27;s private information advantage. The author tests these competing possibilities by treating the adoption of SFAS 131 as an exogenous customer-disclosure shock.

**「Solution」** Drawing on segment data, the author traces how suppliers exposed to expanded customer disclosures reallocate capital. He finds that these suppliers face greater product-market competition and shift capital toward segments with relatively weak growth-opportunity signals, consistent with the competitive-threat channel rather than the information channel. Using a novel method that links supplier segments to customer segments, he shows that the reallocation reflects deliberate capacity investment in affected segments, not a correction of prior under-investment. The effect is stronger for segments dependent on larger customers and in more concentrated industries. Suppliers that deviate from growth-signal-based allocations are more likely to preserve market share and grow their customer base, yet the segments making these defensive investments subsequently report lower ROA.

**「Takeaway」** The author&\#x27;s evidence suggests that disclosures can shape how economically linked firms allocate capital internally, pushing suppliers to accept lower profitability to defend customer relationships. This highlights that disclosure mandates can have real, supply-chain-level consequences beyond their effects on investors.

**Tags**: `#customer disclosures`, `#capital allocation`, `#SFAS 131`, `#segment reporting`, `#competitive dynamics`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Aon to buy USI Insurance Services for $17 billion to build middle-market platform](https://www.cnbc.com/2026/08/31/aon-ceo-says-usi-deal-seeks-to-build-premiere-middle-market-insurance-platform.html) ⭐️ 8.0/10

Aon agreed to acquire rival insurance broker USI Insurance Services from private equity firm KKR for $17 billion, with the deal expected to close in the fourth quarter pending regulatory approvals. Aon says the purchase will create a leading U.S. middle-market insurance platform.

rss · CNBC Finance · Aug 31, 15:15

**「Background」** Aon is a major insurance broker; USI is the 10th largest U.S. insurance broker, with over $3 billion in annual revenue and more than 10,500 employees. The deal builds on Aon&\#x27;s 2024 purchase of NFP, another middle-market broker, and KKR and Canada&\#x27;s CDPQ originally acquired USI in 2017 for $4.3 billion.

<details><summary>References</summary>
<ul>
<li><a href="https://time.news/aon-nears-17-billion-deal-to-acquire-usi-insurance-services-from-kkr/">Aon Nears $17 Billion Deal to Acquire USI Insurance Services From KKR - Time News</a></li>

</ul>
</details>

**Tags**: `#M&amp;A`, `#Insurance`, `#Aon`, `#USI`, `#Middle Market`

---

<a id="item-finance-news-2"></a>
### [Warsh&\#x27;s Hawkish Jackson Hole Speech Boosts September Rate Hike Chances](https://www.cnbc.com/2026/08/31/jackson-hole-fed-chair-kevin-warsh-hawkish-rate-hikes-analysts.html) ⭐️ 8.0/10

Federal Reserve Chair Kevin Warsh&\#x27;s unexpectedly hawkish speech at Jackson Hole led traders to price in a 60.4% chance of a quarter-point rate hike at the September meeting, up from about 56% on Friday, according to CME FedWatch. Gold fell and Asian stocks declined on Monday.

rss · CNBC Finance · Aug 31, 11:28

**「Background」** Warsh has long stressed the Fed&\#x27;s 2% inflation goal, but before the speech markets saw little chance of a hike until December. Recent inflation has been cooler and hiring has slowed, leaving analysts split on whether tighter policy is warranted.

**Tags**: `#Federal Reserve`, `#Monetary Policy`, `#Rate Hikes`, `#Jackson Hole`, `#Financial Markets`

---

<a id="item-finance-news-3"></a>
### [Amazon Stock Slips as FTC Alleges Hidden Ad Fees](https://www.marketwatch.com/story/amazons-stock-slips-as-the-ftc-alleges-billions-of-dollars-in-hidden-ad-fees-4ae44ee4?mod=mw_rss_topstories) ⭐️ 8.0/10

The U.S. Federal Trade Commission \(FTC\) alleges that Amazon charged merchants billions of dollars in hidden advertising fees by raising minimum ad prices during peak shopping periods and adding surcharges; Amazon’s stock slipped after the news.

rss · MarketWatch Top Stories · Aug 31, 22:24

**「Background」** The U.S. Federal Trade Commission \(FTC\) and 22 states plan to sue Amazon, alleging that the company manipulated prices paid by marketplace merchants and caused billions of dollars in harm; Amazon&\#x27;s advertising business generated $19.8 billion in revenue last quarter.

**「Impact」** Merchants who advertise on Amazon are the directly affected group, as the alleged surcharges would raise the cost of their ad campaigns; the FTC’s case is unresolved.

<details><summary>References</summary>
<ul>
<li><a href="https://www.marketwatch.com/story/amazons-stock-slips-as-the-ftc-alleges-billions-of-dollars-in-hidden-ad-fees-4ae44ee4">Amazon ’s stock slips as the FTC alleges billions of dollars in hidden ...</a></li>
<li><a href="https://coinunited.io/en/pulse/2026-08-31/ftc-22-states-sue-amazon-over-hidden-ad-fees-amzn-cfd-leverage-scenarios-cross-market-impact">FTC &amp; 22 States Sue Amazon Over Hidden Ad Fees ... | CoinUnited.io</a></li>

</ul>
</details>

**Tags**: `#Amazon`, `#FTC`, `#advertising fees`, `#e-commerce`, `#regulation`

---

<a id="item-finance-news-4"></a>
### [Cronos halts network after estimated $75M Tectonic exploit](https://cointelegraph.com/news/cronos-network-halt-tectonic-exploit-75-million?utm_source=rss_feed&amp;utm_medium=rss&amp;utm_campaign=rss_partner_inbound) ⭐️ 8.0/10

Cronos halted its network after an exploit on the Tectonic protocol estimated at $75M, while Crypto.com CEO Kris Marszalek said the company&\#x27;s app and exchange were unaffected and continued operating normally.

rss · Cointelegraph · Aug 31, 03:25

**「Background」** Cronos is a blockchain network built by Crypto.com. On August 30, 2026, its validators paused block production after an attacker exploited Tectonic, a lending app on the network, by manipulating the price of its thinly traded TONIC token and borrowing real assets against inflated collateral. The exploit is estimated at about $75 million, and Tectonic&\#x27;s total value locked fell from about $121.7 million to roughly $3 million, according to DefiLlama. Cronos and Tectonic had not given a restart timeline or confirmed losses as of Monday morning.

**「Impact」** Tectonic users on Cronos, the chain&\#x27;s largest lending protocol, face significant losses after the exploit, and its total value locked collapsed from approximately $121.7 million to $3 million within days, undermining trust in the broader DeFi ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coindesk.com/tech/2026/08/31/cronos-halts-blockchain-after-usd75-million-lending-exploit-hits-lending-app-tectonic">Cronos halts blockchain after $75 million lending exploit hits lending app Tectonic</a></li>
<li><a href="https://www.kucoin.com/blog/cronos-tectonic-exploit-tonic-price-manipulation">Cronos Tectonic Exploit Explained: How TONIC Price Manipulation...</a></li>
<li><a href="https://www.tftc.io/cronos-halt-tectonic-exploit-75-million">Cronos Halts After $75M Tectonic DeFi Exploit · TFTC</a></li>

</ul>
</details>

**Tags**: `#Cronos`, `#Tectonic`, `#crypto exploit`, `#blockchain security`, `#DeFi`

---

<a id="item-finance-news-5"></a>
### [California wildfire-liability vote hits PG&amp;E and Edison; Aon to buy USI for $17B](https://www.cnbc.com/2026/08/31/stocks-making-the-biggest-moves-midday-pcg-eix-agco-hwm-more-.html) ⭐️ 7.0/10

California lawmakers blocked a proposal that would have limited damages individuals could seek from utilities whose equipment ignited wildfires, sending PG&amp;E shares down 19% and Edison International down 24%. Aon fell more than 7% after agreeing to buy rival USI Insurance Services from KKR for $17 billion.

rss · CNBC Finance · Aug 31, 19:49

**「Background」** After the vote, analysts downgraded both utility stocks, with Mizuho saying investors are better-positioned in utilities that have few wildfire liability issues.

**Tags**: `#Mergers and Acquisitions`, `#Utilities`, `#Earnings Guidance`, `#Executive Changes`, `#Energy Stocks`

---

<a id="item-finance-news-6"></a>
### [PG&amp;E drops 16% after California blocks wildfire-liability cap; Aon slips on $17B deal](https://www.cnbc.com/2026/08/31/stocks-making-the-biggest-moves-premarket-cvx-pcg-gme-more.html) ⭐️ 7.0/10

In premarket trading, PG&amp;E shares fell 16% after California lawmakers rejected a proposal to cap utility wildfire liability, Aon slipped 1.8% after announcing a $17 billion acquisition of KKR-owned USI Insurance Services, and U.S. oil prices rose more than 3% after U.S.-Iran strikes.

rss · CNBC Finance · Aug 31, 11:35

**「Background」** The California proposal would have limited damages individuals could seek from utilities whose equipment sparked wildfires; without it, PG&amp;E remains exposed to potentially large payout claims.

**「Impact」** The legislative outcome increases PG&amp;E’s wildfire-liability risk, and Mizuho analysts said investors are better placed in utilities with less exposure to such claims.

**Tags**: `#Mergers and Acquisitions`, `#Energy Markets`, `#Utility Regulation`, `#Premarket Movers`, `#Corporate Earnings`

---

<a id="item-finance-news-7"></a>
### [Bitmine now holds 4.9% of Ethereum supply after 65-week buying streak](https://cointelegraph.com/news/bitmine-ether-buying-streak-65-weeks-ethereum?utm_source=rss_feed&amp;utm_medium=rss&amp;utm_campaign=rss_partner_inbound) ⭐️ 7.0/10

Bitmine has bought Ether for 65 consecutive weeks, adding 53,500 ETH, and now controls about 4.9% of Ethereum&\#x27;s total supply, despite reporting an estimated $5.1 billion in paper losses.

rss · Cointelegraph · Aug 31, 15:39

**「Background」** Bitmine Immersion Technologies, a crypto mining and investment firm, has bought Ether every week for 65 consecutive weeks, and its latest purchase of 53,501 ETH brings its holdings to about 4.9% of all Ethereum supply.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cryptobreaking.com/bitmine-gains-53500-eth-lifts/">Bitmine Gains 53,500 ETH, Lifts Stake to 4.9% of Ethereum Supply</a></li>
<li><a href="https://bitrss.com/bitmine-gains-53-500-eth-lifts-stake-to-4-9-of-ethereum-supply-246916">Bitmine Gains 53,500 ETH, Lifts Stake to 4.9% of Ethereum Supply - BitRss - Crypto World News</a></li>
<li><a href="https://www.cryptobreaking.com/bitmine-reaches-4-9-of/">Bitmine Reaches 4.9% of Ethereum Supply After Adding 53.5K ETH</a></li>

</ul>
</details>

**Tags**: `#Ethereum`, `#Bitmine`, `#cryptocurrency`, `#supply accumulation`, `#market concentration`

---

<a id="item-finance-news-8"></a>
### [North Korean hackers reported moving tens of millions on Hyperliquid as Trump urges onshoring](https://www.coindesk.com/business/2026/08/31/north-korean-hackers-are-moving-tens-of-millions-on-hyperliquid-as-trump-pushes-to-onshore-the-crypto-platform) ⭐️ 6.0/10

North Korean hackers are reportedly moving tens of millions on the crypto platform Hyperliquid, while President Trump is pushing to bring the platform onshore in the U.S., raising cyber security and regulatory concerns.

rss · CoinDesk · Aug 31, 20:48

**「Background」** Hyperliquid is a decentralized derivatives trading platform that lets users trade perpetual futures without a central intermediary. President Donald Trump has said US regulators, including the CFTC chair, are working to bring Hyperliquid into the United States legally. Separately, blockchain data ties wallets linked to North Korea&\#x27;s Lazarus Group to over $30 million in bitcoin sold on the platform in the past three weeks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coindesk.com/business/2026/08/31/north-korean-hackers-are-moving-tens-of-millions-on-hyperliquid-as-trump-pushes-to-onshore-the-crypto-platform">North Korean hackers are moving tens of millions on Hyperliquid as Trump pushes to onshore the crypto platform</a></li>
<li><a href="https://cryptobriefing.com/north-korean-hackers-move-30-million-in-bitcoin-via-hyperliquid-data-reveals/">North Korean hackers move $30 million in bitcoin via Hyperliquid, data reveals</a></li>
<li><a href="https://coinspectator.com/other/2026/08/31/north-korean-hackers-are-moving-tens-of-millions-on-hyperliquid-as-trump-pushes-to-onshore-the-crypto-platform/">North Korean hackers are moving tens of millions on Hyperliquid as Trump pushes to onshore the crypto platform – CoinSpectator – Real-time Cryptocurrency News</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-19/trump-opens-door-to-hyperliquid-as-us-pulls-crypto-trade-onshore">Hyperliquid Strategies Soars After Trump Pushes for Platform ’s US...</a></li>
<li><a href="https://coinmarketcap.com/academy/article/hype-jumps-11-percent-trump-cftc-hyperliquid-us">HYPE Jumps 11% After Trump Says CFTC Is... | CoinMarketCap</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#crypto regulation`, `#North Korea`, `#Hyperliquid`, `#policy`

---