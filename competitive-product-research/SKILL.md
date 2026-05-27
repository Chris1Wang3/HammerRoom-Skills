---
name: competitive-product-research
description: >-
  Competitive product research skill for structured benchmarking and strategic differentiation.
  Uses an original dual-track method (experience benchmarking + strategic diagnostics),
  collects sufficient context via a structured checklist before analysis,
  then produces a source-traceable professional HTML report with actionable recommendations.
  竞品调研技能：采用原创双轨方法（体验对标 + 战略诊断），先通过信息采集清单收集充分上下文，再输出证据可溯源的专业 HTML 报告。
---

# 竞品调研（Competitive Product Research）

> 不是观点合集，而是带证据编号、可追溯、可执行的专业竞品分析报告。

## 适用场景

- 竞品调研 / 对标分析 / 行业对比
- 差异化策略 / 竞争格局 / 定位与定价判断
- SWOT / 波特五力 / PESTLE
- 评审前竞品材料准备 / 排期会支撑资料

## 不适合

- 不做无法验证的市场规模"拍脑袋估算"
- 不做只讲概念、不落动作的泛战略报告
- 不做绕过权限的抓取或任何违规采集
- 不替你做最终决策（给方向建议，拍板仍由你）

## 怎么用

```text
我们 App 发帖转化率只有 3%，对标小红书和 Instagram，分析首次发帖漏斗问题。
当前状态：右上角入口 + 空白编辑器 + 无自动存草稿。
```

用户也可以说「帮我做一下 XX 和 YY 的竞品调研」，技能会先输出信息采集清单确认后再生成报告。

## 工作流

```
1) 用户提交调研需求
2) 输出信息采集清单（用户确认或"跳过"）
3) 问题对齐 + 证据建库
4) 双轨分析引擎（体验对标 + 战略诊断）
5) 生成专业 HTML 报告
```

### 信息采集清单（第 2 步输出）

从用户输入中自动提取已有信息并预填，缺失项标注「待补充」，用户可逐项确认或说「跳过，直接生成」。信息越完整，报告越精准——建议尽量补全，跳过的项目将按保守判断处理。

```
收到！在正式开始竞品调研之前，我先帮你梳理一下关键信息。
已有的信息我帮你预填了，你可以逐项确认或修改，也可以直接说「跳过，直接生成」。

━━━━━━━━━━━━━━━━━━━━━━
📋 信息采集清单
━━━━━━━━━━━━━━━━━━━━━━

1️⃣ 调研目标（要解决什么问题）：[已提取 / 待补充]
2️⃣ 对标对象（≥2个，1个时做单竞品深描）：[已提取 / 待补充]
3️⃣ 我方现状（当前方案、痛点、约束）：[已提取 / 待补充]
4️⃣ 核心场景（用户关键链路）：[已提取 / 待补充]
5️⃣ 行业：[已推断 / 待补充]
6️⃣ 补充材料（截图/录屏/文档/链接）：[已提取 / 待补充]
7️⃣ 战略模块：
   🔲 竞争格局（竞争引力图）
   🔲 SWOT（行动矩阵化）
   🔲 波特五力（力场温度）
   🔲 PESTLE（外部信号面板）
   → 当前预设：[根据调研目标推断是否需要]
8️⃣ 报告用途：
   📋 内部评审/排期会 ← 默认
   📤 对外分享（需脱敏）
   → 当前预设：[根据用户语境推断]
9️⃣ 约束条件（时间/资源/技术栈）：[已提取 / 待补充]

💡 信息越详细，报告越精准。也可以直接回复「跳过，直接生成」。
```

用户回复处理：逐项补充→更新后生成 / "跳过"→用推断值生成 / 只补部分→混合使用

---

## 双轨四层法（方法概要）

本技能采用原创「双轨四层法」，详细规则见 [references/research-playbook.md](references/research-playbook.md)：

- **体验对标轨（八维）**：回答"竞品具体怎么做，我方具体差在哪"
  - D1 信息架构 · D2 交互流程 · D3 视觉表达 · D4 文案设计 · D5 行为驱动 · D6 异常边界 · D7 跨端一致 · D8 合规可及
  - 先拆"最小操作节点"，再做逐产品对照

- **战略诊断轨（可选四件套）**：回答"赛道为什么这样竞争，我方应该怎么打"
  - 竞争格局（竞争引力图） · SWOT（行动矩阵化） · 波特五力（力场温度） · PESTLE（外部信号面板）
  - 启用条件：涉及赛道/定位/定价/份额/壁垒/替代威胁时自动开启

- **证据建库（三层证据法）**：每条关键结论挂 `SRC-xxx`
  - SRC-U（用户证据） · SRC-P（公开证据） · SRC-H（经验证据，需标"建议验证"）

---

## 输出

默认输出 HTML 专业报告，严格按照 [references/report-template-pro.html](references/report-template-pro.html) 的结构和样式生成，含：

1. Hero（调研目标、一句话结论、结论标签）
2. KPI Strip（产品数 / 发现数 / Pattern 数 / 行动项数）
3. Callouts（Top Insight / Priority Action）
4. Research Scope + Source Coverage
5. Summary Conclusions
6. Competitive Benchmark Table（场景 × 产品 × 维度对标）
7. Strategic Analysis（SWOT + 波特五力 + PESTLE，启用时）
8. Key Findings
9. Reusable Patterns（可选）
10. Implementation Roadmap
11. Source Index
12. Disclaimer

报告用途为"对外分享"时自动脱敏。详细输出格式锁、建议表达规范、文风护栏和生成前自检规则见 [references/research-playbook.md](references/research-playbook.md)。

---

## 硬约束

### 信息优先原则（最高优先级）

- **禁止编造**：所有分析必须基于用户实际提供的信息，禁止凭想象补充用户未提及的业务细节
- **缺失标注**：用户未提供的信息在分析时标注"信息缺失"，给保守判断
- **推断透明**：从上下文合理推断的信息必须标注「推断」并说明依据
- **追问优先于脑补**：信息不足以完成分析时，优先通过采集清单追问

### 证据与输出

- 每条关键结论至少挂一个 `SRC-xxx`
- 体验轨与策略轨分工清晰，不得同义重复
- 去 AI 化文风，结论必须具名、具数、具动作
- 必须有执行建议（含 Owner / 优先级 / 依赖）
- 报告末尾必须附免责声明
- 优先级：信息优先原则（最高） > 输出格式锁 > 方法规则（playbook） > 文风护栏

### 合规与免责

- 报告末尾必须附免责声明，说明本报告为 AI 生成、不构成专业咨询
- 不可核实的数据不写具体数值
- 必须遵守 [references/factual-reporting-and-style.md](references/factual-reporting-and-style.md)

## 参考文件

| 文件 | 内容 |
|------|------|
| [references/research-playbook.md](references/research-playbook.md) | 调研方法手册（信息采集规则、场景拆解、证据建库、八维体验对标、战略四件套详细输出规则） |
| [references/report-template-pro.html](references/report-template-pro.html) | 专业 HTML 报告模板（浅蓝 Hero 风格，12 分区） |
| [references/factual-reporting-and-style.md](references/factual-reporting-and-style.md) | 事实核查与文风约束 |
