---
type: Operating Rules
title: "Markstrat Coursework — Briefing for Claude"
description: "给后续 Claude 会话的 Markstrat 作业完整背景：课程、评分构成、模拟机制、团队分工。"
tags: [coursework, how-to, Markstrat, 商业模拟, 帝国理工, 考核构成, 会话背景交接, 模拟机制, 怎么打这个模拟, SPI]
status: stable
---

# Markstrat Coursework — Briefing for Claude

> **Purpose of this file:** Persistent context for any future Claude session helping Teemo with the *Corporate Strategy and Economics Simulation* coursework at Imperial College Business School. Read this first before answering questions about the project.

---

## 1. The Task in One Paragraph

Teemo is a student on the ESB programme at Imperial College Business School, taking the **Corporate Strategy and Economics Simulation** module taught by Associate Professor **Sven Mikolon**. The module uses **Markstrat** — a marketing strategy simulation built by INSEAD professors Larréché & Gatignon and published by StratX. Teemo and 2–3 teammates manage the marketing department of a fictional consumer-electronics company for **6 simulated years (rounds)**, competing against 3 other teams in the same industry. The objective is to **maximise the company's Share Price Index (SPI)**.

Assessment:
- **30%** — Markstrat performance (50% relative-to-industry SPI score, 50% relative-overall SPI score)
- **70%** — Final group report, max **2000 words**, due **8 June 2026, 16:00 BST** via Insendi

Lecture & coaching schedule (4 lectures + 4 drop-ins) runs from late April through 22 May; decision rounds I–VI run from 1 May to 22 May.

---

## 2. The Fictional World — What They Actually Sell

Markstrat invents two product categories with **made-up names** so students can't fall back on real-world brand intuitions. They are *not* real products.

### Industry context (constants of the simulated economy)
- **Population:** 80 million inhabitants. **Geography:** 40% top-5 urban / 25% smaller urban / 35% rural.
- **Inflation:** 2%/year. **GNP growth:** 4%/year. Stable — no major shocks anticipated.
- **Up to 6 firms per industry**, identified by firm code L / M / N / R / S / T. Teemo's industry has 4 teams (so 3 competitors). Industries are run in parallel for relative-SPI grading.
- **Brand cap:** each firm may market at most **5 Sonite + 5 Vodite brands** at a time.

### Sonites — the established product
Think of them as a generic stand-in for **laptops / tablets / digital cameras** — a mature consumer-electronics category. Five physical attributes drive everything:

| Attribute | Range | Unit |
|---|---|---|
| Processing Power | 5–100 | Gflops |
| Display Size | 4–40 | inches |
| Design Index | 3–10 | index |
| Battery Life | 24–96 | hours |
| Number of Features | 5–20 | count |
| Base Unit Cost | ≥$25 | $ |

Each team starts with **2 Sonite brands already on the market**.

### Vodites — the emerging product
A speculative future category — think AR glasses / Vision Pro / wearable / brain-computer interface. **Nobody is selling Vodites at game start.** Building the first prototype costs **$5–10M in R&D**. Five attributes:

| Attribute | Range | Unit |
|---|---|---|
| Resolution | 20–100 | LPM |
| Energy Efficiency | 10–100 | bC/Wh |
| Carbon Footprint | 5–50 | kg CO₂ |
| Connectivity | 3–10 | index |
| Apps | 5–100 | count |
| Base Unit Cost | ≥$30 | $ |

A carbon tax may apply to Vodites with Carbon Footprint above a threshold (depends on instructor's scenario settings). When applicable, you get **1–2 years' advance notice**, and the tax appears as an exceptional cost — **fixed amount, independent of sales volume**.

**Sonites and Vodites are independent markets** — no substitution, no complementarity.

### Brand naming convention
Brand names ≤6 chars. **1st letter = firm code** (L/M/N/R/S/T). **2nd letter = O for Sonite, E for Vodite.** Rest is free. So `MOST`, `MOVE` are M's Sonites; `MEGA`, `MEMO` would be M's Vodites. R&D project names start with `P` and follow the same pattern (e.g. `POMOST` is the R&D project underlying brand MOST).

---

## 3. Customer Segments — Who They Sell To

### Sonite segments (5 groups)
- **Explorers (Ex)** — tech enthusiasts, want high performance, price-sensitive (limited income).
- **Shoppers (Sh)** — comparison shoppers, want best price-quality ratio, average specs.
- **Professionals (Pr)** — use Sonites for work, want high quality + ease of use, price = quality signal.
- **High Earners (Hi)** — buy expensive products partly for status, want performance and convenience.
- **Savers (Sa)** — largest segment, price-conscious, low-performance products.

### Vodite segments (3 groups, classic diffusion-of-innovation curve)
- **Innovators (In)** — first adopters, adventurous, above-average income.
- **Early Adopters (Ad)** — opinion leaders, critical for diffusion, average income.
- **Followers (Fo)** — bulk of the market, adopt only after broad acceptance, below-average income.

### Distribution channels (3)
- **Specialty Stores** — ~10,000 outlets, 40% margin, high service, good for high-end & Vodites.
- **Mass Merchandisers** — ~6,000 outlets across 6 chains, 30% margin, low-end products, ~10% promo discount.
- **Online Stores** — ~1,000 outlets, 30% margin, ~5% promo discount, growing channel.

---

## 4. The Decisions Made Each Round

Every simulated year, the team submits decisions across these areas:

1. **Brand Portfolio** — launch / modify / withdraw / maintain each brand.
2. **R&D Projects** — up to 5 Sonite + 5 Vodite projects per period. Specify name, target attributes, target base cost, allocated budget. Use `Feasibility Study` ($100k, takes 1 period) or `Online Query` (instant but ~15% over-estimate, max 5/period) to size the budget.
3. **Marketing Mix per brand:**
   - Production plan (auto-adjusts ±20%; outside that → lost sales or inventory)
   - Recommended retail price (don't change >30% per period)
   - Advertising media budget + advertising research budget (4–8% on research for awareness; 10–15% for repositioning)
   - Segment allocation (% of ad budget per segment, must sum to 100%)
   - Perceptual objectives (for repositioning via advertising)
4. **Commercial Team** — FTEs allocated per brand × per channel matrix. Reallocation is free; net hiring/firing has cost.
5. **Market Research Studies** — purchase up to 12 study types (consumer survey, panel, semantic scales, MDS, conjoint, market forecast, competitive intel, experiments, etc.).

Marketing department operates as a profit centre. Budget ≈ 40% of prior period's net contribution, typically $7–20M. Unspent budget does NOT carry over.

---

## 5. The Three Critical Diagnostic Studies

When advising Teemo on positioning or R&D, lean on these three studies in this order:

| Study | Use it for |
|---|---|
| **Semantic Scales** | Designing R&D projects (1:1 mapping between scale dimensions and physical attributes) |
| **Multidimensional Scaling (MDS)** | Strategy & communication — gives a 3D perceptual map (Economy / Performance / Convenience for Sonites; coordinate scale **−20 to +20**) showing all brands and segment ideal points. **MDS for Vodites only becomes available once Vodite brands exist on the market** — early entrants navigate blind. |
| **Conjoint Analysis** | Validating findings from the other two — measures utility consumers attach to attribute levels and price |

**Ideal points drift slowly but consistently each period.** Position 2–3 periods ahead, not at today's ideal point — R&D takes ≥1 period and the market keeps moving.

---

## 6. How Performance Is Measured — SPI

Share Price Index combines:
- Net contribution generated
- Market share
- Revenue growth
- Quality of completed R&D projects

**Grade scoring:** distance of your team's SPI from the mean SPI within your industry (50%) and across industries (50%).

---

## 7. Strategic Guidance — Things Worth Remembering

These are heuristics from the handbook + general business-strategy frameworks. Treat as starting points, not gospel.

### Round 1 priorities
- Don't make dramatic changes in Round 1. **Read the data first.** Use the four available studies (Consumer Survey, Consumer Panel, Distribution Panel, Market Forecast) to understand: which segments are biggest/growing, where competitors are positioned, what your brands' awareness and purchase intentions look like.
- Note the segment ideal points and how far your existing brands are from them.

### Long-term strategy
- **Pick which segments you target deliberately.** Trying to serve everyone with everything is the most common losing strategy.
- **Vodite entry timing is a big decision.** First-mover advantage is real, but you need ~$5–10M in R&D plus marketing budget to support it. Going early can dominate Innovators; going late risks being locked out. The MDS perceptual map for Vodites only becomes available once brands exist there, so early entrants navigate blind.
- **Experience curve:** transfer cost drops by **~15% every time cumulative production doubles**. Penalty: if first production batch is **<100,000 units**, transfer cost is **~15% higher** than the project's base cost.
- **Cost-reduction R&D projects** are often under-used. Once cumulative production is high, launching a same-spec project at lower base cost can transform a brand's margins (it pushes you onto a new, lower experience curve).
- **Multi-brand strategy** — multiple brands targeting the same segment build barriers to entry but cannibalise each other; weigh the trade-off.
- **Don't over-invest in advertising for brands with already-high awareness** — diminishing returns. Use the Advertising Experiment study to find the sweet spot.

### Common pitfalls (the auto-feedback flags these too)
- Production plan way off → lost sales OR expensive inventory.
- Price set above what segment will bear → market share collapse.
- Repositioning attempted via advertising alone when distance is too large → wasted spend, need R&D.
- Commercial team mis-allocated to channels that don't match the segment's shopping habits.
- Single brand generates >70% of contribution → fragile portfolio.
- Targeting non-attractive (shrinking, low-margin) segments.

### Frameworks to cite in the final report
The brief explicitly rewards using ESB-programme strategy frameworks. Good candidates:
- **BCG Matrix** — classify your brands as Stars / Cash Cows / Question Marks / Dogs over the 6 years.
- **Porter's Five Forces** — analyse the Sonite vs Vodite competitive dynamics.
- **First-mover advantage** — particularly relevant to the Vodite entry decision.
- **SWOT** — for one or two pivotal moments.
- **Segmentation–Targeting–Positioning (STP)** — direct fit.
- **Cash flow at risk / NPV** — for justifying R&D investment decisions.
- **Diffusion of innovation (Rogers)** — Vodite Innovators → Early Adopters → Followers maps perfectly.

---

## 8. The Final Report — How To Win 70% of the Grade

**Length:** ≤2000 words, double-spaced, font 12. Cover page (title, stream, team #, names, word count) + bibliography + ToC are excluded from the word count. Appendices excluded.

**Marking:** 40% structure/readability/flow + 60% quality of arguments.

**Key principle from the brief:** *"Performance does not matter; understanding matters."* You can win the report even if your SPI was middling. You can lose it even with the best SPI if you can't explain why.

**Structure suggestion:**
1. **Executive summary / overall strategy** — what you set out to do and the rationale.
2. **Pivotal decisions** — pick 3–5 (e.g. "when to enter Vodite", "whether to upgrade brand X in Round 3", "the cost-reduction project for Y"). For each: situation → decision → mechanism → outcome → lesson.
3. **What went wrong** — the brief specifically says this is rewarded. Be honest about misreads. Tie failures back to specific data you missed or misinterpreted.
4. **Framework analysis** — apply 1–2 frameworks deeply rather than name-dropping five. BCG matrix snapshot at start vs end is a high-leverage move.
5. **Conclusion / what we'd do differently** — this is where causal reasoning shines.

**Habits to build during the simulation (so the report writes itself):**
- After every decision round, log:
  - The 2–3 main decisions made and the reasoning (one paragraph).
  - The data/study results that drove the reasoning.
  - Predicted outcome.
  - In the *next* round: actual outcome and variance from prediction. **The variance is gold for the report.**
- Screenshot the perceptual maps and brand contribution charts each period.
- Track the SPI trajectory and the contribution-by-brand trajectory.

---

## 9. Files in This Workspace

- `Session_1.pdf` — first lecture deck (course overview)
- `coursework_brief.pdf` — assessment criteria & deadline
- `Participant-Handbook.pdf` — the operational bible (StratX, INSEAD); Sonite/Vodite mechanics, decision flows, study interpretation. **Authoritative source — overrides any conflicting numbers elsewhere.**
- `Markstrat7_Challenge1_MS7-SM-B2C-DG.pdf` — official intro slide deck (35 pp). Same content as Handbook §I–§III but condensed and visual. ⚠ Note: it lists Sonite/Vodite Base Cost minima as $10 — **this is wrong**; trust the Handbook (Sonite ≥$25, Vodite ≥$30).
- `Markstrat_Key_Parameters.md` — single-page parameter reference for exam/report use, cross-checked from Handbook + Challenge deck.
- `Schoemaker_1995.pdf` — *Scenario Planning: A Tool for Strategic Thinking* (Sloan Management Review). Required theoretical reading; useful for justifying long-horizon decisions in the final report
- `Markstrat_Explained.html` — earlier explainer artifact (HTML)
- `CLAUDE_BRIEFING.md` — this file

---

## 10. Notes for Future Claude Sessions

- **Teemo's English is solid but not native. He is more comfortable with Chinese explanations** when concepts are unfamiliar — default to Chinese unless he explicitly asks for English.
- He had genuine confusion about what Sonite/Vodite are (they sound like real products but are intentionally fictional). When in doubt, **ground abstract concepts in concrete real-world analogues** (e.g. "Sonite ≈ laptop", "Vodite ≈ AR glasses", "MOST ≈ iPhone Pro").
- This is a team coursework — Teemo's individual decisions get pooled with teammates. Suggestions should consider that he needs to convince teammates, not just act unilaterally.
- The deadline (8 June 2026) is firm. As the simulation rounds happen weekly, time-sensitive advice (round-specific moves) is more valuable than abstract theory.
- When asked to summarise files, *read them* — don't paraphrase from memory of the handbook.
