# Markstrat 决策框架（可复用模板）

> **用途：** 每轮决策前，用本文件作为结构化框架，确保不遗漏任何决策模块。
> **公司：** TITANS（代码 T）| **共 6 轮（Period 1–6）**
> **Decide 模块共 5 个：** R&D → Brand Portfolio → Marketing Mix → Commercial Team → Market Research

---

## 模块一：R&D（研发）

**入口：** Decide → Research & Development

### 可操作的四类动作

| 动作 | 触发条件 | 关键参数 |
|---|---|---|
| **新建 Sonites 项目** | 需要升级现有品牌规格，或为新品牌准备 platform | 项目名（PO开头）、5个物理属性、预算 |
| **新建 Vodites 项目** | 进入/扩展 Vodite 市场 | 项目名（PE开头）、5个物理属性、预算 |
| **新建降本项目（Cost Reduction）** | 现有 platform 尚未达到 minimum base cost | 选择目标 project，自动消耗一次 Online Query |
| **取消搁置（Unshelve）** | 有之前搁置的项目需要重新推进 | 确认剩余所需预算后分配资金 |

### Sonites 物理属性范围

| 属性 | 最小值 | 最大值 | 感知影响 |
|---|---|---|---|
| Features（#） | 5 | 20 | 弱（次要） |
| Design（Index） | 3 | 10 | Convenience 感知（强） |
| Battery（Hour） | 24 | 96 | Convenience 感知（次要） |
| Display（Inch） | 4 | 40 | Performance 感知（次要） |
| Proc. Power（GFlops） | 5 | 100 | Performance 感知（强） |

### Vodites 物理属性范围

| 属性 | 最小值 | 最大值 |
|---|---|---|
| Resolution（L/mm） | 20 | 100 |
| Energy（BC/Wh） | 10 | 100 |
| Carbon Footprint（Kg） | 5 | 50 |
| Connectivity（Index） | 3 | 10 |
| Apps（Number of） | 5 | 100 |

### R&D 预算模式

- **Budget allocated this period**：本期分配资金，项目可能完成也可能不完成
- **Initiate a Feasibility Study**：花 $100K，下期返回精确的完成所需预算（推荐用于 Vodite 大项目）
- **Online Query**：免费即时估算（~15% 高估），每期最多 5 次（用于 Sonite 小调整）
- **降本项目**：点击 Create 自动消耗一次 Online Query

### 本期（Period 4）R&D 状态

| 项目 | 状态 | 用途 | Base Cost | Min Cost |
|---|---|---|---|---|
| POTONECRP3 | ✅ 完成 | TONE 当前 platform | $65 | $65（已达最低）|
| POTOPS | ✅ 完成 | TOPS 当前 platform | $172 | **$154（可降本）** |
| POSHOP | ✅ 完成 | TOHO 当前 platform | $112 | $112 |
| PEINNO | ✅ 完成 | TERRA 当前 platform | $242 | TBD |
| PEINNOV | ⏸️ 搁置 | 另一 Vodite 项目 | — | 还需 $1,894K |

**⚠️ 每轮决策清单：**
- [ ] TOPS 是否需要启动降本项目（POTOPS $172 → $154）？
- [ ] TOPS 是否需要规格升级 R&D（应对 MOVE 的 Power 84 威胁）？
- [ ] TERRA / Vodite 是否需要新 R&D 项目（升级规格追 Adopters）？
- [ ] PEINNOV 是否值得取消搁置？

---

## 模块二：Brand Portfolio（品牌组合）

**入口：** Decide → Brand Portfolio

### 可操作的动作

| 动作 | 条件 | 说明 |
|---|---|---|
| **Maintain（维持）** | 默认，不做改动 | 品牌继续以当前 platform 运营 |
| **Modify（升级换 platform）** | 有新完成的 R&D 项目 | 切换 base project，下期生效；旧库存按原成本卖给贸易商 |
| **Withdraw（撤市）** | 品牌失去战略意义 | 慎用，不可恢复 |
| **Launch new Sonites brand** | 有完成的 Sonites R&D 项目 | 品牌名 TO开头（Titans 代码 T + O） |
| **Launch new Vodites brand** | 有完成的 Vodites R&D 项目 | 品牌名 TE开头（Titans 代码 T + E） |

### 当前品牌组合（Period 4 起）

| 品牌 | 市场 | 发布期 | Portfolio Role | Period 4 Base Project |
|---|---|---|---|---|
| **TONE** | Sonites | Period 0 | Savers 低价品 | POTONECRP3（已切换）|
| **TOPS** | Sonites | Period 0 | Professionals / High Earners 高端 | POTOPS |
| **TOHO** | Sonites | Period 3 | Shoppers 细分 | POSHOP |
| **TERRA** | Vodites | Period 4 | Innovators（首发）| PEINNO |

**⚠️ 每轮决策清单：**
- [ ] 各品牌是否需要切换 base project？（切换后旧库存清仓）
- [ ] 是否有新 R&D 完成、需要发新品牌？
- [ ] TOPS 是否需要 Modify 切换到升级后的 platform？

---

## 模块三：Marketing Mix（营销组合）

**入口：** Decide → Marketing Mix

> 每个品牌独立设置，包含 4 个子决策。

### 3.1 Production（生产计划）

- 填入**计划生产量（单位）**
- 系统自动调整范围：±20%（计划的80%～120%）
- 上期期末库存会在展示中标注

**生产计划原则：**
- 需求 > 供给：设为预期需求 ÷ 0.9（留 10% buffer 防缺货）
- 需求 < 供给：设为预期需求 × 1.05（轻微库存比缺货代价小）
- 连续缺货品牌：计划量至少是上期实际销量的 1.3 倍

**当前各品牌参考（Period 4）：**

| 品牌 | P3 实际销量 | P3 计划 | P3 结果 | P4 建议方向 |
|---|---|---|---|---|
| TONE | 185,522 | 240,000 | 过剩（下调 20%）| 计划 ~190,000–200,000 |
| TOPS | 141,754 | 180,000 | 过剩（下调 20%）| 计划 ~150,000–160,000 |
| TOHO | 60,000 | 50,000 | 爆仓（+20%仍售完）| 计划 **120,000+**（至少翻倍）|
| TERRA | — | — | 新品首发 | 待定（Vodite 市场规模参考 SESENEW） |

### 3.2 Price（价格）

- 填入**建议零售价（$）**
- 系统会显示竞品历史价格走势
- 每期价格变化不超过 30%（否则系统警告）
- Unit Margin 表格显示：Retail Price → Avg Selling Price → Unit Transfer Cost → Unit Margin

**当前各品牌价格（P3）及竞品参考：**

| 品牌 | P3 价格 | 主要竞品价格 | P4 建议 |
|---|---|---|---|
| TONE | $225 | ROCK: $200, MOST: $230, SOFT: $220 | ⚠️ ROCK 降价到 $200，研究是否跟降 |
| TOPS | $500 | SOLO: $499, ROLL: $499, MOVE: $575 | 维持 $500（高端信号）|
| TOHO | $235 | ROCK: $200, MOST: $230, SOFT: $220 | 维持或微调（Shoppers 价敏感）|
| TERRA | 待定 | SESENEW: $750, READ: $1,200 | 参考竞品定位，推荐 $800–$1,000 |

**Vodite 市场价格参考：**
- SESENEW（Snipers）：$750
- READ（Rocket）：$1,200
- TERRA 建议：若攻 Innovators，可定 $800–$900（比 SESENEW 略贵，比 READ 便宜）

### 3.3 Advertising（广告）

填入：
1. **广告媒体预算（Media budget，K$）**
2. **广告研究预算（Research budget，K$）**——建议为 Media 的 15%
3. **各细分市场分配比例（%）**——必须合计 100%

**广告分配原则（基于 Sonites）：**
- 主攻细分市场分配 60–80%
- 次要细分不超过 20%
- 不相关细分填 0%

**当前品牌广告细分定向（P3 实际）：**

| 品牌 | P3 Media | 分配方向 | P4 建议 |
|---|---|---|---|
| TONE | $1,270K | Savers 70%, Shoppers 25%, Explorers 5% | 维持，考虑增到 $1,500K（实验显示 +20% → +$316K 贡献）|
| TOPS | $1,270K | High Earners 55%, Professionals 35%, Explorers 10% | 恢复到 $1,500K+（P3 被砍后份额下降）|
| TOHO | $1,700K | Shoppers 90%, Explorers/Savers 各 5% | 维持高比例 Shoppers，考虑增到 $2,000K |
| TERRA | 待定 | Innovators 为主 | 参考 SESENEW：Innovators ~54%, Adopters ~32%, Followers ~14% |

**Vodite 广告细分（SESENEW P3 参考）：**

| 品牌 | Innovators | Adopters | Followers | Total |
|---|---|---|---|---|
| SESENEW | 1,150 (54%) | 680 (32%) | 310 (14%) | 2,140 |
| READ | 1,280 (66%) | 390 (20%) | 280 (14%) | 1,950 |

### 3.4 Perceptual Objectives（感知目标）

- **No objectives**：只提升知名度，不影响感知定位
- **Semantic Scales**：指定各属性的目标评分（1–7）
- **MDS**：指定在 Economy / Performance / Convenience 三维空间的目标位置

**使用规则：**
- 新品牌（如 TERRA）：建议先设 No objectives，第一期主要建立知名度
- 感知偏离目标细分 ideal point 较远时：才需要设定 MDS 目标
- 通过 R&D 改变规格才能真正移动感知位置；广告感知目标只是辅助微调

---

## 模块四：Commercial Team（商业团队/销售力量）

**入口：** Decide → Commercial Team

### 填写格式

| 品牌 | Specialty Stores | Mass Merch. | Online Stores | TOTAL |
|---|---|---|---|---|
| TONE | ? | ? | ? | ? |
| TOPS | ? | ? | ? | ? |
| TOHO | ? | ? | ? | ? |
| TERRA | ? | ? | ? | ? |
| **TOTAL** | | | | |

### 渠道分配原则

渠道分配应与**目标细分的购物习惯**匹配：

**Sonites 各细分购物渠道偏好（P3 数据）：**

| 细分 | Specialty | Mass Merch. | Online |
|---|---|---|---|
| Savers | 26% | **61%** | 13% |
| High Earners | **48%** | 30% | 22% |
| Professionals | **54%** | 23% | 23% |
| Shoppers | **42%** | 42% | 16% |
| Explorers | **71%** | 12% | 17% |

**Vodites 各细分购物渠道偏好（P4 新数据）：**

| 细分 | Specialty | Mass Merch. | Online |
|---|---|---|---|
| Innovators | **76%** | 11% | 13% |
| Adopters | **63%** | 18% | 18% |
| Followers | 36% | **41%** | 23% |

### 销售人员分配策略

- **TONE（攻 Savers）**：重点 Mass Merch.（Savers 61% 在此购买）
- **TOPS（攻 Professionals/High Earners）**：重点 Specialty Stores
- **TOHO（攻 Shoppers）**：Specialty + Mass Merch. 均衡分配（各 42%）
- **TERRA（攻 Innovators）**：重点 Specialty Stores（Innovators 76%）

### 销售团队实验数据参考（P3，每渠道 +10 人的贡献增量）

| 品牌 | 贡献增量 | 建议方向 |
|---|---|---|
| TOPS | +$888K | 积极扩张 |
| TONE | +$447K | 适度扩张 |
| TOHO | −$248K | ⚠️ 不扩张（因 P3 产能不足数据无效） |

**⚠️ 每轮决策清单：**
- [ ] 根据品牌目标细分的购物渠道习惯分配销售人员
- [ ] 参考 Commercial Team Experiment 数据判断扩张 ROI
- [ ] TERRA（Vodites）：Innovators 主要在 Specialty，重点投入该渠道
- [ ] 注意：增员有招聘成本（$3,443/人），减员有解雇成本（$5,739/人）

---

## 模块五：Market Research Studies（市场调研购买）

**入口：** Decide → Market Research Studies

### 通用研究（所有市场）

| 研究 | 费用 | 用途 |
|---|---|---|
| Industry Benchmark | $34,500 | 竞品完整 P&L、各品牌规格、SPI 排名 |

### Sonites 市场研究（每期价格）

| 研究 | 费用 | 决策用途 | 优先级 |
|---|---|---|---|
| Consumer Survey | $68,750 | 品牌知名度、购买意向、购物习惯 | ⭐⭐⭐ 必买 |
| Consumer Panel | $114,750 | 市场份额（量 + 值）、渠道销量分布 | ⭐⭐⭐ 必买 |
| Semantic Scales | $11,500 | 品牌感知属性评分 + 各细分理想值 | ⭐⭐⭐ 必买（便宜）|
| Multidimensional Scaling | $40,250 | 3D 感知地图，判断品牌感知位置 | ⭐⭐ 推荐 |
| Market Forecast | $23,000 | 各细分未来 5 期增长预测 | ⭐⭐ 推荐 |
| Competitive Advertising | $34,500 | 竞品广告投入和细分分配 | ⭐⭐ 推荐 |
| Distribution Panel | $68,750 | 渠道覆盖率、铺货门店数 | ⭐ 按需 |
| Advertising Experiment | $28,750 | +20% 广告对贡献的边际影响 | ⭐⭐ 推荐（每轮运行）|
| Commercial Team Experiment | $40,250 | +10人/渠道对贡献的边际影响 | ⭐⭐ 推荐（每轮运行）|
| Competitive Commercial Team | $17,250 | 竞品销售人员规模 | ⭐ 按需 |

### Vodites 市场研究（每期价格）

| 研究 | 费用 | 用途 | 优先级 |
|---|---|---|---|
| Consumer Survey | $46,000 | Vodite 各细分知名度、意向 | ⭐⭐⭐ TERRA 上市后必买 |
| Consumer Panel | $80,250 | Vodite 市场份额 | ⭐⭐⭐ 必买 |
| Semantic Scales | $11,500 | Vodite 感知 + 理想值 | ⭐⭐ 推荐 |
| Multidimensional Scaling | $40,250 | Vodite 感知地图 | ⭐⭐ 推荐 |
| Market Forecast | $23,000 | Vodite 各细分增长预测 | ⭐⭐ 推荐 |
| Competitive Advertising | $34,500 | 竞品 Vodite 广告投入 | ⭐⭐ 推荐 |
| Distribution Panel | $57,500 | Vodite 渠道铺货 | ⭐ 按需 |
| Advertising Experiment | $28,750 | Vodite 广告边际效益 | ⭐ 按需 |
| Commercial Team Experiment | $40,250 | Vodite 销售团队边际效益 | ⭐ 按需 |
| Competitive Commercial Team | $17,250 | 竞品 Vodite 销售团队 | ⭐ 按需 |

### 推荐每期标配购买清单（预算参考 ~$450K）

```
必买（约 $350K）：
☑ Industry Benchmark          $34,500
☑ Sonites Consumer Survey      $68,750
☑ Sonites Consumer Panel      $114,750
☑ Sonites Semantic Scales      $11,500
☑ Sonites Market Forecast      $23,000
☑ Sonites Advertising Exp.     $28,750
☑ Vodites Consumer Survey      $46,000  ← Period 4 起 TERRA 上市后加入
☑ Vodites Consumer Panel       $80,250  ← Period 4 起加入

推荐追加（约 $100K）：
☑ Sonites MDS                  $40,250
☑ Sonites Competitive Adv.     $34,500
☑ Sonites Comm. Team Exp.      $40,250
```

---

## 决策顺序建议（每轮流程）

```
Step 1: 阅读市场调研数据（本轮新数据）
         ↓
Step 2: R&D 决策
         — 是否启动新项目？
         — 是否做降本项目？
         — 分配各项目预算
         ↓
Step 3: Brand Portfolio 决策
         — 品牌是否切换 base project？
         — 是否发新品牌？
         ↓
Step 4: Marketing Mix 决策（每个品牌）
         — 生产计划（先算需求预测）
         — 定价（参考竞品）
         — 广告预算 + 细分分配
         — 感知目标
         ↓
Step 5: Commercial Team 决策
         — 按细分购物习惯分配渠道人员
         — 参考 Experiment 数据判断扩张幅度
         ↓
Step 6: Market Research Studies 购买
         — 按预算选择研究项目
         — 确保下期有足够数据支撑决策
         ↓
Step 7: 提交前核查
         — 预算是否超支？
         — TOHO/TERRA 是否仍会缺货？
         — 广告分配比例是否合计 100%？
```

---

## 附录：关键约束和规则

| 规则 | 说明 |
|---|---|
| 生产计划范围 | 系统自动调整 ±20%（实际产量在计划的 80%–120% 之间）|
| 价格变化上限 | 单期不超过 30%，否则系统警告 |
| 广告分配合计 | 各细分百分比必须合计 100% |
| R&D Online Query | 每期最多 5 次（Sonites + Vodites 合计）|
| 品牌命名 | Sonites 品牌 TO 开头，Vodites 品牌 TE 开头 |
| Base cost 最低值 | Sonites ≥ $25，Vodites ≥ $30（Handbook 规定，Challenge PPT 错误）|
| 经验曲线 | 累计产量每翻倍，转移成本降约 15%；首批 <100K 有 15% 成本惩罚 |
| 贷款影响 | P4 起每期须偿还 $2,119K（本金 $1,779K + 利息 $340K）|
| 通胀影响 | P4 通胀 4%（vs P3 的 2%），所有 base cost 会相应提高 |

---

*文件创建：2026-05-15 | 适用范围：Round 4–6*
