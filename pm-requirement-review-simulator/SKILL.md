---
name: pm-requirement-review-simulator
description: >-
  PRD review stress-test simulator: 5 cross-functional roles challenge your requirements
  across 3 difficulty levels, outputs a scored HTML or Markdown survival report with radar chart and meeting script.
  Use when PRD review, requirement review simulation, or cross-functional pushback rehearsal,
  or when the user says「评审需求」「模拟评审会」「帮我预演一下」.
---

# PM 需求评审模拟器 · Requirement Review Simulator

> **EN** Five roles stress-test your PRD before the real meeting → survival score + meeting assets.  
> **中文** 五角色预演评审攻防 → 存活率报告 + 会议脚本。

**When / 何时用：** 评审前预演 · 跨部门博弈 · 会议资产准备  
**Not / 不用：** 从零写 PRD · 上线后全面复盘 · 替用户拍板

```text
Review our group-buying feature. Realistic mode.
帮我评审拼团功能，实战模式。
```

结构化输入 → [user_templates.md](references/user_templates.md)

| 档位 | EN | 中文 |
|------|----|------|
| 🟢 | Rookie — gentle | 新手村 |
| 🟡 | Realistic — big-tech | 实战（默认） |
| 🔴 | Hell — hostile | 地狱 |

## 可直接触发的说法

以下口语输入都应触发本技能，不要求用户先提交完整 PRD：

- 帮我预演一下这个需求评审会。
- 这个 PRD 会被研发/运营/老板怎么怼？
- 我只有草稿，先按实战模式评一下。
- 帮我准备评审会上可能被问的问题和回答。
- 这个需求能不能过会？给我存活率。
- 用地狱模式挑战一下这个方案。
- 评审前帮我生成 RACI、会议脚本和行动清单。

## 最小可用输入

**最低可启动**：需求名称 + 核心功能。若缺业务目标，先按“提升关键业务指标”预填并要求用户确认。

**推荐输入**：业务目标、用户场景、核心功能、约束条件、技术依赖、评审角色、残酷度、PRD 来源（完整 PRD / 展示版 / 草稿 / 口述）、输出格式。

**可兼容输入**：

- 只有草稿：按“草稿 PRD”评审，缺失项保守分 1。
- 只有展示版：启用展示版评分校准，不因合理脱敏项过度扣分。
- 只有链接/截图：先提取可见需求，再标注不可见缺口。
- 用户说“直接生成”：默认实战模式，缺失项按保守分处理。

## 工作流

```text
1) 提交需求  2) 信息采集清单  3) 识别类型 + PRD 来源 + N/A 维度
4) 五角色质疑（按残酷度）  5) 子项打分 → 存活率  6) 按用户选择生成 HTML / Markdown 报告 + 会议资产
```

### 信息采集清单（第 2 步）

```text
1️⃣ 需求名称  2️⃣ 业务目标  3️⃣ 核心功能  4️⃣ 残酷度  5️⃣ 行业  6️⃣ 公司规模
7️⃣ 技术栈  8️⃣ 约束  9️⃣ 评审角色  🔟 需求类型  1️⃣1️⃣ N/A 维度  1️⃣2️⃣ PRD 来源
1️⃣3️⃣ 输出格式（HTML / Markdown）
```

跳过项保守分 1。

## 五角色 × 五维

| 角色 | 主评维度 |
|------|---------|
| 🛠️ 技术 | 技术友好 |
| 📈 运营 | 运营价值 |
| 🎨 设计 | 运营价值 |
| 👔 老板 | 老板满意 |
| ⚖️ 法务 | 合规安全 |

五维：逻辑自洽（永不 N/A）· 技术友好 · 运营价值 · 老板满意 · 合规安全。公式 → [scoring-engine-deterministic.md](references/scoring-engine-deterministic.md)。

## 输出

生成前先确认输出格式：`HTML` 或 `Markdown`。用户选择 HTML 时，按 [report-template-pro.html](references/report-template-pro.html) 生成；用户选择 Markdown 时，按同一评审结构输出结构化 Markdown。用户跳过格式选择时，默认 HTML。格式锁与自检 → [review-playbook.md](references/review-playbook.md)。

必含：存活率卡 · Go 结论 · 五角色质疑 · 杀手回复 TOP3 · RACI · 会议脚本 · 行动清单 · 免责声明。

## 硬约束

- **信息优先**：禁止编造；缺失→保守分 1；推断须标注；清单追问优于脑补
- **评分**：25 子项逐项；禁止凭感觉；必须有 Go 结论；残酷度确认后不降级
- **优先级**：信息优先 > 评分引擎 > 报告模板 > 角色灵魂
- **合规**：免责声明；专业领域提醒咨询持牌人士

**Rigid**（不可跳过）：
- 25 子项逐项打分 · 存活率公式计算 · Go/Conditional/No Go 结论 · 残酷度确认后不降级 · 杀手回复 TOP3 · RACI · 免责声明

**Flexible**（可按场景调整）：
- 角色话术措辞风格 · 质疑排序 · 会议脚本详略 · 行动清单条目数量

## N/A 维度规则

N/A 维度须在信息采集清单第 11 项确认，不可在评审中途自行降维。确认后该维子项不参与总分计算，公式分母相应减少。

## 验收与失败路径

- **清单追问**：≤3 轮未响应 → 标注缺失信息，跳过项保守分 1 继续
- **只有草稿**：可启动，但必须标注 PRD 来源为草稿，并按缺失项保守评分
- **只有展示版**：启用展示版校准；不得因脱敏省略内部指标而直接判低分
- **只有一句需求**：先追问业务目标和核心功能；用户拒绝补充时输出弱评审而非完整存活率
- **合规敏感**：金融/医疗/法律/未成年人场景，合规安全维度必须参与评分
- **残酷度**：确认后不降级；用户明确要求降级须重新确认
- **角色质疑**：每角色≥2 条质疑（地狱模式≥4 条）；信息不足时以保守假设质疑
- **完成标准**：存活率≥70% 为 Conditional Pass；≥85% 为 Pass；<50% 为 Fail
- **失败判定**：核心功能描述完全缺失且用户拒绝补充 → 告知无法有效评审

## 运行时说明

本 skill 无运行时脚本，工作流第 5 步（子项打分→存活率）由 LLM 读取 [scoring-engine-deterministic.md](references/scoring-engine-deterministic.md) 后自行计算执行。本 scoring-engine 为 PM 需求评审模拟器专属评分引擎，与仓库中其他同名文件无关。

## 参考文件

| 文件 | 内容 |
|------|------|
| [references/scoring-engine-deterministic.md](references/scoring-engine-deterministic.md) | 评分引擎 |
| [references/review-playbook.md](references/review-playbook.md) | 角色话术 · 格式锁 |
| [references/report-template-pro.html](references/report-template-pro.html) | HTML 模板 |
| [references/user_templates.md](references/user_templates.md) | 输入模板 |
