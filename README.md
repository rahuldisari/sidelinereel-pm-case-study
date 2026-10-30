# 🏈 SidelineReel — Product Manager Case Study & A/B Prototype Exploration

> 🧪 **Prototype A/B Testing & Design Iteration:**  
> * **[Launch Variant B — Interactive Core Flow ](https://rahuldisari.github.io/sidelinereel_prototype_roadmap.html/)** — *Focuses on high-interactivity, coach verification state switches, and live feedback loops.*  
> * **[Launch Variant A — Visual Overview & Dashboard Site](https://rahuldisari.github.io/sidelinereel-pm-case-study/SidelineReel.html)** — *Focuses on high-level executive dashboard summaries and roadmap visual architecture.*  
>  
> 📄 **Product Spec & Documentation:** 📝 [Read Full Spec (`SidelineReel.md`)](https://github.com/rahuldisari/sidelinereel-pm-case-study/blob/main/SidelineReel.md)  
> **Role:** Product Manager Case Study | **Focus:** B2B SaaS Churn, AI OCR Accuracy, & Data-Driven Prioritization

---

## 🔬 A/B Prototype Exploration & Usability Evaluation

To determine the most effective user experience for both internal coaches and external stakeholders, two prototype variants were built and evaluated:

| Metric / Dimension | Variant A: Executive Summary View | Variant B: Interactive HITL Flow (Selected) |
| :--- | :--- | :--- |
| **Primary Target User** | Executive Leadership / Club Board | Coaches & Parents (Daily Operational Flow) |
| **Core Strengths** | Scannable high-level roadmap metrics, clean visual layout for presentations | Hands-on state switches, live 1-click crop verification, real-time feedback loops |
| **Usability Focus** | Comprehensive dashboard overview | Reduced cognitive load for post-game coach task completion |
| **Decision Outcome** | Retained for executive dashboard reporting | **Selected for Core Product Build** due to superior task completion speed in HITL testing |

---

## ⚡ The Business Context
**SidelineReel** is a B2B SaaS product sold to youth sports clubs ($180k+ annual contracts). It automatically detects jersey numbers via computer vision and sends highlight reels to parents and weekly recaps to club directors.

When the AI misidentifies a jersey number (e.g., swapping #14 for #4), **parents receive the wrong kid's reel.** This single failure breaks trust, drives parent complaints to club boards, and threatens multi-thousand-dollar account renewals.

---

## 🚨 Core PM Challenges & Strategic Trade-Offs

1. **The 30% Engagement Drop-Off:** 30% of generated reels sit unopened because OCR errors put the wrong kid on the cover thumbnail.  
   * **Solution:** Roster Tagging 2.0 with Human-In-The-Loop (HITL) review for low-confidence OCR clips (<85%).
2. **The $180k Renewal Ultimatum:** Ridgeline Youth Soccer Club threatened to walk away in 6 weeks if live streaming wasn't added.  
   * **Solution:** Said **NO** to a 6-month native streaming build ($500k+ engineering cost). Delivered a **3-week RTMP Livestream Bridge** (embedding YouTube Live/Twitch links in the team hub) to protect Ridgeline's $180k account.
3. **Survey vs. Telemetry Conflict:** 58% of parents asked for complex video editing tools in surveys, but product analytics showed **only 6% opened the editor and <1% completed an edit**.  
   * **Solution:** Deprioritized video editing tools to avoid engineering waste.

---

## 📊 Feature Decision Matrix

| Candidate Initiative | Decision | Key Evidence & Data | Strategic Impact |
| :--- | :--- | :--- | :--- |
| **Roster Tagging 2.0 (HITL Engine)** | **BUILD NEXT (#1)** | Support log digit swaps (#14 vs #4); 30% unopened reels | Eliminates bad thumbnails & rescues lost engagement |
| **Smart Delivery Scheduler** | **BUILD NEXT (#2)** | Late-night push notification drop-off telemetry | Holds overnight reels until 8:00 AM local time |
| **RTMP Livestream Bridge** | **BUILD NEXT (#3)** | Materials 1 & 4 ($180k Ridgeline renewal risk) | Fast 3-week integration saves key B2B client |
| **Native In-House Live Streaming** | **DO NOT BUILD** | High CDN bandwidth cost; 6+ month core AI distraction | Replaced with RTMP embed bridge |
| **Expanded Video Editor** | **DEPRIORITIZED** | Telemetry: 6% open rate, <1% completion rate | Avoids building features users don't actually use |
