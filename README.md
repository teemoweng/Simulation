# Markstrat Simulation · Team TITANS

> Imperial College Business School · ESB Programme · Corporate Strategy & Economics Simulation 2026
> Instructor: Sven Mikolon · Live hub: https://teemoweng.github.io/Simulation/
>
> **For future Claude sessions:** start by reading `CLAUDE.md` (workflow rules) → then this file (current state) → then the latest `round{N}/` folder.

---

## 🎯 Current Standing (end of Period 4)

| Rank | Firm | SPI | Δ vs Round 4 |
|---|---|---|---|
| 1 | Snipers | 1,912 | +196 |
| **2** | **Titans (us)** | **1,870** | **+331** ⭐ biggest gain |
| 3 | Rocket | 1,522 | +111 |
| 4 | Marvels | 1,357 | -81 |

**Gap to leader:** 42 SPI points · **Rounds remaining:** Round 5 (this round) + Round 6 (final).
**Next-period budget:** $18,700K (Round 5 authorized).

---

## 🏷️ Brand Portfolio (5 brands as of P5)

| Brand | Market | Segment | Status | Base Project | One-liner |
|---|---|---|---|---|---|
| **TONE** | Sonites | Savers | Cash Cow | POTONECRP3 | $13.2M CAM in P4; cost dropped to $56 |
| **TOPS** | Sonites | Pros / High Earners | Star | POTOPS | $25.6M CAM (62% of Sonites profit) |
| **TOHO** | Sonites | Shoppers | Growth | POSHOP | Awareness 19% but Shoppers share 27.9% (#1) |
| **TERRA** | Vodites | Innovators / Adopters | Defend | PEINNO | 47.6% Vodite share at launch |
| **TECHNO** | Vodites | Followers | New (P5) | PENT | Launched by Adith for portfolio diversification |

---

## 👥 Team

| Member | Phone | Working style |
|---|---|---|
| **Teemo (me)** | — | Heavy AI user · workflow / infrastructure / HTML guides |
| **Mary Rui Ma** | +852 | Heavy AI user, partners with Teemo on analysis |
| **Adith** (admin) | +44 | **Strategic keeper** — reviews AI output, makes judgment calls (e.g. launched TECHNO) |
| **Nathan Tob** | +32 | Role TBD |
| **Yousef** | +966 | Role TBD |

**Communication notes:**
- Default team language: English (Adith / Nathan / Yousef don't read Chinese)
- HTML deliverables for team: **English only**
- Markdown working docs: Chinese or English (Teemo's choice)
- Mary can read both

**Outstanding question:** What are PENT's physical specs? Adith hasn't shared them; TECHNO numbers in the P5 Decision Guide are inferred from $266 transfer cost + Followers intent. He's been given override authority via the guide's TECHNO tab.

---

## 📅 Schedule (all 2026)

| Date | Event |
|---|---|
| May 1 | Round 1 decisions submitted |
| May 8 | Round 2 submitted · Lecture 2 (R&D) |
| May 12 / 15 | Round 3 & 4 submitted |
| May 19 | Lecture 3 (review) |
| **May 20** | **Round 5 decision deadline** ← current |
| May 22 | Round 6 (final) decision deadline |
| May 26 | Lecture 4 (Champions Day) |
| **June 8 · 16:00 BST** | **Final Report due** (≤2,000 words · 70% of grade) |

---

## 📂 Repository Layout

```
Simulation/
├── README.md                ← this file (current state for any new session)
├── CLAUDE.md                ← workflow rules for Claude
├── index.html               ← public hub (GitHub Pages homepage)
├── reference/               ← Handbook, framework refs, Markstrat explainer (EN)
├── report/                  ← Final Report scaffolding (Report_Source_Material.md)
├── round1/ … round6/        ← per-round artifacts (see below)
└── og-image.png             ← social preview for the hub URL
```

**Standard files per round** (created across the round's lifecycle):
- `Round{N}_Final_Decisions.md` — what we actually submitted
- `Round{N}_Results.md` — P&L, market share, brand CAM
- `Round{N}_MarketResearch.md` — awareness, intent, semantic scales, forecast
- `Round{N}_Decision_Analysis.md` — internal 5-module reasoning (for next round)
- `Round{N}_Decision_Guide_EN.html` — fill-in guide for teammates (English)
- `Round{N}_Results_Analysis_EN.html` — English recap of last round (English)
- `round5/raw_reports/` — raw Markstrat system dumps (P4 end-of-period)

---

## 🧠 Standing Strategic Heuristics

(validated across rounds — see `CLAUDE.md` for fuller list)

1. **Ideal points drift every period** — R&D should target 2-3 periods ahead, not today
2. **Cost reduction R&D is the highest-ROI lever** — payback often < 2 months
3. **Don't cap your own production** — plan above expected demand; system will cap to ±20% anyway
4. **Allocate ads by experiment ROI, not equally** — Round 4 mistake was flat $1.31M per brand
5. **Production cap = 1.2× prior period production** for active brands
6. **Vodite has been a duopoly opportunity** (Titans + Snipers = 96% in P4); Round 5 adds Marvels MEME + Rocket READ, so it's now 4–5 player

---

## 🚀 Next-Session Quick-Start

When a new Claude session opens for **Round 5 results processing** (after submission), follow `CLAUDE.md`'s Session Kickoff Protocol:

1. Read **this README.md** (5 seconds for context)
2. Read **`CLAUDE.md`** (workflow rules)
3. Ask Teemo for `Round5_Final_Decisions.md` content (from DECISIONS REVIEW)
4. Collect raw Round 5 results data → save as `round5/Round5_Results.md`
5. Collect raw market research → save as `round5/Round5_MarketResearch.md`
6. Generate `Round5_Results_Analysis_EN.html` for team
7. Generate `Round6_Decision_Analysis.md` and `Round6_Decision_Guide_EN.html`
8. **Update `report/Report_Source_Material.md`** — fill in the "actual" cells for Round 5 predictions
9. Deploy: `git add` specific files (not `-A`!), commit, push to `main`

> ⚠️ **Don't use `git add -A`** — it once accidentally committed Obsidian local files (`clippings/`, `_obsidian_context.md`). `.gitignore` now covers them, but `git add <specific files>` is safer.

---

## 📊 Final Report Logistics

- **Due:** June 8, 2026, 16:00 BST · Insendi submission
- **Word limit:** 2,000 (excluding cover, ToC, appendices, references)
- **Marking:** 40% structure & readability + 60% quality of argument
- **Performance does NOT matter; understanding does** (from course brief)
- **Source material:** `report/Report_Source_Material.md` — pre-organized by framework, with predicted vs actual gaps logged per round

**Frameworks expected in the report:**
BCG Matrix · STP · Diffusion of Innovation · Experience Curve · Scenario Planning (Schoemaker 1995) · Porter's Five Forces · First-Mover Advantage

---

*Last updated: 2026-05-20 (after Round 5 prep, before Round 5 submission)*
