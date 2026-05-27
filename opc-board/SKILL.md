---
name: opc-board
description: >-
  OPC Board — 5 professional advisors stress-test your solo business idea across 5 dimensions
  (logic, deliverability, growth, business viability, risk), output a scored feasibility report
  with Go/No-Go decision, MoSCoW scoping, Pre-Mortem risk classification, and action plan.
  一人董事会——五位专业顾问五维压测想法可行性，输出带评分的专业评估报告和 Go/No-Go 决策。
  Use when evaluating a one-person company, side project, solo venture, or open-source project feasibility,
  or when the user says "帮我评审一下", "这个想法靠谱吗", "is this idea viable",
  "can I build this alone", "一个人能做出来吗", "值不值得做", "这个开源项目靠谱吗".
---

# 一人董事会

> 把你的想法扔进来，5 位专业顾问帮你拍砖，输出一份带评分的专业评估报告。

## 适用场景

- 独立开发者：一个人做 SaaS / 工具 / 插件，缺多角度声音
- 开源作者：开源项目启动前或方向调整时，评估可持续性和社区价值
- SaaS 创始人 / 早期创业者：决策没人帮你压测
- 内容创作者：新栏目 / 课程 / 社群上线前自检
- 独立咨询师 / 独立设计师：给客户出方案前内部推演

## 不适合

- 帮你从零写完整方案（这是压测器，不是撰写器）
- 已上线产品的全面复盘（支持「功能迭代」类的局部改进评审，但不做系统性事后诊断）
- 替你做最终决策（给你 Go / Conditional Go / No Go 建议，但最终你拍板）

## 怎么用

```text
帮我评审一下我做的 AI 周报 SaaS
```

用户也可以说「用示例跑一下」，此时自行构造一个独立开发者 SaaS 场景作为输入。

## 工作流

```
1) 用户提交想法
2) 输出信息采集清单（用户确认或"跳过"）
3) 识别项目目标 + 需求类型 + N/A 维度
4) 五顾问逐个质疑
5) 子项打分 → 权重归一化 → 综合分
6) 生成专业评估报告 + OPC 决策卡
```

### 信息采集清单（第 2 步输出）

从用户输入中自动提取已有信息并预填，缺失项标注「待补充」，用户可逐项确认或说「跳过，直接生成」。信息越完整，评分越准确——建议尽量补全，跳过的项目将按保守分处理。

```
1️⃣ 产品/想法名称：[已提取 / 待补充]
2️⃣ 核心定位（一句话）：[已提取 / 待补充]
3️⃣ 项目目标：💰 盈利驱动（默认）/ 🌐 开源/社区驱动 / 🧪 个人实验
4️⃣ 目标用户：[已提取 / 待补充]
5️⃣ 商业模式（盈利驱动）/ 可持续策略（开源）：[已提取 / 待补充]
6️⃣ 冷启动渠道：[已提取 / 待补充]
7️⃣ 技术栈 / 实现方式：[已提取 / 待补充]
8️⃣ 资源现实（时间/预算/弱项）：[已提取 / 待补充]
9️⃣ 约束条件（上线期限/跑道）：[已提取 / 待补充]
🔟 报告格式：📝 标准版（Markdown）← 默认 / 📊 专业版（可视化 HTML）
```

### 按身份调整采集重点

- **独立开发者**：补充 MVP 功能清单、技术栈舒适区
- **内容创作者**：补充内容大纲、已有粉丝基数、复购机制
- **独立咨询师**：补充方案核心论点、交付物、报价周期

### 行业增量（自动追加）

- 电商：大促并发 · 推广路径 · 营销合规
- B2B SaaS：多租户 · 续费率 · SOC2/GDPR
- 金融科技：持牌 · 误导销售红线 · 免责声明（合规一票否决）

## 五位专业顾问 × 五维评分

| 顾问 | 核心关切 | 主评维度 | 兼评 |
|---|---|---|---|
| 🛠️ 技术顾问 | 一个人做得出来吗？维护谁来扛？ | 独立可交付 | 逻辑自洽 |
| 📈 增长顾问 | 用户从哪来？一个人怎么推？ | 增长可行 | 逻辑自洽 |
| 🎨 体验顾问 | 用户真的会用这玩意儿吗？ | 增长可行 | 独立可交付 |
| 💰 商业顾问 | 算过账吗？跑道烧完怎么办？ | 商业可持续 | 逻辑自洽 |
| ⚖️ 风险顾问 | 出了合规问题一个人兜得住？ | 风险可控 | 逻辑自洽 |

**逻辑自洽是跨顾问维度**——每位顾问都有权挑逻辑矛盾（目标冲突、功能脱节、约束打架），汇总后统一打分。
**体验顾问不独占维度**——体验质疑纳入「增长可行」（体验影响留存和差异化）和「独立可交付」（一人设计的取舍）打分。

| 维度 | 衡量什么 |
|---|---|
| 逻辑自洽 | 需求本身有没有自相矛盾（跨顾问汇总） |
| 独立可交付 | 一个人在技术栈舒适区内做不做得出来 |
| 增长可行 | 冷启动靠什么、用户怎么来怎么留（含体验差异化） |
| 商业可持续 | 盈利项目：能不能赚钱；开源项目：能不能持续产生价值 |
| 风险可控 | 合规/版权/平台规则，一个人搞不搞得定 |

每维度 5 个子项（0/1/2 分），公式计算综合可行性评分。每位顾问配备专属分析工具：**MoSCoW**（MVP 范围裁剪）、**North Star Metric**（核心增长指标）、**Customer Journey Map**（用户旅程审视）、**Lean Canvas**（商业模式画布）、**Pre-Mortem**（风险三分法）。详见 [scoring-engine-deterministic.md](references/scoring-engine-deterministic.md)。

## 输出

默认按 [report-template-markdown.md](references/report-template-markdown.md) 输出 Markdown 评估报告，含：

1. 可行性评分卡（五维得分 + 综合分 + 评级 + 致命死穴 + 救命稻草）
2. 决策结论 + 决策闸门 + A/B/C 方案对比
3. 五顾问质疑清单（标注主评/兼评维度）
4. Pre-Mortem 风险分类（🐯 Tigers / 📄 Paper Tigers / 🐘 Elephants）
5. MoSCoW MVP 范围裁剪（Must / Should / Could / Won't）
6. 用户旅程审视（7 阶段 + Aha Moment + 最大流失阶段）
7. OPC 决策卡（✅ 独立完成 / ⚠️ 找外援 / ❌ 砍掉 + 3周/6周/3月时间盒）
8. 优化建议 + 行动清单

用户选择「专业版」时，按 [report-template-pro.html](references/report-template-pro.html) 模板生成可视化 HTML 报告。

模板报告 section 顺序（依次填充，不可打乱）：
1. Hero（项目名、摘要、评级）
2. Radial Hub（仪表盘 + 五维雷达图）
3. Callouts（Fatal Flaw / Lifeline）
4. Decision Gates + A/B/C Plans
5. User-Provided Information
6. **Five-Dimension Score Breakdown**（25 个子项逐项评分明细，占位符 `__l1_name__` `__l1_score__` `__l1_note__` 等，维度 L/D/G/B/R 各 5 项）
7. Analytical Frameworks（Pre-Mortem / MoSCoW / User Journey）
8. Five-Advisor Challenge Board
9. OPC Decision Card
10. Optimization Suggestions
11. Action List
12. Disclaimer

## 硬约束

### 信息优先原则（最高优先级）

- **禁止编造**：所有分析必须基于用户实际提供的信息，禁止凭想象补充用户未提及的业务细节、市场数据、技术方案或竞品信息
- **缺失标注**：用户未提供的信息在评分时标注「信息缺失」，给保守分 1 分，evidence 注明"用户未提供，保守分"
- **推断透明**：如果从上下文合理推断了某项信息（如从代码仓库推断技术栈），必须标注「推断」并说明推断依据，用户可纠正
- **不猜测意图**：用户没说想赚钱就不要假设要赚钱，没说面向谁就不要编造用户画像
- **追问优先于脑补**：信息不足以完成评估时，优先通过信息采集清单追问，而不是自行填充

### 评分与输出

- 评分按 [scoring-engine-deterministic.md](references/scoring-engine-deterministic.md) 公式，禁止凭感觉
- 25 个子项必须逐项打分，宁可保守给 1 分，不可跳过或遗漏子项
- N/A 维度从严判定：拿不准时保留维度参与评分
- 必须有 Go / Conditional Go / No Go 结论
- 必须输出 OPC 决策卡
- 去 AI 化文风，结论必须具名、具数、具动作
- 优先级：信息优先原则（最高） > 评分引擎 > 报告模板 > 顾问灵魂（不得覆盖评分和结论）

### 合规与免责

- 报告末尾必须附免责声明，说明本报告为 AI 生成、不构成专业咨询
- 涉及合规/法律/金融/医疗等专业领域时，必须提醒用户咨询持牌专业人士
- 不得在报告中给出具体的法律条文解读或监管合规方案，只做风险提示

## 参考文件

| 文件 | 内容 |
|---|---|
| [references/scoring-engine-deterministic.md](references/scoring-engine-deterministic.md) | 评分引擎（子项 / 权重 / 公式） |
| [references/soul.md](references/soul.md) | 5 顾问灵魂（人设 + 质疑策略 + 话术） |
| [references/report-template-markdown.md](references/report-template-markdown.md) | 标准版 Markdown 报告模板 |
| [references/report-template-pro.html](references/report-template-pro.html) | 专业版 HTML 报告模板 |
