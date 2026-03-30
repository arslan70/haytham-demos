## 1. Problem Analysis (Top 3 Problems)

**Problem 1: Bloomberg Terminal costs $24K+/year, excluding retail investors and indie traders**
- **Trigger Moment:** "The user reaches for this product when they want to run technical analysis or screen stocks before a trade and realize their broker's charts are too basic, but a Bloomberg subscription is out of the question financially."
- **Trigger Confidence:** Observed (founder explicitly states they built it because they couldn't afford the real thing)
- **Current Workaround:** Cobbling together free tools: Yahoo Finance for quotes, TradingView free tier for charts, Google Alerts for news, manual watchlists in spreadsheets.
  - **Effort:** High [estimate: 15-30 mins per session] -- assumes switching between 3-5 browser tabs and re-entering symbols across tools
- **Pain Intensity:** High -- professionals locked out of industry-standard tooling; self-directed investors are operating with degraded signal

**Problem 2: No unified terminal experience for non-institutional users**
- **Trigger Moment:** "The user reaches for this product when they want to cross-reference a news headline with a stock chart and price alert simultaneously and realize none of their free tools talk to each other."
- **Trigger Confidence:** Inferred (fragmentation is the structural consequence of the cost barrier described above)
- **Current Workaround:** Manual context-switching between browser tabs; no single pane of glass for market data + news + screening.
  - **Effort:** Medium [estimate: 5-10 mins per workflow] -- assumes user knows their tools and is not searching for features
- **Pain Intensity:** Medium -- reduces efficiency, but users tolerate it as the cost of not paying for Bloomberg

**Problem 3: No conversational AI layer over personal market data for retail/indie users**
- **Trigger Moment:** "The user reaches for this product when they want to ask 'why did this stock drop today?' and get an AI answer that includes their own watchlist context, but ChatGPT has no market data and Bloomberg's AI is behind the paywall."
- **Trigger Confidence:** Inferred (AI financial analyst feature is listed; the need to bring your own API key implies the founder sees this gap)
- **Current Workaround:** Asking general-purpose AI tools questions without live market data; or reading analyst reports manually.
  - **Effort:** Medium [estimate: 10-20 mins per question] -- assumes reading 2-3 articles and cross-referencing charts manually
- **Pain Intensity:** Medium -- useful but not blocking; users manage without it today

---

## 2. Target User Segments

**Primary Segment: Self-directed retail investors who actively research their own trades**
- **Defining Behavior:** Opens multiple financial tabs daily; runs technical analysis before placing trades; tracks 10+ stocks on a watchlist
- **Where to Find Them:** r/investing, r/stocks, r/SecurityAnalysis, TradingView community, Stocktwits
- **Trigger Context:** Pre-market research sessions or post-market review; triggered when a news event hits their watchlist
- **Budget Indicator:** professional discretionary [needs validation]
- **Urgency Driver:** Competing on the same data as institutional players; every information gap is a potential missed trade

**Secondary Segment: Finance students, indie quants, and developers who want Bloomberg-grade tooling for learning or side projects**
- **Defining Behavior:** Builds or runs financial models outside institutional environments; uses free APIs; contributes to or forks open-source finance tools
- **Where to Find Them:** GitHub (finance repos), Hacker News, r/learnprogramming, CFA prep communities
- **Trigger Context:** When coursework or project requires market data analysis but no institutional access is provided
- **Budget Indicator:** student [needs validation]
- **Urgency Driver:** Academic deadlines; project demos; building a portfolio of financial tools

---

## 3. Unique Value Proposition

Self-directed investors get Bloomberg Terminal capabilities (real-time data, charting, screener, AI analyst) for free, with their own API key keeping costs under their control.

---

## 4. Solution Concept

- **Core Value Delivery:** A keyboard-driven, self-hostable financial terminal that surfaces the same workflow Bloomberg provides -- quotes, charts, news, screening, alerts, and AI analysis -- without a subscription.
- **Key Capabilities:**
  - Real-time multi-asset data (stocks, crypto, indices, commodities) -> addresses Problem 1
  - Integrated news feed + article reader in the same interface -> addresses Problem 2
  - Stock screener with technical indicators -> addresses Problem 1
  - Watchlist + price alerts -> addresses Problem 2
  - AI financial analyst (BYOK: bring your own key) -> addresses Problem 3

---

## 5. Lean Canvas Summary

- **Problem:** Bloomberg is financially inaccessible; no unified free terminal exists; no AI layer over personal market data for retail users
- **Segments:** Self-directed retail investors (primary); finance students and indie quants (secondary)
- **UVP:** Self-directed investors get Bloomberg Terminal capabilities for free, keeping full control of their API costs.
- **Solution:** Self-hostable terminal with real-time multi-asset data, charting, screener, watchlist, news, and BYOK AI analyst
- **Unfair Advantage:** Open-source distribution via GitHub (organic developer community); founder credibility as a cost-driven builder solving their own problem; zero subscription lock-in as structural differentiator

---

## 6. Concept Health Signals

- **Pain Clarity:** Clear -- the cost barrier to Bloomberg is a well-known, documented pain point with a large community of affected users
- **Trigger Strength:** Strong -- founder lived the trigger moment; Reddit audience validates it (side project post format implies real traction signal)
- **Willingness to Pay Signal:** Absent (by design -- this is a free/open-source product; monetization is undefined or BYOK API costs only)
