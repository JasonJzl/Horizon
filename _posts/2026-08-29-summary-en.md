---
layout: default
title: "Horizon Summary: 2026-08-29 (EN)"
date: 2026-08-29
lang: en
---

> From 66 items, 15 important content pieces were selected

---

**Technology News**
1. [Htmx 4.0.0 Released](#item-tech-news-1) ⭐️ 8.0/10
2. [OpenAI announces decision on Cursor after SpaceX acquisition](#item-tech-news-2) ⭐️ 8.0/10
3. [U.S. sanctions against Autistici/Inventati, a host of noblogs.org](#item-tech-news-3) ⭐️ 8.0/10
4. [Bug rumors now become exploits within minutes, as OCaml and rclone show](#item-tech-news-4) ⭐️ 8.0/10
5. [Boot a Virtual iPhone via Apple&\#x27;s Virtualization.framework](#item-tech-news-5) ⭐️ 7.0/10
6. [Keyboard-Driven GUIs: Accessibility vs. User Experience Debate](#item-tech-news-6) ⭐️ 7.0/10

**Technology Blog**
1. [Where to Go After a Trading Bot Loses Its Edge](#item-tech-blog-1) ⭐️ 4.0/10

**Financial News**
1. [Corn and Wheat Futures Surge to Three-Year Highs](#item-finance-news-1) ⭐️ 8.0/10
2. [Appeals court says sports event contracts are state-regulated betting, not CFTC swaps](#item-finance-news-2) ⭐️ 8.0/10
3. [PayPal plunges after Advent-Stripe buyout report; Affirm, Gap, Elastic climb on earnings news](#item-finance-news-3) ⭐️ 8.0/10
4. [September Fed Rate Hike Now a Coin Flip After Warsh Speech](#item-finance-news-4) ⭐️ 7.0/10
5. [Nvidia’s revenue forecast highlights demand from SpaceX and other big chip buyers](#item-finance-news-5) ⭐️ 7.0/10
6. [Fed Chair Warsh: &\#x27;We have work to do&\#x27; on inflation at Jackson Hole](#item-finance-news-6) ⭐️ 7.0/10
7. [SBI buys 20% stake in Indonesia&\#x27;s Ajaib for $270 million to expand yen stablecoin in Southeast Asia](#item-finance-news-7) ⭐️ 7.0/10
8. [Abu Dhabi royal&\#x27;s group reportedly backs 49% stake in World Liberty crypto bank venture](#item-finance-news-8) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Htmx 4.0.0 Released](https://four.htmx.org/announcements/2026-08-28-htmx-4.0.0-is-released) ⭐️ 8.0/10

Htmx 4.0.0 has been released, according to an announcement dated August 28, 2026 on htmx.org, marking a major update to the hypermedia-driven frontend library. The supplied announcement text was not available, so no specific features, fixes, versions, or compatibility constraints from the release notes can be confirmed here. The release matters because htmx is a popular library for building interactive web interfaces with server-rendered HTML rather than JavaScript-heavy frontend frameworks.

hackernews · rmsaksida · Aug 28, 13:28 · [Discussion](https://news.ycombinator.com/item?id=49478178)

**「Background」** htmx is a JavaScript library that extends HTML with custom attributes for making AJAX requests and driving dynamic behavior directly from markup, emphasizing hypermedia and server-rendered HTML over client-side frameworks. The project grew out of intercooler.js and gained broad adoption among developers who favor simpler, server-centric web architectures. htmx 4.0 is a major rewrite of the implementation, now built on the fetch\(\) API, and introduces features such as ETag-based conditional requests, with a documented upgrade path from htmx 2.x.

**「Impact」** Existing htmx users should evaluate the 4.0 release carefully before upgrading, since the update has sparked significant community debate over decisions such as the fetch migration and new features like the hx-partial tag. The polarized reaction suggests teams may need to weigh compatibility and migration effort against the new capabilities.

**「Community Discussion」** Commenters were generally enthusiastic, with one praising htmx and saying they could not wait to try the new version and another describing experiments built with Go, htmx, and SQLite. One .NET/Angular developer offered a contrarian view, saying htmx made things more difficult by pushing presentation into the backend, and another said alpine-ajax was smaller than htmx while providing needed features.

<details><summary>References</summary>
<ul>
<li><a href="https://four.htmx.org/announcements/2026-08-28-htmx-4.0.0-is-released">htmx 4 . 0 .0 has been released ! ~ htmx</a></li>
<li><a href="https://four.htmx.org/whats-new-in-htmx-4/">htmx ~ Changes in htmx 4 . 0</a></li>
<li><a href="https://biggo.com/news/202511040131_htmx-4-community-reaction">HTMX 4 . 0 Sparks Community Debate: Fetch Migration... - BigGo News</a></li>

</ul>
</details>

**Tags**: `#htmx`, `#web development`, `#hypermedia`, `#release`, `#frontend`

---

<a id="item-tech-news-2"></a>
### [OpenAI announces decision on Cursor after SpaceX acquisition](https://openai.com/index/our-decision-on-cursor-following-its-acquisition-by-spacex/) ⭐️ 8.0/10

OpenAI has published an official decision about Cursor following Cursor&\#x27;s acquisition by SpaceX, a move that affects developer access to OpenAI models inside the coding tool. The announcement signals shifting competitive alliances among frontier AI companies, with Cursor now tied to SpaceX/xAI and its Grok models. Community context notes Cursor&\#x27;s business model has depended on reselling third-party model APIs at scale; users say third-party model access was already expensive except for Grok/Composer. The specific terms of OpenAI&\#x27;s decision are not detailed in the available material, but commenters expect it will push some Cursor users back to Anthropic or to xAI&\#x27;s own models.

hackernews · meetpateltech · Aug 29, 01:47 · [Discussion](https://news.ycombinator.com/item?id=49486172)

**「Background」** Cursor is an AI-powered code editor that has relied on models from multiple providers, including OpenAI, to offer coding assistance. SpaceX, led by Elon Musk, acquired Cursor, and OpenAI subsequently announced it would wind down its contract to provide OpenAI models to Cursor, proposing November 12, 2026 as the shutoff date. This follows earlier tensions between OpenAI and Musk-related ventures over model usage and reflects the growing competitive divide among frontier AI companies.

**「Impact」** Developers who rely on OpenAI models inside Cursor are the directly affected group: OpenAI says its decision will most affect those users, and the concrete consequence is that Cursor will no longer offer OpenAI models after SpaceX&\#x27;s acquisition, forcing affected developers to switch to other model providers inside Cursor or to different coding tools. Longer-term effects remain uncertain, but the move signals that the previously open model choice within Cursor is narrowing as AI labs reassess supplying a competitor-owned tool.

**「Community discussion」** Commenters largely view the move as a predictable consequence of Cursor selling itself to a competing model provider, and they compare it to Anthropic&\#x27;s earlier ban of xAI over ToS violations after xAI allegedly distilled Anthropic models. Several users say they will continue using Grok and Composer in Cursor, while at least one Cursor/Claude subscriber plans to drop OpenAI models entirely, and there is open speculation about whether Anthropic will follow suit despite a datacenter deal with Musk.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/our-decision-on-cursor-following-its-acquisition-by-spacex/">Our decision on Cursor following its acquisition by SpaceX - OpenAI</a></li>
<li><a href="https://www.reuters.com/business/media-telecom/openai-end-partnership-with-spacexs-cursor-2026-08-29/">OpenAI to end agreement with SpaceX&#x27;s AI coding tool Cursor ... - Reuters</a></li>
<li><a href="https://www.explainx.ai/blog/openai-ends-cursor-partnership-spacex-acquisition-august-2026">OpenAI Ends Cursor Model Access Nov 12 - explainx.ai</a></li>
<li><a href="https://openai.com/index/our-decision-on-cursor-following-its-acquisition-by-spacex/">Our decision on Cursor following its acquisition by SpaceX | OpenAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Cursor`, `#SpaceX`, `#AI competition`, `#model access`

---

<a id="item-tech-news-3"></a>
### [U.S. sanctions against Autistici/Inventati, a host of noblogs.org](https://www.inventati.org/) ⭐️ 8.0/10

The U.S. government has sanctioned Autistici/Inventati, the Italian activist hosting collective behind noblogs.org, designating the host as a &\#x27;global terrorist&\#x27; entity. The action is widely seen as unprecedented because it targets the infrastructure provider itself rather than specific content or users, raising concerns about the future of privacy and decentralized technologies. Community reports already show autistici.org is down and noblogs.org is partly dysfunctional, affecting the collective&\#x27;s users. Privacy advocates argue the sanctions could set a dangerous precedent, potentially extending to other privacy-focused projects like I2P, Monero, and Signal.

hackernews · exiguus · Aug 28, 12:58 · [Discussion](https://news.ycombinator.com/item?id=49477854)

**「Background」** Autistici/Inventati \(A/I\) is a volunteer-run Italian technology collective that provides secure communications tools, email hosting, and the noblogs.org blogging platform to activists, often describing its work as &\#x27;digital self-defense.&\#x27; Founded by participants in Italian social movements, it helped build the independent media infrastructure during the 2001 Genoa G8 protests. The U.S. Treasury and State Department have now sanctioned A/I along with other groups accused of supporting far-left terrorism; the collective denies the allegations and says it is a small volunteer-run technology collective.

**「Impact」** Users of Autistici/Inventati&\#x27;s services are facing outages, with autistici.org unreachable and noblogs.org only partly functional as a result of the sanctions.

**「Community Discussion」** Commenters largely see the sanctions as an unprecedented criminalization of infrastructure providers, drawing parallels to I2P, Monero, and Signal, while others question whether there is concrete evidence linking the collective to the PKK. Some also provide historical context, noting the group&\#x27;s involvement in activist media during the 2001 G8 protests in Genoa.

<details><summary>References</summary>
<ul>
<li><a href="https://kollektivbibliothek.noblogs.org/?p=2461">In solidarity with Autistici / Inventati | kollektivbibliothek</a></li>
<li><a href="https://news.ycombinator.com/item?id=49460834">A Statement by Autistici / Inventati Collective About US Sanctions</a></li>
<li><a href="https://www.zerohedge.com/markets/us-sanctions-3-groups-accused-supporting-far-left-terrorism">US Sanctions 3 Groups Accused Of Supporting Far-Left... | ZeroHedge</a></li>

</ul>
</details>

**Tags**: `#sanctions`, `#internet freedom`, `#hosting`, `#privacy`, `#activism`

---

<a id="item-tech-news-4"></a>
### [Bug rumors now become exploits within minutes, as OCaml and rclone show](https://simonwillison.net/2026/Aug/28/just-a-rumour-of-a-bug/) ⭐️ 8.0/10

Anil Madhavapeddy, a Cambridge professor and OCaml compiler core maintainer, reports that OCaml projects are probed for exploits within about ten minutes of patches being shared, and demonstrated that modern coding agents can turn a rumor of a bug into an exploit almost immediately. He found current open-source embargo practices incompatible with this speed and switched to DeepSeek V4 Pro when Claude refused the task. rclone maintainer Nick Craig-Wood confirms the trend: his project received about 20 security disclosures in its first 10 years, more than 40 in the last month, and around 75% contain something worth examining. GitHub CVE assignment has slowed from 2-3 days to 3-4 weeks, forcing point releases with CVE-PENDING in changelogs.

rss · Simon Willison · Aug 28, 22:12

**「Background」** Open-source security disclosures traditionally rely on embargoes: maintainers fix a vulnerability privately, then release a patch and details together. Automated watchers and AI coding agents now make that window nearly unusable because any public hint—even a patch, commit message, or rumor—can be turned into an exploit within minutes.

**「Impact」** Maintainers like those of rclone are spending large amounts of time triaging AI-driven reports and shipping releases with unresolved CVE-PENDING statuses because CVE assignment lags behind the new attack pace.

**「Community discussion」** Commenters broadly agree AI has scaled and democratized exploit finding, though some note the technique predates LLMs and is now simply mass-produced at lower-value targets. Others argue deployment/rollout lag and managerial unwillingness to fix bugs are bigger problems, and one developer describes monitoring commits for silent bug fixes.

**Tags**: `#security`, `#AI agents`, `#OCaml`, `#exploits`, `#open source`

---

<a id="item-tech-news-5"></a>
### [Boot a Virtual iPhone via Apple&\#x27;s Virtualization.framework](https://github.com/Lakr233/vphone-cli) ⭐️ 7.0/10

vphone-cli is an open-source project that boots a virtual iPhone using Apple&\#x27;s Virtualization.framework, enabling iOS testing and reverse engineering. The tool was created by Lakr233 and shared on Hacker News, and it stands out for its novel approach to iOS virtualization. Its practical value lies in giving developers and researchers a way to run a virtual iPhone for testing and analysis, though it is limited to Apple platforms and has a niche impact.

hackernews · hentrep · Aug 28, 23:02 · [Discussion](https://news.ycombinator.com/item?id=49485267)

**「Background」** Apple&\#x27;s Virtualization.framework enables macOS apps to create and run virtual machines on Apple Silicon, and the Private Cloud Compute \(PCC\) research VM infrastructure provides a way to boot iOS-like environments. vphone-cli leverages this to boot a virtual iPhone \(iOS 26\) on macOS 15+ with Apple Silicon, cross-compiling a guest daemon using Xcode and the iOS SDK. This differs from the iOS Simulator, which runs simulated apps rather than a full virtualized iOS system.

**「Impact」** Developers and security researchers on Apple platforms can now use vphone-cli to boot a virtual iPhone for testing and reverse-engineering tasks, but the tool&\#x27;s usefulness is constrained to Apple hardware and software.

**「Community Discussion」** In the Hacker News thread, commenters were curious about the extra regulatory checks that make Japan and the EU problematic regions during setup, asked how the tool differs from the iOS simulator, and wondered whether it could ever run on non-Apple hardware. One commenter noted that requiring SIP to be disabled or partially disabled could break some things, while another expressed hope that the project, if it works, would open up many testing and reverse-engineering possibilities.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Lakr233/vphone-cli">GitHub - Lakr233/ vphone - cli · GitHub</a></li>
<li><a href="https://numfer.com/Lakr233/vphone-cli">vphone - cli : Virtualize iOS on macOS</a></li>
<li><a href="https://senumy.com/vphone-cli-ios-26-virtual-iphone-setup/">vphone - cli &amp; vphone-aio: Easier iOS 26 Virtual iPhone Setup on...</a></li>

</ul>
</details>

**Tags**: `#iOS virtualization`, `#Apple Virtualization.framework`, `#reverse engineering`, `#iOS development`, `#open source`

---

<a id="item-tech-news-6"></a>
### [Keyboard-Driven GUIs: Accessibility vs. User Experience Debate](https://ckardaris.com/blog/2026/08/28/keyboard-driven-guis.html) ⭐️ 7.0/10

A blog post argues that GUIs should be designed to be fully keyboard-driven, connecting keyboard navigation to accessibility for people with disabilities and to efficiency for power users, and places responsibility on UI frameworks. The post reportedly highlights that when keyboard focus or tab order breaks, disabled users can hit serious barriers, while power users lose speed. It also suggests that older frameworks such as Cocoa/AppKit make keyboard accessibility easier, while newer or custom UI choices often neglect it. The article generated a large Hacker News discussion, with commentators adding practical accessibility experience and debating whether keyboard-driven design should be a universal requirement or only a power-user feature.

hackernews · ckardaris · Aug 28, 15:17 · [Discussion](https://news.ycombinator.com/item?id=49479837)

**「Background」** Keyboard-driven GUI design advocates that all interface actions should be accessible without a mouse, typically via shortcuts and focus-based navigation. This principle connects to broader web accessibility: standards like WCAG require keyboard operability, and ADA compliance tools exist to help organizations meet these requirements \(tool-1-1, tool-1-3\). For users with physical disabilities who rely on adaptive input devices \(tool-1-2\), comprehensive keyboard support is essential, while power users also benefit from faster, keyboard-centered workflows.

**「Community Discussion」** Commenters agree that keyboard accessibility is frequently overlooked and that a broken tab order creates real obstacles for disabled users, while pointing to frameworks like Cocoa/AppKit as examples that handle it well. Others counter that power-user experience is not the same as general user experience and that forcing keyboard-driven interactions on everyone can impose an unnecessary learning curve.

<details><summary>References</summary>
<ul>
<li><a href="https://accessibe.com/">Web Accessibility Platform for WCAG</a></li>
<li><a href="https://know-the-ada.com/adaptive-keyboards-and-mice-tools-for-physical-accessibility/">Adaptive Keyboards and Mice: Tools for Physical Accessibility – KNOW-THE-ADA</a></li>
<li><a href="https://slashdot.org/software/ada-compliance/">Best ADA Compliance Software in 2025</a></li>

</ul>
</details>

**Tags**: `#accessibility`, `#keyboard-navigation`, `#user-interface`, `#software-design`, `#hn-discussion`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Where to Go After a Trading Bot Loses Its Edge](https://www.reddit.com/r/algotrading/comments/1w0ipa5/where_do_i_go_from_here/) ⭐️ 4.0/10

reddit · r/algotrading · /u/Extension\_Ad4492 · Aug 28, 06:27

**「Background」** The author started building a trading bot as a fun experiment to disprove trading, but got hooked when it made thousands on paper over a few weeks. Using AI to develop quickly and six months of tick data, they moved into spreadbetting on Gold and Brent Crude, only to see the apparent edge disappear as market conditions changed.

**「Solution」** The author built their own candles and backtester with six strategies, then added a regime filter to classify market states by trend, direction, and timeframe agreement. After collecting 60 days of paper trades, they found no regime where any strategy was meaningfully more effective than deploying it generally. Parameter changes and new strategy backtests also failed to restore profits. The author suspects the tick stream may be unreliable and wonders whether the early profits came from an &\#x27;extreme&\#x27; trend regime that the classifier did not isolate, or whether additional timeframes triggered contradictions. Their notes suggest checking how the classifier would have classified the early days and keeping extreme trends separate if the math supports it.

**「Takeaway」** The author concludes that their failure to find a profitable market state proves day trading does not work, yet admits the conclusion is unsound and unsatisfying. The real lesson is that a short, regime-dependent experiment is too fragile to support sweeping claims—an edge may be an illusion, highly regime-specific, or hidden by unreliable data.

**Tags**: `#algorithmic trading`, `#backtesting`, `#regime filtering`, `#day trading`, `#trading edge`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Corn and Wheat Futures Surge to Three-Year Highs](https://www.cnbc.com/2026/08/28/corn-and-wheat-prices-jump-to-highest-prices-in-more-than-three-years.html) ⭐️ 8.0/10

Corn and wheat futures hit their highest prices in more than three years on Friday, with wheat settling at 784 cents per bushel \(up 3.1%\) and corn at 536.5 cents per bushel \(up 0.6%\). Wheat is up 54.5% year-to-date on Black Sea supply disruptions, while corn is up 21.8% on weaker U.S. crop expectations.

rss · CNBC Finance · Aug 28, 20:00

**「Background」** Wheat and corn futures are contracts to buy crops at a set price later; Russia and Ukraine together account for more than a quarter of global wheat exports, and the U.S. corn harvest had been expected to ease tight global supplies before a USDA report cut its yield forecast and crop tour findings showed heat damage.

**「Impact」** Higher grain prices raise costs for grain buyers and may push European livestock farmers to use more wheat for animal feed because Europe&\#x27;s drought-damaged corn crop is smaller.

**Tags**: `#agriculture`, `#commodities`, `#wheat`, `#corn`, `#supply disruption`

---

<a id="item-finance-news-2"></a>
### [Appeals court says sports event contracts are state-regulated betting, not CFTC swaps](https://www.cnbc.com/2026/08/28/appeals-court-rules-against-prediction-markets-tees-up-scotus-fight.html) ⭐️ 8.0/10

The Ninth U.S. Circuit Court of Appeals rejected requests by Kalshi, Crypto.com, and Robinhood to stop Nevada from blocking their sports-related event contracts, ruling that those contracts are sports bets subject to state regulation rather than federally regulated swaps. Because the Third Circuit ruled in April that the CFTC has exclusive jurisdiction over such contracts, legal experts say the Supreme Court will likely decide the issue.

rss · CNBC Finance · Aug 29, 02:23

**「Background」** Nevada and 44 other states argue the platforms&\#x27; sports event contracts are just sports betting, while the platforms and the Commodity Futures Trading Commission say all event contracts are swaps—derivatives under CFTC jurisdiction exclusively.

**Tags**: `#prediction markets`, `#CFTC`, `#regulation`, `#derivatives`, `#court ruling`

---

<a id="item-finance-news-3"></a>
### [PayPal plunges after Advent-Stripe buyout report; Affirm, Gap, Elastic climb on earnings news](https://www.cnbc.com/2026/08/28/stocks-making-the-biggest-moves-premarket-pypl-afrm-gap-mrvl.html) ⭐️ 8.0/10

PayPal shares fell nearly 16% in premarket trading after Bloomberg reported, citing people familiar with the matter, that Advent and Stripe had decided not to pursue a buyout of the company. Other big movers: Affirm rose 13% after fiscal Q4 revenue of $1.17 billion beat LSEG’s $1.11 billion estimate, Gap rose about 15% after second-quarter adjusted EPS of 52 cents beat the 48-cent consensus and it named a new Old Navy CEO, and Elastic gained more than 17% after full-year adjusted EPS guidance of $3.29-$3.37 topped analysts’ $3.24 estimate; Marvell, Rubrik, and Autodesk fell after guidance or margin figures missed or disappointed.

rss · CNBC Finance · Aug 28, 11:43

**「Background」** The proposed deal, attributed by Bloomberg to people familiar with the matter, would have been one of the largest leveraged buyouts, a purchase funded mostly with borrowed money.

**Tags**: `#PayPal`, `#leveraged buyout`, `#earnings guidance`, `#stock movers`, `#fintech`

---

<a id="item-finance-news-4"></a>
### [September Fed Rate Hike Now a Coin Flip After Warsh Speech](https://www.cnbc.com/2026/08/28/-september-fed-decision-now-a-coin-flip-as-rate-hike-odds-increase.html) ⭐️ 7.0/10

Investors now see roughly a coin-flip chance \(48%–56% across Kalshi, CME FedWatch and Polymarket\) that the Federal Reserve will raise its key interest rate by a quarter-point at its Sept. 16 meeting, after Chairman Kevin Warsh&\#x27;s Jackson Hole speech stressed that inflation still needs to fall further. Before the speech, markets put nearly 70% odds on no change in September.

rss · CNBC Finance · Aug 28, 15:22

**「Background」** The Federal Reserve sets short-term interest rates, and its policy committee next meets on September 16. Fed Chairman Kevin Warsh spoke at the annual Jackson Hole symposium, where he stressed the need to be confident that inflation is moving toward the Fed&\#x27;s 2% target, saying otherwise &quot;we have work to do.&quot; His hawkish tone shifted market expectations: traders using the CME FedWatch tool now see about a 56% chance of a quarter-point rate hike in September, up from roughly 35% a day earlier.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/economy/live/jackson-hole-fed-summit-live-kevin-warsh-keynote-speech-180442096.html">Jackson Hole Fed summit live: Kevin Warsh&#x27;s keynote speech comes at a pivotal moment for the Federal Reserve</a></li>
<li><a href="https://www.cnbc.com/2026/08/28/kevin-warsh-jackson-hole-federal-reserve-inflation.html">Fed Chairman Warsh warns on inflation at Jackson Hole</a></li>
<li><a href="https://www.theguardian.com/business/live/2026/aug/28/us-federal-reserve-kevin-warsh-jackson-hole-conference-inflation-economy-ftse-stock-markets-latest-updates">US Federal Reserve’s Kevin Warsh warns there will be ‘work to do’ unless high inflation eases – as it happened | Business | The Guardian</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Interest Rates`, `#Monetary Policy`, `#Inflation`, `#Treasury Yields`

---

<a id="item-finance-news-5"></a>
### [Nvidia’s revenue forecast highlights demand from SpaceX and other big chip buyers](https://www.marketwatch.com/story/nvidias-revenue-forecast-is-so-huge-that-wall-street-wonders-if-spacex-is-the-reason-1ee7a8a9?mod=mw_rss_topstories) ⭐️ 7.0/10

Nvidia’s massive revenue forecast is partly credited to strong demand from high-profile customers, including SpaceX, which recently announced it will buy only Nvidia chips. The exact size of the forecast or the sales impact is not disclosed in the report.

rss · MarketWatch Top Stories · Aug 28, 20:58

**「Background」** Nvidia&\#x27;s Aug. 14 SEC filing disclosed a $21 billion equity stake in SpaceX and a $30 billion stake in Intel, the same companies that have pledged to buy chips exclusively from Nvidia. Analysts at UBS and Mizuho have flagged that Nvidia&\#x27;s growth trajectory may depend heavily on this single relationship.

**「Impact」** SpaceX&\#x27;s exclusive commitment to buy Nvidia chips strengthens Nvidia&\#x27;s revenue outlook but increases SpaceX&\#x27;s supply chain concentration risk for AI compute, since it depends on a single chip supplier.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techtimes.com/articles/324564/20260815/nvidia-discloses-50b-equity-stake-spacex-intel-both-exclusive-chip-buyers.htm">Nvidia Discloses $50B Equity Stake in SpaceX and Intel: Both Exclusive ...</a></li>
<li><a href="https://cryptobriefing.com/nvidia-revenue-spacex-impact-speculation/">Nvidia&#x27;s revenue forecast raises speculation about SpaceX impact</a></li>
<li><a href="https://www.techrepublic.com/article/news-spacex-nvidia-exclusive-ai-chip-strategy/">Elon Musk Goes All-In on Nvidia: What SpaceX’s Chip Strategy Means for AI Infrastructure</a></li>
<li><a href="https://thebusinessperspective.com/spacex-nvidia-ai-chip-deal/">SpaceX Nvidia AI Chip Deal: Why $15B Went to Nvidia Not AMD</a></li>
<li><a href="https://www.roic.ai/news/spacex-to-rely-exclusively-on-nvidia-for-ai-compute-musk-says-08-04-2026">SpaceX to Rely Exclusively on Nvidia for AI Compute, Musk Says | Roic News</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#SpaceX`, `#AI chips`, `#revenue forecast`, `#data center demand`

---

<a id="item-finance-news-6"></a>
### [Fed Chair Warsh: &\#x27;We have work to do&\#x27; on inflation at Jackson Hole](https://www.coindesk.com/markets/2026/08/28/warsh-at-jackson-hole-we-have-work-to-do-on-inflaiton) ⭐️ 7.0/10

Fed Chair Kevin Warsh told the Jackson Hole symposium that “we have work to do” on inflation, signaling the central bank will keep addressing price pressures.

rss · CoinDesk · Aug 28, 14:05

**「Background」** Kevin Warsh was speaking at the Federal Reserve’s annual Jackson Hole conference, his first high-profile address as chair, amid rising bond yields and concerns about his approach to inflation. He reiterated the Fed’s commitment to lowering consumer prices, saying inflation is still too high and there is “work to do,” which nudged investor expectations of a possible rate increase.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=EhAKCIK-F0Q">LIVE: Fed Chair Kevin Warsh Speaks at Jackson Hole Amid Inflation ...</a></li>
<li><a href="https://www.nytimes.com/2026/08/28/business/markets-stocks-bonds-warsh-jackson-hole.html">Investors Expect Higher Rates After Fed Chairman’s Inflation Pledge</a></li>
<li><a href="https://www.cbsnews.com/news/kevin-warsh-fed-speech-jackson-hole-inflation/">Fed will have &quot;work to do&quot; if inflation doesn&#x27;t fade, Warsh ... - ...</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#inflation`, `#monetary policy`, `#Jackson Hole`, `#interest rates`

---

<a id="item-finance-news-7"></a>
### [SBI buys 20% stake in Indonesia&\#x27;s Ajaib for $270 million to expand yen stablecoin in Southeast Asia](https://www.coindesk.com/business/2026/08/28/sbi-stakes-usd270-million-in-ajaib-to-expand-yen-stablecoin-in-southeast-asia) ⭐️ 7.0/10

SBI is buying a 20% stake in Indonesian fintech company Ajaib for $270 million, according to CoinDesk, as part of a push to expand a yen-pegged stablecoin—a digital token designed to hold the value of the Japanese yen—across Southeast Asia.

rss · CoinDesk · Aug 28, 12:18

**「Background」** SBI Holdings, a Japanese financial group, is spending $270 million for a 20% stake in Indonesian online brokerage Ajaib, aiming to distribute its yen stablecoin \(a digital token pegged to the yen\) to retail investors in Southeast Asia.

**「Impact」** The investment gives SBI access to one of Southeast Asia&\#x27;s largest retail-investing markets, allowing it to distribute its yen stablecoin and blockchain-based settlement infrastructure to Indonesian retail investors.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coindesk.com/business/2026/08/28/sbi-stakes-usd270-million-in-ajaib-to-expand-yen-stablecoin-in-southeast-asia">How SBI &#x27;s $ 270 million Ajaib stake drives its Asian stablecoin ...</a></li>
<li><a href="https://gokhshtein.com/news/2026-08-28-sbi-holdings-deploys-270m-in-ajaib-to-establish-yen">SBI Holdings Deploys $ 270 M in Ajaib to Establish Yen Stablecoin ...</a></li>
<li><a href="https://www.coindesk.com/business/2026/08/28/sbi-stakes-usd270-million-in-ajaib-to-expand-yen-stablecoin-in-southeast-asia">How SBI &#x27;s $270 million Ajaib stake drives its Asian stablecoin ...</a></li>
<li><a href="https://gokhshtein.com/news/2026-08-28-sbi-holdings-deploys-270m-in-ajaib-to-establish-yen">SBI Holdings Deploys $270M in Ajaib to Establish Yen Stablecoin ...</a></li>

</ul>
</details>

**Tags**: `#SBI`, `#Ajaib`, `#stablecoin`, `#Southeast Asia`, `#fintech acquisition`

---

<a id="item-finance-news-8"></a>
### [Abu Dhabi royal&\#x27;s group reportedly backs 49% stake in World Liberty crypto bank venture](https://cointelegraph.com/news/abu-dhabi-royal-trump-world-liberty-crypto-bank-wsj?utm_source=rss_feed&amp;utm_medium=rss&amp;utm_campaign=rss_partner_inbound) ⭐️ 7.0/10

The group led by Abu Dhabi royal Sheikh Tahnoon has reportedly agreed to back a 49% stake in the holding company behind World Liberty&\#x27;s conditionally approved US trust bank, according to the Wall Street Journal.

rss · Cointelegraph · Aug 28, 04:17

**「Background」** World Liberty Financial&\#x27;s proposed US trust bank has received conditional approval. Sheikh Tahnoon bin Zayed Al Nahyan, the UAE&\#x27;s national security adviser who oversees a financial empire including AI firm G42 and investment fund MGX, previously invested $500 million in World Liberty Financial in January 2025 for a 49% stake, one of the largest sovereign-linked bets in crypto. This reported 49% stake in the holding company behind the trust bank would deepen that relationship.

<details><summary>References</summary>
<ul>
<li><a href="https://cointelegraph.com/news/abu-dhabi-royal-trump-world-liberty-crypto-bank-wsj">Abu Dhabi Royal Backs Trump -Linked Crypto Bank Venture</a></li>
<li><a href="https://bingx.com/en/flash-news/post/wsj-abu-dhabi-s-sheikh-tahnoon-and-coinvestors-hold-of-wltc-holdings-behind-world-liberty-s-planned-usd-trust-bank">Abu Dhabi &#x27;s Sheikh Tahnoon Said to Hold 49 % of World ...</a></li>
<li><a href="https://www.binance.com/en/square/post/35888183089489">Abu Dhabi royal Sheikh Tahnoon bin Zayed Al Nahyan secretly...</a></li>

</ul>
</details>

**Tags**: `#crypto banking`, `#Abu Dhabi`, `#World Liberty`, `#investment`, `#regulatory approval`

---