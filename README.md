# 🏈 SidelineReel — Product Manager Strategy Case Study & Live Prototype

> **Live Demo:** 🔗 [Click Here to View the Interactive Prototype](https://<YOUR-GITHUB-USERNAME>.github.io/sidelinereel-pm-case-study/)  
> **Role:** Product Manager Case Study  
> **Focus:** B2B SaaS Churn, AI OCR Accuracy, Data-Driven Prioritization, Human-In-The-Loop (HITL) Workflows

---

## ⚡ 10-Second Executive Summary

### The Context
**SidelineReel** automatically detects youth sports jersey numbers in video footage and sends AI-generated highlight reels to parents and weekly recaps to youth sports clubs ($180k+ annual accounts).

### The Challenge
1. **30% Engagement Drop-Off:** 30% of generated reels sit unopened because OCR errors put the wrong kid on the cover thumbnail (e.g., swapping jersey #14 for #4, or #1 for #11).
2. **$180k Revenue at Risk:** The biggest club client (Ridgeline) threatened to cancel their $180k renewal in 6 weeks if live streaming wasn't added to the product roadmap.
3. **Survey vs. Telemetry Noise:** 58% of parents asked for complex video editing tools in surveys, but telemetry showed only **6% opened the editor and <1% completed an edit**.

### The PM Solution & Decisions
* **Priority #1 — Roster Tagging 2.0 (HITL Engine):** Route low-confidence OCR clips (<85%) and ambiguous digit pairs to a 20-second post-game Coach Review Queue to eliminate thumbnail errors and recover the lost 30% unopened reel volume.
* **The Strategic Trade-Off (Live Streaming):** Said **NO** to building expensive native video live streaming ($500k+ engineering build). Instead, offered a **3-week RTMP Livestream Bridge** (embedding YouTube Live/Twitch links in the team hub) to protect Ridgeline's $180k account without derailing the AI core.
* **Deprioritized Video Editor:** Overrode survey requests in favor of behavioral data to avoid engineering waste.

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

## 🖥️ Interactive Prototype Features
The included **`index.html`** prototype demonstrates the three core workflows:

1. **Coach HITL Verification Dashboard:** Shows flagged clips with OCR confidence scores and 1-tap jersey confirmation.
2. **Parent Guardrails & Scheduler:** Simulates held overnight notifications and a single-tap "Report Wrong Kid" feedback loop.
3. **Product Roadmap & Metrics View:** Visual breakdown of user telemetry vs. survey feedback.

👉 **[Try the Live Web App Prototype](https://<YOUR-GITHUB-USERNAME>.github.io/sidelinereel-pm-case-study/)**

---

## 📂 Repository Contents
* **`index.html`**: Runnable interactive prototype (HTML, Tailwind CSS, JavaScript).
* **`spec.md` / `sidelinereel.md`**: Full Product Requirement Document (PRD) including acceptance criteria, failure modes, and HITL flowcharts.
* **`sidelinereel.html`**: Raw Replit application code export.
