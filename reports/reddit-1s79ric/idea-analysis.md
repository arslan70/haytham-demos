## 1. Problem Analysis

**Problem 1: Paid screenshot tools charge for features that belong in the OS**
- **Trigger Moment:** "The user reaches for this product when they open their renewal email for CleanShot X (or similar) and realize they're paying $30-50/year for a capture-annotate-save workflow that macOS Screenshot.app handles poorly"
- **Trigger Confidence:** Observed -- founder states this motivation directly ("I was tired of paying for CleanShot X")
- **Current Workaround:** Pay for CleanShot X, Snagit, or similar. Or use the native macOS screenshot tool and annotate in Preview. Inadequate because native tools lack rich annotation, quick upload, or OCR in one flow.
  - **Effort:** Medium
  - [estimate: 5-10 mins per screenshot workflow] -- assumes copy, annotate, redact, and share are done in separate apps
- **Pain Intensity:** Medium -- people tolerate it by paying, but actively seek free alternatives on forums

**Problem 2: Screenshots containing sensitive data (PII, secrets) get shared accidentally**
- **Trigger Moment:** "The user reaches for this product when they're about to paste a screenshot into a Slack message and realize it contains an API key or phone number they need to redact manually"
- **Trigger Confidence:** Inferred -- auto-redact PII is a listed feature; no direct founder statement about user pain here
- **Current Workaround:** Manually blur or crop in Preview or a separate editor. Inadequate because it's slow and error-prone.
  - **Effort:** High
  - [estimate: 2-5 mins per incident] -- assumes the user notices the sensitive data at all
- **Pain Intensity:** Medium -- pain spikes when a leak occurs; otherwise ignored until then

**Problem 3: Screen recordings and captures are scattered across apps and storage**
- **Trigger Moment:** "The user reaches for this product when they finish a screen recording and have to manually convert it, upload it to Drive or S3, and share the link -- using three different tools"
- **Trigger Confidence:** Inferred -- upload integrations and recording features imply this need
- **Current Workaround:** Use QuickTime for recording, Handbrake or ffmpeg for conversion, then manual upload. Inadequate because the workflow is fragmented and slow.
  - **Effort:** High
  - [estimate: 10-15 mins per recording workflow] -- assumes MP4/GIF conversion and upload to cloud storage
- **Pain Intensity:** Medium -- developers and technical users feel this most acutely

---

## 2. Target User Segments

**Primary Segment: Mac developers and technical users who share screenshots as part of their daily workflow**
- **Defining Behavior:** Screenshots code, error messages, UI bugs, or terminal output multiple times per day and shares them in Slack, GitHub issues, or documentation
- **Where to Find Them:** r/SideProject, r/macapps, Hacker News, developer Discord servers, GitHub
- **Trigger Context:** During code review, bug reporting, or writing documentation
- **Budget Indicator:** Professional discretionary [needs validation]
- **Urgency Driver:** Time cost of a clunky workflow compounds daily; open-source/free alternative eliminates license friction for tools shared across teams

**Secondary Segment: Content creators and designers producing polished product screenshots**
- **Defining Behavior:** Uses beautify mode, annotation tools, and gradient backgrounds to produce marketing or tutorial screenshots
- **Where to Find Them:** Twitter/X #buildinpublic, Product Hunt, designer communities on Discord
- **Trigger Context:** Preparing app store screenshots, blog posts, or social media content
- **Budget Indicator:** Professional discretionary [needs validation]
- **Urgency Driver:** Aesthetic output quality matters; free tools typically look utilitarian

---

## 3. Unique Value Proposition

Mac developers can replace their paid screenshot tool with a native, feature-complete open-source alternative that auto-redacts PII before sharing.

---

## 4. Solution Concept

- **Core Value Delivery:** A full capture-annotate-share workflow in one native macOS app, with no subscription and no Electron overhead
- **Key Capabilities:**
  - Capture + annotate in one flow (18 tools) -> addresses Problem 1
  - Auto-redact PII before sharing -> addresses Problem 2
  - Screen recording (MP4/GIF) + direct cloud upload -> addresses Problem 3
  - OCR text extraction (30+ languages) -> addresses Problem 1
  - Editor for compositing multiple captures -> addresses Problem 1

---

## 5. Lean Canvas Summary

- **Problem:** (1) Paid tools charge subscription fees for core capture/annotate workflows; (2) PII in screenshots gets shared accidentally; (3) recording-to-share pipeline is fragmented across apps
- **Segments:** Primary: Mac developers sharing screenshots daily; Secondary: Content creators producing polished product visuals
- **UVP:** Mac developers can replace their paid screenshot tool with a native, feature-complete open-source alternative that auto-redacts PII before sharing
- **Solution:** Native Swift/AppKit app -- capture, annotate, redact, record, upload in one flow; no subscription; GPLv3
- **Unfair Advantage:** Existing open-source codebase (v3.4 shipped), Homebrew distribution, GPLv3 community lock-in, zero-cost positioning against paid incumbents

---

## 6. Concept Health Signals

- **Pain Clarity:** Clear -- founder experienced the problem personally; PII redact and fragmented recording workflow are concrete secondary pains
- **Trigger Strength:** Moderate -- primary trigger (renewal cost) is observed; secondary triggers are inferred from feature list, not from described user research
- **Willingness to Pay Signal:** Absent -- this is a free/open-source product; monetization is not the stated goal
