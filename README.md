# 🤖 Eng Performance Calibration

**[→ Live Demo](https://deckelsf.github.io/eng-calibration)**

An AI-first engineering performance calibration tool for engineering leaders. Stack rank your team, monitor AI adoption signals in real time, set proactive alert thresholds, and subscribe to automated performance digests — all in a single-file app deployable via GitHub Pages.

![Eng Calibration Screenshot](EngCalibrationScreenshot.png)

---

## The Problem

Most performance review tools are point-in-time, qualitative, and disconnected from the signals that actually matter. Engineering leaders need to know:

- Who is leaning into AI to 10x their output — and who isn't
- Who is trending down before it becomes a problem
- How to make calibration decisions (promote, keep, PIP, exit) with data, not just gut feel

---

## Features

### 🤖 AI-First Monitoring
- Live AI token usage dashboard across Claude, Cursor, and Copilot
- Per-engineer 4-week trend chart — spot declining AI adoption early
- Team AI leaderboard always visible at the top of the view
- Red flags automatically triggered when anyone drops below your token threshold

### ⊞ Three Team Views
- **Table** — sortable by any metric, inline AI alert badges, trend arrows
- **Ranked list** — visual metric bars per engineer, flag controls
- **Heatmap** — color-coded grid across all metrics for instant pattern recognition

### 🚨 Proactive Alerts
- Configurable thresholds for AI token usage, commits, PRs, cycle time, and bug rate
- Alert badge in the nav updates live as engineers cross thresholds
- Dedicated Alerts tab with full list, AI adoption health panel, and 4-week trend view

### 📬 Performance Digest
- Subscribe to weekly, bi-weekly, or monthly digests
- Delivered via email and/or Slack
- Digest includes: team health score, AI usage leaderboard, red flags, promotion candidates, and individual scorecards
- Live preview of exactly what gets sent

### 👤 Individual Evaluation
- Auto-populated quantitative metrics (GitHub, Jira, Claude API)
- Qualitative sliders for collaboration, ownership, feedback receptiveness, growth, and communication
- Auto-recommended outcome (Promote / Promote with Conditions / Keep / PIP / Exit) with manual override
- Notes field for justification

### 👥 Team Management
- Add people via CSV upload, HRIS pull (BambooHR, Workstream, Rippling, Lattice), or manual entry
- CSV template downloadable with one click
- Cut scenario tool — auto-flag bottom N engineers by any metric

### 📤 Export
- Per-person CSV export from the drawer
- Full team CSV export from the nav

---

## Data Sources

| Integration | Metrics |
|---|---|
| **Claude API** | AI token usage, prompt volume |
| **Cursor / Copilot** | AI-assisted code tokens |
| **GitHub** | Commits, PRs merged, cycle time, bug escape rate |
| **Jira / Linear** | Sprint velocity, tickets closed |
| **PagerDuty** | On-call participation, incident response |

---

## Scoring Model

Each engineer receives a weighted composite score (0–5.0):

| Signal Type | Weight |
|---|---|
| Auto-populated metrics (GitHub, Jira, AI tokens) | 55% |
| Qualitative manager assessment | 45% |

Recommendation thresholds:

| Score | Recommendation |
|---|---|
| ≥ 4.3 | Promote |
| 3.6 – 4.3 | Promote with Conditions |
| 2.7 – 3.6 | Keep at Level |
| 1.9 – 2.7 | PIP |
| < 1.9 | Exit |

All thresholds and weights are configurable in the Alerts tab.

---

## How to Use

1. Open the [live demo](https://deckelsf.github.io/eng-calibration)
2. Review the **AI Adoption Dashboard** at the top — see who's above and below token thresholds
3. Use the **Team View** to sort, compare, and flag engineers across any metric
4. Click any engineer to open their **detail drawer** — review AI trends, adjust qualitative scores, set a recommendation
5. Go to **Alerts** to configure thresholds and see all active flags
6. Go to **Digest** to subscribe to weekly/monthly team health reports via email or Slack
7. Add your own team via **👤 Add People** in the nav — CSV upload, HRIS pull, or manual entry

---

## Built With

- Vanilla JavaScript (no framework, no build step)
- Single `index.html` — deployable anywhere
- Google Fonts — Geist + Geist Mono

---

## About

Built by a PM at [Workstream](https://www.workstream.us) (SMB SaaS — hiring, HR, and payroll for hourly workers) as a portfolio project demonstrating product thinking around:

- **AI adoption as a first-class performance signal** — the belief that engineers who lean into AI compound their output; those who don't fall behind
- **Proactive monitoring over point-in-time reviews** — catching problems early with configurable thresholds and trend detection
- **Data-informed calibration** — combining quantitative signals from integrations with qualitative manager judgment, weighted and scored transparently
