We ran a market analysis on BLMTRM based on your [Reddit post](https://www.reddit.com/r/SideProject/comments/1s7ixfu/i_spent_2_weeks_building_a_free_bloomberg/). The competitive window is real and the timing is good, but the data quality gap is likely to bite you before anything else does.

## What we found that you might not know

**OpenBB has quietly vacated your niche.** In October 2024, OpenBB repositioned as an enterprise "AI Workspace for Finance" with SOC 2 and VPC deployments (TechCrunch). Users are reporting installation failures on Windows (GitHub Issues #4591, #6499). The consumer-facing open-source terminal slot is empty. That said, they still hold 64K GitHub stars and dominate SEO, so discoverability is an uphill fight.

**The "unification" pitch may not be what drives adoption.** We looked for direct evidence that users want a single terminal replacing their TradingView + FINVIZ + Yahoo Finance workflow and didn't find any. Multiple sources suggest users have *accommodated* the fragmentation. Your product may win on a different axis entirely: the keyboard-driven UX, the AI analyst, or the open-source ethos. Worth tracking which feature early users actually mention.

**Koyfin already owns the "Bloomberg without the price" search query.** They have 500K+ users, a generous free tier, and years of data partnerships. Anyone Googling "free Bloomberg alternative" will find Koyfin before BLMTRM. Your distribution edge is GitHub and Reddit, not search.

## The sharpest risk

Free APIs from Yahoo Finance and Alpha Vantage deliver 15-20 minute delayed data with rate limits. Real-time exchange-level quotes require premium keys from Polygon.io ($199/mo+) or Databento. The BYOK model solves the AI cost problem but not the data cost problem. If someone downloads BLMTRM expecting Bloomberg-grade data and gets 15-minute delays, that first impression is hard to recover from. A visible "data delayed 15 min" badge when using free APIs protects trust.

## One thing to try

Post on r/investing, r/stocks, and Hacker News with a link to a hosted demo, instrumented with basic analytics (Plausible or PostHog free tier). You already posted on r/SideProject, but those subreddits are where your actual users are. Measure D7 return rate, not just stars or upvotes. "Working" looks like 500+ GitHub stars in two weeks AND 10%+ of demo visitors returning after 7 days. "Not working" looks like strong stars but under 5% return rate, meaning the product is interesting but not sticky. If that happens, you might get more traction shipping the data + AI layer as a developer library rather than a consumer terminal.

Full report with competitive analysis, risk profile, and financial breakdown: [validation-report.md](validation-report.md)
