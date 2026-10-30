# sidelinereel-pm-case-study
Data-backed PM case study &amp; interactive prototype solving AI OCR roster tagging errors, retention drop-offs, and B2B SaaS account risks for SidelineReel.
sidelinereel-pm-case-study/
│
├── README.md               # The full case study write-up (Recruiters read this first)
├── index.html              # Your working Task 3 interactive prototype
├── docs/                   # Optional folder for screenshots or wireframes
└── spec.md                 # Detailed Product Requirement Document (PRD)

# SidelineReel: Roster Tagging 2.0 & Strategic Roadmap Case Study

> **Role:** Product Manager (Case Study / Portfolio Project)  
> **Challenge:** Solve automated highlight accuracy issues, handle a high-stakes enterprise account renewal ($180k Ridgeline account demanding live streaming), and balance conflicting parent survey data against actual telemetry.

---

## 📌 Executive Summary
SidelineReel automates youth sports highlight reels by matching jersey numbers in match footage to team rosters. However, core engagement was bottlenecked: **30% of generated reels were never opened**, driven by jersey number misidentifications (e.g., #14 vs #4) and poor notification timing. 

This case study covers:
1. **The Roadmap Call:** Rigorous, evidence-based prioritization (saying **NO** to building in-house live streaming and video editing tools).
2. **The Product Spec:** Human-in-the-Loop (HITL) OCR verification & delivery scheduling.
3. **Working Prototype:** A fully interactive single-file prototype demonstrating the coach verification queue and parent notification guardrails.

---

## 🚀 1. Strategic Prioritization & Trade-offs (Task 1)

| Priority | Initiative | Strategic Rationale & Evidence |
| :--- | :--- | :--- |
| **#1** | **Roster Tagging 2.0 (HITL OCR Engine)** | **Support & Analytics (Materials 3 & 5):** Fixes repetitive digit-swap errors (#14 vs #4, #1 vs #11) and unlocks the 30% unopened reel volume caused by wrong thumbnails. |
| **#2** | **Smart Notification Scheduling** | **Analytics (Material 5):** Prevents late-night notification drop-offs by holding overnight recaps until 8:00 AM local time. |
| **#3** | **Turnkey RTMP Livestream Bridge** | **Sales Risk (Materials 1 & 4):** Satisfies Ridgeline’s $180k renewal ultimatum for live streaming via a lightweight embedded RTMP bridge instead of a $500k+ custom video CDN build. |
| **DEPRIORITIZED** | **Expanded Reel Editor** | **Survey vs. Telemetry (Material 2):** 58% asked for it in surveys, but **only 6% opened it and <1% completed an edit**. Avoided engineering waste. |

---

## 📋 2. Product Specification Highlights (Task 2)
* **Core Outcome:** >99.2% jersey-to-player mapping accuracy; reduce zero-open reel volume from 30% to <5%.
* **Human-in-the-Loop Workflow:** 
  1. AI OCR flags low-confidence (<85%) or overlapping digit pairs (e.g., #4 and #14).
  2. Routed to a 30-second post-game **Coach Verification Queue** for 1-tap confirmation.
  3. Parent "Not My Kid" safety flag instantly suppresses and re-queues erroneous clips.

---

## 💻 3. Interactive Prototype (Task 3)
* **Live Demo / File:** You can run `index.html` locally in any browser or view it hosted here: [Link to your hosted version / GitHub Pages]
* **Key Features Built:**
  * **Coach HITL Dashboard:** Review queue with OCR confidence scores and jersey crop previews.
  * **Parent Preview & Guardrails:** Delivery time scheduler & instant correction feedback.
  * **Roadmap & Analytics Tab:** Executive summary of metrics and trade-offs.

---

## 🛠️ How to Run the Prototype Locally
1. Clone the repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/sidelinereel-pm-case-study.git](https://github.com/YOUR_USERNAME/sidelinereel-pm-case-study.git)
