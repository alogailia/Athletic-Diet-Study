# 🌙 Ramadan Athletic Performance Study

A research project and working prototype studying how Ramadan fasting affects athletic performance. Built around a dataset of 12 athletes, a Python analysis notebook, and an interactive AI-assisted coaching application.

**[🌐 Live Site →](https://alogailia.github.io/Athletic-Diet-Study/)**  
**[🏅 Open the Advisor App →](https://alogailia.github.io/Athletic-Diet-Study/app.html)**

---

## About

Muslim athletes at every level face a gap in structured, evidence-based guidance for training during Ramadan. This project is a working prototype that that demonstrates how structured data collection and AI-assisted coaching could work for this population. It's built on a small dataset, documented clearly enough that it could be extended.

---

## What Was Built
 
### The Dataset
- 12 athletes across a mix of sports and genders
- 30 days of Ramadan diary data (energy, recovery, hydration, sleep, training completion)
- Collected at a local gym during Ramadan 2026
- N=12 is small: findings are treated as directional, not definitive, and are mapped against published literature rather than presented as standalone conclusions

## The App

A single-page web app with four features:
- Athlete profile: sport, training intensity, gender, current Ramadan day
- Performance trend charts: weekly averages, day-by-day view, sport comparison
- Daily training log: logs energy, recovery, hydration, sleep, and training completion with username-based data persistence and CSV export
- AI coaching interface: gives sport and week-specific guidance based on logged data (see Coach Logic below)

---

## Analysis Notebook

`Ramadan_Athletic_Performance.ipynb` — 10 sections covering training completion, energy/recovery trends, dehydration and sleep impact, sport and intensity breakdowns, gender comparison, individual athlete profiles, and a correlation heatmap. Available in this repository.

---

## Coach Logic — How the Advisor Works
 
The AI coach gives responses that vary based on three inputs: sport, Ramadan week, and logged diary data. The decision rules are documented here so the logic is transparent and reviewable.
 
### By Energy Level (logged daily)
| Energy Score | Guidance |
|---|---|
| 1–2 (Very Low) | Reduce session intensity by ~40%. Prioritize mobility or light skill work. Flag to coach. |
| 3 (Moderate) | Maintain planned session with modified rep ranges or reduced volume. |
| 4–5 (Normal) | Proceed with full session. Monitor hydration closely post-training. |
 
### By Recovery Score (logged daily)
| Recovery Score | Guidance |
|---|---|
| 1–2 (Poor) | Rest day or active recovery only. Do not stack consecutive low-recovery sessions. |
| 3 (Partial) | Lower-intensity session acceptable. Prioritize sleep window before next session. |
| 4–5 (Full) | Normal training load appropriate. |
 
### By Ramadan Week
| Week | Expected Pattern | Coach Focus |
|---|---|---|
| Week 1 (Days 1–6) | Adaptation — energy dip begins | Reduce volume, establish hydration routine at iftar |
| Week 2 (Days 7–13) | Settling — sleep hit hardest | Prioritize sleep window, consider session timing shift |
| Week 3 (Days 14–20) | Fatigue peak — lowest avg scores | Lowest intensity week, recovery sessions over performance |
| Week 4 (Days 21–27) | Mental push — motivation rises | Gradual intensity rebuild, maintain hydration discipline |
| Week 5 (Days 28–30) | Final stretch | Conserve, finish strong, prepare for Eid transition |
 
### By Dehydration (logged daily)
- Reported dehydrated → coach emphasizes post-iftar hydration window (500–750ml within 30 min of iftar), pre-suhoor water intake, and electrolyte replenishment before next session
- Not dehydrated → coach reinforces current strategy and adjusts advice based on energy/recovery scores
 
### By Sport
- High-intensity sports (Track, Soccer, Wrestling) — higher dehydration risk, more aggressive hydration guidance, stronger intensity scaling recommendations
- Moderate-intensity sports (Basketball, Volleyball, Swimming) — balanced guidance, focus on session timing relative to iftar
- Lower-intensity sports (Tennis) — maintenance-focused, recovery optimization prioritized
 
---

## Key Findings

| Finding | Stat | Note |
|---|---|---|
| Energy dips Weeks 1–2, recovers by Week 4 | +0.39 avg energy Wk1→Wk4 | Consistent with published literature |
| Dehydration affects nearly half of training days | 42% overall rate | 58% among high-intensity athletes |
| Fewer than half met 6-hour sleep threshold | 52% compliance | Week 2 lowest at 44% |
| Training modification dominant coping strategy | 61% full, 24% modified | Full skips peaked Week 2 |
| Data collection itself is a challenge | Inconsistent logging during Ramadan | Points to need for passive data collection |
 
These findings are treated as a foundation to map onto published datasets — not standalone conclusions. A larger study using this framework would need 40–50+ participants to support sport and gender-specific analysis.

---

## What a Larger Study Would Need
 
- Minimum 40–50 participants for meaningful sport/gender splits
- Passive data collection to reduce logging burden
- Push notification reminders to sustain daily compliance
- Pre-Ramadan baseline period (2 weeks prior) for within-subject comparison
- Post-Ramadan follow-up to measure return to baseline
 
---

## Repository Structure
 
```
Athletic-Diet-Study/
├── index.html                          # Project landing page
├── app.html                            # Ramadan Tracker & Coaching Framework app
├── Ramadan_Athletic_Performance.ipynb  # Python analysis notebook
├── README.md                           # This file
└── _config.yml                         # GitHub Pages config
```
 
---

## Project Context

Built as part of a course project. Data collected from 12 athletes at a local gym during Ramadan 2026. The goal is to demonstrate a working framework for data collection and AI-assisted coaching.

*Ramadan Mubarak 🌙*
