# 🌙 Ramadan Athletic Performance Study

A research project and interactive web app studying how Ramadan fasting affects athletic performance across energy levels, recovery, hydration, sleep, and training completion.

**[🌐 Live Site →](https://alogailia.github.io/Athletic-Diet-Study/)**  
**[🏅 Open the Advisor App →](https://alogailia.github.io/Athletic-Diet-Study/app.html)**

---

## About

Muslim athletes at every level face a gap in structured, evidence-based guidance for training during Ramadan. This project:

- Tracks 12 athletes across 7 sports over 30 days using a daily diary methodology
- Analyzes energy, recovery, dehydration, sleep, and training completion patterns
- Delivers findings through an interactive AI-powered advisor app

---

## Repository Structure

```
ramadan-athletic-study/
├── index.html                          # Landing page / study overview
├── app.html                            # Interactive Ramadan Advisor app
├── Ramadan_Athletic_Performance.ipynb  # Full Python analysis notebook
├── README.md                           # This file
└── _config.yml                         # GitHub Pages config
```

---

## The App

The **Ramadan Athletic Advisor** (`app.html`) is a single-file web app that:

- Accepts your athlete profile (sport, intensity, gender, Ramadan day)
- Shows performance trend charts from study data (weekly, daily, by sport)
- Lets you log daily diary entries (energy, recovery, training, hydration, sleep)
- Compares your personal data to study averages
- Connects to Claude AI for personalized coaching advice
- Exports your full log as a CSV

---

## Analysis Notebook

`Ramadan_Athletic_Performance.ipynb` covers 10 sections:

1. Setup & Data Loading
2. Dataset Overview
3. Training Completion Analysis
4. Energy & Recovery Trends Over Time
5. Hydration & Sleep Impact
6. Sport-by-Sport Breakdown
7. Intensity Group Comparisons
8. Gender Comparison
9. Individual Athlete Profiles
10. Correlation Heatmap & Key Insights Summary

**Dependencies:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`

---

## Key Findings

| Finding | Stat |
|---|---|
| Energy dips in Weeks 1–2, recovers by Week 4 | +0.39 avg energy Wk1→Wk4 |
| Dehydration affects nearly half of training days | 42% overall rate |
| Fewer than half of athletes met 6-hour sleep threshold | 52% compliance |
| Training modification is the dominant coping strategy | 61% full completion, 24% modified |

---

## Project Context

This study was developed as part of a course project exploring evidence-based athletic performance research. The data was collected from 12 athletes across 7 sports over 30 days of Ramadan.

*Ramadan Mubarak 🌙*
