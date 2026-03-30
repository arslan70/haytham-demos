## 1. Problem Analysis

**Problem 1: Solo founders lack functional depth across disciplines required to run a company**
- **Trigger Moment:** "The user reaches for this product when they realize they need a legal contract reviewed, a marketing copy written, and a financial model updated -- all in the same week -- with no one to delegate to."
- **Trigger Confidence:** Inferred -- the idea describes "giving a single founder the leverage of a full organization" which implies the felt absence of that organization.
- **Current Workaround:** Hire freelancers per task, use multiple disconnected SaaS tools (e.g., one for legal templates, another for financial modeling), or skip the function entirely.
  - **Effort:** High
  - Time estimates: [estimate: 2-5 hours per cross-functional task] -- assumes sourcing, briefing, and reviewing external help
- **Pain Intensity:** High -- operational gaps in a startup can block fundraising, stall product launches, and create legal exposure.

**Problem 2: Context is lost between tools and sessions, forcing the founder to re-explain the business repeatedly**
- **Trigger Moment:** "The user reaches for this product when they start a new task and realize they have to re-summarize their company, product, and goals from scratch because no previous tool remembers them."
- **Trigger Confidence:** Inferred -- "compounding your company knowledge with every session" directly implies the problem of non-compounding knowledge.
- **Current Workaround:** Maintain a "context doc" or company wiki manually updated by the founder; paste it into each new AI chat session.
  - **Effort:** Medium
  - Time estimates: [estimate: 10-30 mins per session] -- assumes founder remembers to update the wiki and knows what to paste
- **Pain Intensity:** Medium -- frustrating and time-consuming, but founders adapt with workarounds.

**Problem 3: Routing the right expertise to the right problem is itself a task**
- **Trigger Moment:** "The user reaches for this product when they type a request into a general AI chat and get a generic answer because the model has no department-level specialization for their context."
- **Trigger Confidence:** Inferred -- the routing command `/soleur:go <intent>` classifies and routes, implying current tools don't do this.
- **Current Workaround:** Use a general-purpose AI assistant and manually prompt-engineer for each domain (legal, finance, marketing).
  - **Effort:** Medium
  - Time estimates: [estimate: 5-15 mins of prompt iteration per task] -- assumes founder knows enough about the domain to judge output quality
- **Pain Intensity:** Medium -- reduces quality of AI output but does not fully block work.

---

## 2. Target User Segments

**Primary Segment: Solo technical founders running pre-revenue or early-revenue startups**
- **Defining Behavior:** Ships code weekly, manages business admin alone, context-switches between engineering and non-engineering tasks daily
- **Where to Find Them:** Indie Hackers, Hacker News "Who's hiring" threads, r/startups, Product Hunt, X/Twitter startup communities
- **Trigger Context:** When preparing for an investor meeting, launching a new feature, or facing a compliance question with no one to ask
- **Budget Indicator:** Professional discretionary [needs validation] -- willing to pay for tools that replace hiring
- **Urgency Driver:** Hiring is not yet affordable; every non-technical task comes directly at the cost of product time

**Secondary Segment: Early-stage startup teams (2-3 people) without department coverage**
- **Defining Behavior:** Has a technical co-founder but no finance, legal, or marketing hire; uses ad-hoc tools per department gap
- **Where to Find Them:** YC company directories, AngelList, Slack startup communities
- **Trigger Context:** When a board meeting, contract negotiation, or campaign launch creates a sudden need outside the team's expertise
- **Budget Indicator:** Professional discretionary to early enterprise [needs validation]
- **Urgency Driver:** Specific high-stakes events (fundraise, contract, launch) demand expertise the team doesn't have

---

## 3. Unique Value Proposition

Solo founders get the output of 8 departments without making a single hire.

---

## 4. Solution Concept

- **Core Value Delivery:** A single command routes any founder task to a specialized agent with full company context already loaded -- no re-briefing, no tool-switching.
- **Key Capabilities:**
  - Intent classification and routing -> addresses Problem 3
  - Persistent, compounding company knowledge base -> addresses Problem 2
  - Specialized agents per department (engineering, finance, marketing, legal, ops, product, sales, support) -> addresses Problem 1
  - Delivered as a Claude Code plugin (zero new tool install friction) -> addresses Problem 3
  - Session-to-session knowledge accumulation -> addresses Problem 2

---

## 5. Lean Canvas Summary

- **Problem:** Solo founders lack cross-functional expertise; context is lost between sessions; routing expertise is itself a burden
- **Segments:** Solo technical founders (primary); small early-stage teams without department coverage (secondary)
- **UVP:** Solo founders get the output of 8 departments without making a single hire
- **Solution:** Intent-routing plugin with persistent company knowledge and 61 specialized department agents
- **Unfair Advantage:** BSL 1.1 license limits forks; first-mover in the Claude Code plugin ecosystem for company operations; compounding knowledge moat grows with usage

---

## 6. Concept Health Signals

- **Pain Clarity:** Clear -- the absence of a full organization for a solo founder is concrete and widely felt
- **Trigger Strength:** Moderate -- triggers are inferred from product design, not from stated user research or observed behavior
- **Willingness to Pay Signal:** Unclear -- the idea does not describe a pricing model or user validation evidence; the use of BSL 1.1 suggests a commercial intent but monetization path is unconfirmed
