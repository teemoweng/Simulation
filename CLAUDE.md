---
type: Operating Rules
title: Markstrat Simulation（Corporate Strategy & Economics）— Claude 操作规则
description: Markstrat 营销仿真小组作业的决策流程、数据组织与最终报告规则
tags: [workspace-meta, reference, how-to, Markstrat, 营销仿真, 小组作业, TITANS, Sonite, Vodite, 帝国理工]
---

# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

---

## Project Overview

**Markstrat marketing simulation** — Teemo's *Corporate Strategy and Economics Simulation* module at Imperial College Business School (ESB programme, instructor: Sven Mikolon). Team: **TITANS** (firm code T). 6 rounds (Periods 1–6), decisions submitted weekly 1–22 May 2026.

**Assessment:** 30% simulation SPI + 70% final group report (≤2,000 words, due 8 June 2026 16:00 BST via Insendi).

For current simulation state, read the latest `Round{N}_Results.md` and `Round{N}_MarketResearch.md`.

---

## Session Kickoff Protocol

When the user says anything like "help me with this round's decisions" / "开始做这轮决策" / "let's do Round N", immediately run this intake sequence — do not jump to analysis until all inputs are collected.

**Step A — Establish context**
Ask: "Which round are we working on? Please also share `Round{N-1}_Final_Decisions.md` so I can see what was actually submitted last round (it may differ from the Decision Guide)."
→ Read that file before proceeding.

**Step B — Collect Results data**
Say: "Please paste the raw results from Round {N-1} — this includes company P&L, brand contributions, market share, production outcomes, and any other data the simulation showed after submission."
→ Organise and save as `Round{N-1}_Results.md`, then confirm: "Results saved. Ready for market research data."

**Step C — Collect Market Research data**
Say: "Now please paste the market research reports you purchased last round — Consumer Survey, Consumer Panel, Semantic Scales, MDS, experiment results, etc. Paste them one section at a time if easier."
→ Organise and save as `Round{N-1}_MarketResearch.md`, then confirm: "All inputs collected. Starting analysis."

**Step D — Generate Decision Guide**
Analyse all inputs → produce `Round{N}_Decision_Analysis.md` first (internal reasoning), then `Round{N}_Decision_Guide_EN.html` (9-tab fill-in guide for the team).

> If the user skips ahead (e.g. pastes results without sharing Final_Decisions first), accept the data and note what's still missing — don't block progress.

---

## Per-Round Workflow

Each round follows these four steps in order:

**Step 1 — Confirm Last Round's Actual Decisions**
Request `Round{N-1}_Final_Decisions.md` from Teemo. The submitted decisions may differ from the Decision Guide — always work from the actual submission, not the guide.

**Step 2 — Process Results**
Teemo provides raw results data (company P&L, market share, brand metrics, etc.). Organise and save as `Round{N}_Results.md`. Cover: SPI standings, brand CAM, production outcomes, competitive moves, key anomalies.
→ After saving the `.md`, generate `Round{N}_Results_Analysis_EN.html` — the English HTML report summarising last round's results, what worked, what went wrong, and key signals. This is shared directly with teammates.

**Step 3 — Process Market Research**
Teemo provides raw market research data (Consumer Survey, Consumer Panel, Semantic Scales, MDS, experiments, etc.). Organise and save as `Round{N}_MarketResearch.md`. Cover: awareness, purchase intent, perceptual positions, ideal point drift, experiment results.

**Step 4 — Generate Decision Guide**
Synthesise Steps 1–3. Produce:
- `Round{N}_Decision_Analysis.md` — full analysis and rationale (5 modules: R&D → Brand Portfolio → Marketing Mix → Commercial Team → Market Research)
- `Round{N}_Decision_Guide_EN.html` — fill-in guide for teammates (see Document Standards below)

**Two HTML deliverables per round (both shared with teammates in English):**
1. `Round{N}_Results_Analysis_EN.html` — recap of the previous round: what happened, what worked, what went wrong, signals for next round
2. `Round{N}_Decision_Guide_EN.html` — fill-in decision guide for the current round's submissions

---

## Document Standards

### HTML Decision Guide
- **Language: English only** (teammates are native English speakers)
- **Reuse the 9-tab structure** from `Round4_Decision_Guide_EN.html` as the template:
  - Tabs: Overview · R&D · Brand Portfolio · TONE · TOPS · [brand] · [brand] · Sales Team · Market Research
  - Per-brand tabs each cover: ① Production Plan · ② Price · ③ Advertising (Media + Research budget + segment allocation bar) · ④ Perceptual Objectives
  - Fill-in values displayed in orange `.fv` boxes; new brand actions in purple
  - Overview tab: budget bar + 5 priority actions + 4-brand quick-reference cards
- Design system (CSS variables, badge/alert/card classes) should be carried forward unchanged between rounds

### Markdown Files
- Language: Chinese or English — Teemo's choice per session (default Chinese)
- Results and MarketResearch files should be structured with consistent section headers so data is easy to locate across rounds

### File Naming Convention
All round files live in `round{N}/` subdirectories. Reference PDFs and evergreen docs live in `reference/`.

```
round{N}/Round{N}_Final_Decisions.md           ← actual submitted decisions (source of truth)
round{N}/Round{N}_Results.md                   ← processed results data (Chinese)
round{N}/Round{N}_Results_Analysis_EN.html     ← results recap HTML for teammates (English) ← NEW
round{N}/Round{N}_MarketResearch.md            ← processed market research data (Chinese)
round{N}/Round{N}_Decision_Analysis.md         ← analysis + rationale (Chinese)
round{N}/Round{N}_Decision_Guide_EN.html       ← fill-in decision guide for team (English)
```

---

## Key Reference Files

| File | Purpose |
|---|---|
| `reference/Participant-Handbook.pdf` | **Authoritative** mechanics reference — overrides all other sources |
| `reference/Markstrat7_Challenge1_MS7-SM-B2C-DG.pdf` | Intro deck — ⚠️ base cost minima are wrong ($10); use Handbook values (Sonite ≥$25, Vodite ≥$30) |
| `reference/Markstrat_Key_Parameters.md` | Quick-reference parameter tables |
| `reference/Schoemaker_1995.pdf` | Required reading for final report (Scenario Planning framework) |
| `reference/Markstrat_Decision_Framework.md` | Reusable 5-module decision framework (backup reference) |

---

## Communication Defaults

- **Default to Chinese** for explanations and advice — Teemo is more comfortable in Chinese for unfamiliar topics
- Use real-world analogies: Sonite ≈ laptop/tablet, Vodite ≈ AR glasses/Vision Pro
- Teemo needs to convince teammates — frame recommendations accordingly
- When summarising PDFs, always read them; never paraphrase from training data

---

## Decision-Making Heuristics

Validated across multiple rounds — treat as standing rules unless new data contradicts them:

1. **Ideal points drift every period** — R&D targets should lead the ideal point by 2–3 periods, not chase today's position
2. **Advertising experiment every round** — if +20% spend yields negative contribution delta, cut budget; if valid experiment data is unavailable (e.g. stockout), note this explicitly
3. **Commercial team ROI is high** — expand headcount until experiment shows diminishing returns; current experiment: TOPS +$888K, TONE +$447K per +10 FTE/channel
4. **Production planning** — in a growing market, plan at the upper edge of expected demand; lost sales from the ±20% cap are very costly
5. **Price changes** — never exceed 30% per period; high-end segments use price as a quality signal; Savers/Shoppers are price-sensitive
6. **R&D budget sizing** — Feasibility Study ($100K, 1 period, precise) for large Vodite projects; Online Query (instant, ~15% overestimate, max 5/period) for Sonite tweaks
7. **Experience curve** — unit cost drops ~15% each time cumulative production doubles; first batch <100K incurs a 15% cost penalty
8. **Perceptual objectives** — use MDS targets whenever MDS data has been purchased; select "No Objectives" only when the relevant market's MDS data is unavailable (e.g. Vodite in launch period)

---

## Final Report Writing

**Due:** 8 June 2026, 16:00 BST. Max 2,000 words (cover page, bibliography, ToC, appendices excluded).
**Marking:** 40% structure/readability + 60% quality of argument. Performance rank does not matter; understanding does.

**Log after each round** (this feeds the report):
- 2–3 key decisions + reasoning + data source
- Predicted outcome → actual outcome → variance analysis (variance = highest-value content)

**Frameworks to apply:**
- BCG Matrix — brand lifecycle across 6 periods
- STP — segment targeting and positioning evolution
- Diffusion of Innovation / Rogers — Vodite entry timing
- Experience Curve — cost reduction logic
- Scenario Planning — cite Schoemaker (1995) for long-horizon decisions
- Porter's Five Forces — Sonite vs Vodite competitive dynamics

---

*Schema 版本：v1.1 — 2026-07-28*
*v1.1 变更：新增 OKF frontmatter（type: Operating Rules），配合全库 OKF（Open Knowledge Format v0.2）改造；约定见根 `CLAUDE.md`「OKF 知识格式约定」+ `.claude/okf-convention.md`。正文规则一字未改。*
*v1.0 初版：项目级 Claude 操作规则*
