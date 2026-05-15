# Markstrat — Key Parameter Reference (考试 & 报告速查)

> 来源：交叉对比 `Participant-Handbook.pdf`（StratX 官方手册，权威）与 `Markstrat7_Challenge1_MS7-SM-B2C-DG.pdf`（介绍 PPT）。两者冲突时以 Handbook 为准。
>
> **冲突标记 ⚠**：Challenge PPT 把 Sonite/Vodite 的 base cost 最低写成 \$10；Handbook 是 **Sonite ≥\$25 / Vodite ≥\$30**。课程实际用 Handbook 数字。

---

## 1. 模拟世界（The Markstrat World）

| 项目 | 数值 / 说明 | 来源 |
|---|---|---|
| 总人口 | **80 million** inhabitants | Challenge p.5 |
| 地理分布 | 40% top-5 大城市 / 25% 小型 urban / 35% rural | Challenge p.5 |
| 通胀率 | 2% | Handbook p.7 |
| GNP 增长 | 4% | Handbook p.7 |
| 货币 | Markstrat Dollar (\$) | Challenge p.5 |
| 每行业最多公司数 | 最多 **6 家** (firm code: L / M / N / R / S / T) | Challenge p.5 / Handbook |
| 决策回合数 | 每年 1 round；课程共 6 rounds (Period 1–6) | Coursework brief |
| 起始品牌 | 每家公司开局 **2 个 Sonite 品牌**，0 个 Vodite | Handbook §II.1, §III.2 |
| 每类别品牌上限 | 同时最多 **5 个 Sonite + 5 个 Vodite** | Challenge p.6 |

---

## 2. Sonite 产品（已上市）

### 5 个物理属性

| 属性 | 缩写 | 单位 | 范围 |
|---|---|---|---|
| Processing Power | Power | GFLOPS | **5 – 100** |
| Display Size | Display | inches (") | **4 – 40** |
| Design Index | Design | index | **3 – 10** |
| Battery Life | Battery | hours (h) | **24 – 96** |
| Number of Features | Features | count | **5 – 20** |
| Base Unit Cost | Base Cost | \$ | **≥ \$25** ⚠ |

### Sonite 5 个消费者细分（Segments）

| 代码 | 名称 | 关键诉求 | 价格敏感度 | 典型规模 |
|---|---|---|---|---|
| **Ex** | Explorers | 高性能（Power、Display），不太在乎便利性 | 高 | 中 |
| **Sh** | Shoppers | 高性价比、参数对比 | 高 | 中 |
| **Pr** | Professionals | 高质量 + 易用，price 当作 quality signal | 低 | 中 |
| **Hi** | High Earners | 性能 + 便利 + 状态象征 | 低 | 较小 |
| **Sa** | Savers | 便宜、低性能、平均便利 | 极高 | **最大**，未来增长可能超预期 |

### Sonite MDS 感知图（Perceptual Map）

3 个维度：**Economy × Performance × Convenience**（一次只能可视化 2 维）。坐标范围 **−20 ~ +20**。Period 0 起即可购买，含 200 名受访者数据。

---

## 3. Vodite 产品（开局尚未上市）

### 5 个物理属性

| 属性 | 缩写 | 单位 | 范围 |
|---|---|---|---|
| Resolution | Resolution | LPM | **20 – 100** |
| Energy Efficiency | Energy | bC/Wh | **10 – 100** |
| Carbon Footprint | Carbon | kg CO₂ | **5 – 50** |
| Connectivity | Connect | index | **3 – 10** |
| Apps | Apps | count | **5 – 100** |
| Base Unit Cost | Base Cost | \$ | **≥ \$30** ⚠ |

> **Carbon Tax**：根据 instructor 选定的 scenario，可能对 Carbon Footprint 高于某阈值的 Vodite 征税。会**提前 1–2 年通知**，作为 exceptional cost 出现，**金额固定，与销量无关**。

### Vodite 3 个消费者细分（Rogers 创新扩散）

| 代码 | 名称 | 收入 | 行为特征 |
|---|---|---|---|
| **In** | Innovators | 高于平均 | 第一批尝鲜，敢冒风险；初期最大群体，但占总人口比例小 |
| **Ad** | Early Adopters | 平均 | 意见领袖，对扩散最关键；不能忽视 |
| **Fo** | Followers | 低于平均 | 真正的市场主体，需要他人先验证才购买 |

### Vodite 特殊规则

- 首个 Vodite prototype 需要 **\$5–10M** R&D 投入。
- **Vodite 的 MDS map 在有品牌之前不可用** ⇒ 早期入场者是"盲飞"。
- Sonite 与 Vodite 互不替代、互不互补、互相独立。

---

## 4. 渠道（Distribution Channels）

| 渠道 | 门店数 | 分销商 margin | 平均促销折扣 | 典型产品 |
|---|---|---|---|---|
| **Specialty Stores** | ~10,000 | **40%** | 0% | 高端、Vodite 优先渠道 |
| **Mass Merchandisers** | ~6,000（6 chains） | **30%** | **10%** | 低价低性能 |
| **Online Stores** | ~1,000 | **30%** | **5%** | 增长中，方便比价 |

### 价格 → 单位贡献样例（retail \$400, 转移成本 \$123）

| 项目 | Specialty | Mass Merch | Online |
|---|---|---|---|
| 实际零售价 | \$400 | \$360 | \$380 |
| 分销 margin | 40% = \$160 | 30% = \$108 | 30% = \$114 |
| Selling price | \$240 | \$252 | \$266 |
| Transfer cost | \$123 | \$123 | \$123 |
| **Unit contribution** | **\$117** | **\$129** | **\$143** |

---

## 5. 每轮决策（Tactical Decisions per Period）

### A. 生产计划（Production Plan）

- 系统会根据实际需求**自动 ±20% 调整**你的生产计划。
- 超过 ±20% → 要么 lost sales，要么累积 inventory。
- Inventory holding cost = 单位库存 × transfer cost × % (在 Newsletter 公布)。
- 库存处置（产品下架时）有 disposal loss。

### B. 定价（Pricing）

- 你设的是 **Recommended Retail Price**。
- **变动幅度 > 30%/period** 系统会警告，过激会被自动校正回。
- 反倾销：所有渠道下，selling price 必须 > transfer cost。

### C. 广告（Advertising）

- 拆成两块：**Media** 预算（买曝光）+ **Research** 预算（提升说服力）。
- 维持知名度：research 占 **4–8%**。
- 重新定位：research 占 **10–15%**。
- 必须设定 **Segment allocation**：% 加总 = 100%。
- 必须设 **perceptual objective**（如强调"性能"或"便利性"）。
- **Share of voice**（你 / 行业总广告费）很关键，新品发布或重新定位通常需要高于竞争对手。

### D. 商务团队（Commercial Team）

- 决策粒度：**FTE × brand × channel** 矩阵。
- 跨渠道/跨品牌**调动免费**，但**净 hire/fire 有成本**（按 FTE 成本的 % 收取）。

### E. 市场调研（Market Research Studies）

共 **12 种**，但 **Period 0 报告里只能买 4 种**：
1. Consumer Survey
2. Consumer Panel
3. Distribution Panel
4. Market Forecast

剩余 8 种 Period 1+ 起可买：Semantic Scales / MDS / Conjoint Analysis / Competitive Advertising estimates / Competitive Commercial Team estimates / Industry Benchmarking / Advertising Experiment / Commercial Team Experiment.

> **三大诊断研究的优先顺序**（写报告必引）：
> 1. **Semantic Scales**：设计 R&D 项目（与物理属性一一对应）
> 2. **MDS**：定义战略与传播（提供 3D 感知图 + segment ideal points）
> 3. **Conjoint Analysis**：验证以上两者，量化各属性 utility

### F. R&D 项目

| 规则 | 数值 |
|---|---|
| 每期上限 | 5 个 Sonite + 5 个 Vodite |
| 项目命名 | 第一字母 P；第二字母 O (Sonite) 或 E (Vodite)；总长 ≤ 8 |
| Sonite 升级预算 | 几十万 ~ 200 万美元 |
| Vodite 首版预算 | **\$5–10M** |
| **Feasibility Study** | **\$100k**，需 **1 period**，结果精准 |
| **Online Query** | **即时**，但**高估约 15%**（Vodite 可能更多）；**每期最多 5 次** |
| 完成判定 | 分配预算 ≥ 实际所需 → 下个 period 可用；如果"略低"，仍可能完成；远低则失败，可下期补完或搁置 |
| 名称重用 | **完成的项目名不可再用**（即便只是小改） |

### G. 学习曲线 / 成本下降（Productivity Gains）

- **每累计产量翻倍 → 单位成本下降约 15%** （experience curve）
- 首个生产批次 < 100,000 单位 → transfer cost **比 base cost 高 ~15%**
- 可发起 **Cost Reduction R&D project**（同规格、低 base cost）→ 一段时间后总成本曲线低于原曲线
- 通胀会侵蚀部分 cost reduction

---

## 6. 财务 & 预算

| 项目 | 数值 / 规则 |
|---|---|
| 营销部门预算 | 上一期 net contribution 的 **40%** |
| 预算上下限 | **\$7M – \$20M**（按通胀调整） |
| 超支处理 | Finance Control 会自动砍预算，**先砍广告** |
| 未花完预算 | **不滚存**到下一期 |
| Loan | Instructor 可能授予；本金当期到账，利息当期付，本金从 P+1 起还 |

### P&L 结构（自上而下）

```
Revenues  =  units sold × avg selling price
−  COGS  =  units sold × transfer cost
−  Inventory costs  =  holding cost + disposal loss
=  CBM  (Contribution Before Marketing)
−  Advertising media + research
−  Commercial team costs
=  CAM  (Contribution After Marketing)
−  Market research studies
−  R&D budgets
−  Interest paid
−  Exceptional cost / profit (e.g. brand withdrawal, carbon tax)
=  Net Earnings  (= EBT)
```

---

## 7. 评分（Share Price Index, SPI）

SPI 综合 4 项：
1. Net contribution generated
2. Brand market shares
3. Revenue growth
4. Quality of completed R&D projects

课程评分（performance 部分占 30%）：
- 50% × 你和 industry 内 4 队的相对 SPI
- 50% × 你和所有 industry 的相对 SPI

> **Coursework brief 强调**："Performance does not matter; understanding matters." → 报告（70%）才是关键，可以业绩平庸但分析深刻。

---

## 8. 报告会用到的高杠杆框架

| 框架 | 适用场景 |
|---|---|
| **STP** (Segmentation–Targeting–Positioning) | 直接对应 Markstrat 的 segment + ideal point |
| **BCG Matrix** | 6 年里 brand 从 Question Mark → Star → Cash Cow → Dog 的迁移 |
| **Diffusion of Innovation (Rogers)** | Vodite 的 In → Ad → Fo 完美对应 |
| **First-Mover Advantage / Disadvantage** | Vodite 进入时机决策 |
| **Porter's Five Forces** | Sonite vs Vodite 竞争结构对比 |
| **NPV / Cash Flow at Risk** | 论证 R&D 投资是否值得 |
| **Experience Curve (BCG/Henderson)** | 解释 cost reduction R&D 的逻辑 |
| **Scenario Planning (Schoemaker 1995)** | 报告必引的理论文献 |

---

## 9. 速记口诀（决策时反复检查）

1. **Period 1 不要乱动**：先读数据，建立 baseline 认知。
2. **看 ideal point 走向，定位未来 2–3 个 period**（不是今天）。
3. **每次大动作（升级/新品/定价跳变）前问：share of voice 够不够？**
4. **Cost reduction R&D 经常被低估** → Cash Cow 阶段必做。
5. **多品牌 vs 单品牌**：多品牌建壁垒但会 cannibalize。
6. **不要 over-invest 于已经高 awareness 的品牌**（边际递减）。
7. **每一轮结束写决策日志**：决策 → 数据依据 → 预测 → 下轮的实际结果与差异。**差异是报告的金矿。**
