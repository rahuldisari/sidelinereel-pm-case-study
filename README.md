# 🏈 SidelineReel — Product Manager Strategy Case Study & Live Prototype

> 🚀 **Interactive Prototype:** 🔗 [Click Here to View the Interactive Prototype](https://rahuldisari.github.io/sidelinereel-pm-case-study/sidelinereel_prototype_roadmap.html)  
> 📄 **Product Spec & Documentation:** 📝 [Read Full Spec (`SidelineReel.md`)](https://github.com/rahuldisari/sidelinereel-pm-case-study/blob/main/SidelineReel.md)  
> **Role:** Product Manager Case Study | **Focus:** B2B SaaS Churn, AI OCR Accuracy, & Data-Driven Prioritization

---

## ⚡ The Context (Why Parents & Clubs Matter)
**SidelineReel** is a B2B SaaS product sold to youth sports clubs and leagues ($180k+ annual contracts). It automatically records games, detects jersey numbers via AI computer vision, and sends highlight reels to **parents** (users) and weekly recaps to **club directors** (payers). 

When the AI misidentifies a jersey number (e.g., swapping #14 for #4), **parents receive the wrong kid's highlight reel.** This single failure breaks trust, causes parents to complain to club boards, and threatens multi-thousand-dollar club renewals.

---

## 🚨 The Core Challenges
1. **The 30% Engagement Drop-Off:** 30% of generated reels sit unopened because OCR errors put the wrong kid on the cover thumbnail.
2. **The $180k Renewal Ultimatum:** Ridgeline Youth Soccer Club (our largest account) threatened to walk away in 6 weeks if live streaming wasn't added.
3. **Survey vs. Telemetry Conflict:** 58% of parents asked for complex video editing tools in surveys, but product analytics showed **only 6% opened the editor and <1% completed an edit**.

---

## 💡 The PM Decisions & Roadmap
* **Priority #1 — Roster Tagging 2.0 (HITL Engine):** Build a Human-in-the-Loop review queue for low-confidence OCR clips (<85%) and overlapping digits. This eliminates thumbnail errors and rescues the lost 30% unopened reel volume.
* **The Strategic Trade-Off (Live Streaming):** Said **NO** to building expensive native video live streaming ($500k+ engineering build). Instead, delivered a **3-week RTMP Livestream Bridge** (embedding YouTube Live/Twitch links in the team hub) to protect Ridgeline's $180k account.
* **Deprioritized Video Editor:** Overrode survey noise in favor of actual user telemetry to avoid engineering waste.

---

## 📊 Core Decision Matrix

| Feature Candidate | Status | Primary Evidence & Data | Strategic Impact |
| :--- | :--- | :--- | :--- |
| **Roster Tagging 2.0 (HITL Engine)** | **BUILD NEXT (#1)** | Support log digit swaps (#14 vs #4); 30% unopened reels | Eliminates bad thumbnails & rescues lost engagement |
| **Smart Delivery Scheduler** | **BUILD NEXT (#2)** | Dashboard telemetry (late-night push notification drop-off) | Holds overnight reels until 8 AM local time |
| **RTMP Livestream Bridge** | **BUILD NEXT (#3)** | Materials 1 & 4 ($180k Ridgeline account renewal risk) | Fast 3-week integration saves key B2B client |
| **Native In-House Live Streaming** | **DO NOT BUILD** | High bandwidth/CDN cost; 6+ month core AI distraction | Replaced with RTMP embed bridge |
| **Expanded Video Editor** | **DEPRIORITIZED** | Telemetry: 6% open rate, <1% completion rate | Avoids building features users don't actually use |

---

## 🖥️ Interactive Prototype & Repository Deliverables
All deliverables for this assignment are interlinked directly in this repository:

* 📱 **[Launch Live Web App Prototype (`SidelineReel.html`)](https://rahuldisari.github.io/sidelinereel-pm-case-study/SidelineReel.html)** — The interactive Task 3 application showing the Coach HITL verification queue, parent guardrails, and roadmap metrics.
* 📝 **[Read Product Spec & Documentation (`SidelineReel.md`)](https://github.com/rahuldisari/sidelinereel-pm-case-study/blob/main/SidelineReel.md)** — Complete Product Requirement Document (PRD) with acceptance criteria and failure mode analysis.
