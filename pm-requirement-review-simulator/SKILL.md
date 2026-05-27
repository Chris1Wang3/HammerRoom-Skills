---
name: pm-requirement-review-simulator
description: >-
  PRD review stress-test simulator: 5 cross-functional roles challenge your requirements
  across 3 difficulty levels, outputs a scored HTML survival report with radar chart and meeting script.
  当用户需要评审产品需求文档(PRD)、模拟需求评审会议、或预演跨部门博弈时使用。以需求评审攻防推演为核心，模拟技术/运营/设计/老板/法务五方挑战；具备"新手/实战/地狱"三级残酷度；输出质疑清单、应对话术、存活率评分卡和标准会议资产。
---

# PM 需求评审模拟器

> 把你的需求扔进来，五方角色帮你拍砖，输出一份带存活率评分的专业报告。

## 适用场景

- 产品经理在需求评审前预演，担心被技术/运营/老板等角色挑战
- 需要多方博弈下的可落地决策方案，不只要"问题列表"
- 需要会议可执行资产：脚本、分工表、决策闸门、风险预案
- 想看看自己的 PRD 能在"地狱模式"活几分钟

## 不适合

- 从零撰写 PRD（这是压测器，不是写作工具）
- 已上线产品的全面复盘（支持局部迭代评审，不做系统性事后诊断）
- 替你做最终决策（给 Go / Conditional Go / No Go 建议，拍板仍由你）

## 怎么用

```text
帮我评审一下我们要做的拼团功能，实战模式。
```

用户也可以说「用示例跑一下」，或按 [references/user_templates.md](references/user_templates.md) 模板详细填写。

## 工作流

```
1) 用户提交需求
2) 输出信息采集清单（用户确认或"跳过"）
3) 识别需求类型 + PRD 来源 + N/A 维度
4) 五角色逐个质疑（按残酷度调整语气）
5) 子项打分 → 权重归一化 → 综合存活率
6) 生成 HTML 报告 + 会议资产
```

### 信息采集清单（第 2 步输出）

从用户输入中自动提取已有信息并预填，缺失项标注「待补充」，用户可逐项确认或说「跳过，直接生成」。信息越完整，评分越准确——建议尽量补全，跳过的项目将按保守分处理。

```
1️⃣ 需求名称：[已提取 / 待补充]
2️⃣ 业务目标：[已提取 / 待补充]
3️⃣ 核心功能：[已提取 / 待补充]
4️⃣ 评审残酷度：🟢 新手村 / 🟡 实战（默认）/ 🔴 地狱
5️⃣ 行业：[已推断 / 待补充]
6️⃣ 公司规模：[已提取 / 待补充]
7️⃣ 技术栈：[已提取 / 待补充]
8️⃣ 约束条件（上线期限/预算/人力）：[已提取 / 待补充]
9️⃣ 评审角色：技术/运营/设计/老板/法务（默认全开，可删减）
🔟 需求类型：📦 大型产品功能 / 🔧 工具类 / 🚀 MVP / 🔄 迭代优化 / ⚖️ 合规敏感型
1️⃣1️⃣ 维度适用性：自动识别是否存在 N/A 维度
1️⃣2️⃣ PRD 来源：📄 用户自有 PRD / 🌐 公开/展示版 PRD
```

## 五角色 × 五维评分

| 角色 | 核心关切 | 主评维度 |
|------|---------|---------|
| 🛠️ 技术负责人 | 做得出来吗？维护谁扛？ | 技术友好 |
| 📈 运营总监 | 能带来多少 DAU？怎么推？ | 运营价值 |
| 🎨 设计主管 | 交互合理吗？用户会用吗？ | 运营价值（体验影响留存） |
| 👔 老板/决策者 | ROI 多少？战略匹配吗？ | 老板满意 |
| ⚖️ 法务顾问 | 合规风险兜得住？ | 合规安全 |

| 维度 | 衡量什么 |
|------|---------|
| 逻辑自洽 | 需求本身有没有自相矛盾（跨角色汇总，永不 N/A） |
| 技术友好 | 技术可行性、开发成本、维护负担 |
| 运营价值 | 推广路径、数据埋点、用户增长、体验差异化 |
| 老板满意 | 商业价值、ROI、战略匹配 |
| 合规安全 | 合规风险、数据安全、知识产权 |

每维度 5 个子项（0/1/2 分），公式计算综合存活率。三档残酷度调整角色语气和问题深度。详见 [scoring-engine-deterministic.md](references/scoring-engine-deterministic.md)。

## 输出

默认输出 HTML 报告，严格按照 [report-template-pro.html](references/report-template-pro.html) 生成，含：

1. 存活率评分卡（五维得分 + 综合分 + 评级 + 致命死穴 + 救命稻草）
2. 决策结论 + 决策闸门 + A/B/C 方案对比
3. 五角色质疑面板（按致命/重要/次要排序）
4. 杀手回复 TOP 3（普通回复 vs 杀手回复 + 技巧拆解）
5. 跨团队协作（RACI 矩阵 + 冲突识别与解决）
6. 评审会议脚本（开场 → 核心论证 → 风险预案 → 决策 → 收尾）
7. 优化建议（🔴 必修 / 🟡 可选 / ⚪ 延后）
8. 行动清单（责任人 + 截止时间 + 交付物 + 回看节点）

报告 11 大分区顺序：Hero → Radial Hub → Callouts → Decision Gates → Five-Role Challenge → Killer Replies → Cross-Team Collaboration → Meeting Script → Optimization → Action List → Disclaimer

详细输出格式锁、质量标准和生成前自检规则见 [references/review-playbook.md](references/review-playbook.md)。

## 硬约束

### 信息优先原则（最高优先级）

- **禁止编造**：所有分析必须基于用户实际提供的信息，禁止凭想象补充用户未提及的业务细节
- **缺失标注**：用户未提供的信息在评分时标注「信息缺失」，给保守分 1 分
- **推断透明**：从上下文推断的信息必须标注「推断」并说明依据
- **追问优先于脑补**：信息不足时，优先通过信息采集清单追问

### 评分与输出

- 评分按 [scoring-engine-deterministic.md](references/scoring-engine-deterministic.md) 公式，禁止凭感觉
- 25 个子项必须逐项打分，宁可保守给 1 分，不可跳过
- 必须有 Go / Conditional Go / No Go 结论
- 去 AI 化文风，结论必须具名、具数、具动作
- 残酷度一旦确认不中途降级
- 优先级：信息优先原则（最高） > 评分引擎 > 报告模板 > 角色灵魂

### 合规与免责

- 报告末尾必须附免责声明，说明本报告为 AI 生成、不构成专业咨询
- 涉及合规/法律/金融/医疗等专业领域时，必须提醒用户咨询持牌专业人士

## 参考文件

| 文件 | 内容 |
|------|------|
| [references/scoring-engine-deterministic.md](references/scoring-engine-deterministic.md) | 确定性评分引擎（子项清单、权重归一化、展示版豁免、硬校验规则） |
| [references/review-playbook.md](references/review-playbook.md) | 评审攻防手册（角色人设 + 话术 + 会议脚本 + 输出格式锁 + 质量标准） |
| [references/report-template-pro.html](references/report-template-pro.html) | HTML 报告模板（浅蓝 Hero 风格，11 大分区） |
| [references/user_templates.md](references/user_templates.md) | 用户输入模板（通用/电商/B2B/金融 + 展示版快捷句） |
