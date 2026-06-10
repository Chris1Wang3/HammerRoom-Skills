<div align="center">

**中文** · [English](./README.en.md)

# 🪑 拍砖间 · HammerRoom Skills

**拍砖间** — 一人董事会 · 竞品调研 · 需求评审模拟器 · 技能质量评分器

<br/>

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)
[![Skills](https://img.shields.io/badge/Skills-4-22c55e?style=flat-square)](#技能)
[![Agent Skills](https://img.shields.io/badge/Agent-Skills-8b5cf6?style=flat-square)](https://agentskills.io)
<br/>
[![Claude Code](https://img.shields.io/badge/Claude_Code-✓-d97706?style=flat-square&logo=anthropic&logoColor=white)](https://claude.ai/code)
[![Cursor](https://img.shields.io/badge/Cursor-✓-000000?style=flat-square&logo=cursor&logoColor=white)](https://cursor.com)
[![OpenClaw](https://img.shields.io/badge/OpenClaw-✓-ec4899?style=flat-square)](https://openclaw.ai)
[![Codex](https://img.shields.io/badge/Codex-✓-10b981?style=flat-square&logo=openai&logoColor=white)](https://openai.com/codex)

</div>

---

## 目录

| # | 技能 | 说明 | ClawHub |
|---|------|------|---------|
| 1 | 🏛️ [**一人董事会（OPC Board）**](#opc-board) | 五维压测一人公司 / 副业想法可行性 | [ClawHub v1.3.6](https://clawhub.ai/Chris1Wang3/opc-board) |
| 2 | 🔍 [**竞品调研（CPR）**](#competitive-product-research) | 双轨四层法：体验对标 + 战略诊断 | [ClawHub v1.4.1](https://clawhub.ai/Chris1Wang3/competitive-product-research) |
| 3 | ⚔️ [**PM 需求评审模拟器**](#pm-requirement-review-simulator) | 五角色攻防推演 + 存活率报告 | [ClawHub v1.2.3](https://clawhub.ai/Chris1Wang3/pm-requirement-review-simulator) |
| 4 | 📊 [**技能质量评分器**](#skill-quality-scorer) | TRACE+ 六维 30 子项确定性评分 | [ClawHub v1.1.7](https://clawhub.ai/Chris1Wang3/skill-quality-scorer) |

---

## 安装

### OpenClaw / ClawHub

```bash
openclaw skills install opc-board
openclaw skills install competitive-product-research
openclaw skills install pm-requirement-review-simulator
openclaw skills install skill-quality-scorer
```

或从 [ClawHub · Chris1Wang3](https://clawhub.ai/Chris1Wang3) 安装对应技能包。

### Cursor / Claude Code / Codex

将本仓库克隆到本地，在 Agent 设置中将各技能目录（含 `SKILL.md`）加入技能路径，或复制子目录到项目的 `.cursor/skills` / 用户技能目录。

```bash
git clone https://github.com/Chris1Wang3/HammerRoom-Skills.git
```

> **注意：** 请勿在本仓库目录内安装第三方 CLI 或 Agent 工具产物；请使用全局路径或仓库外的独立目录。

---

## 技能

<a id="opc-board"></a>

<table width="100%">
<tr>
<td valign="top" width="100%">

<h3>🏛️ 一人董事会 · OPC Board</h3>

<p>
<a href="https://clawhub.ai/Chris1Wang3/opc-board"><img src="https://img.shields.io/badge/ClawHub-v1.3.6-ff69b4?style=for-the-badge" alt="ClawHub" /></a>
</p>

<p><strong>朋友说「不错」，AI 说 wonderful idea——你真正需要的是愿意拍砖的人。</strong> 一人董事会召集 5 位专业顾问（技术 / 增长 / 体验 / 商业 / 风险），对一人公司、副业、开源或 SaaS 想法进行<strong>五维 25 子项</strong>确定性压测，输出带公式的可行性评分、Go / Conditional Go / No Go 决策、MoSCoW 范围、Pre-Mortem 风险与行动清单。</p>

<ul>
<li>适用：独立开发者、开源作者、早期创业者、内容创作者上线前自检</li>
<li>输出：专业HTML评估报告 + OPC 决策卡</li>
<li>文档：<a href="opc-board/SKILL.md">SKILL.md</a></li>
</ul>

</td>
</tr>
</table>

<br/>

<a id="competitive-product-research"></a>

<table width="100%">
<tr>
<td valign="top" width="100%">

<h3>🔍 竞品调研 · Competitive Product Research</h3>

<p>
<a href="https://clawhub.ai/Chris1Wang3/competitive-product-research"><img src="https://img.shields.io/badge/ClawHub-v1.4.1-ff69b4?style=for-the-badge" alt="ClawHub" /></a>
</p>

<p><strong>竞品分析不应是功能清单堆砌。</strong> 本技能采用原创<strong>双轨四层法</strong>：体验对标（8 大 UX 维度）与战略诊断（SWOT、波特五力、PESTLE）并行；先通过结构化信息采集清单对齐上下文，再生成<strong>证据可溯源</strong>的专业 HTML 报告，含动作建议、责任人、复杂度与证据编号。</p>

<ul>
<li>适用：对标分析、差异化策略、评审会前竞品材料、漏斗 / 转化问题诊断</li>
<li>输出：专业 HTML 竞品调研报告</li>
<li>文档：<a href="competitive-product-research/SKILL.md">SKILL.md</a></li>
</ul>

</td>
</tr>
</table>

<br/>

<a id="pm-requirement-review-simulator"></a>

<table width="100%">
<tr>
<td valign="top" width="100%">

<h3>⚔️ PM 需求评审模拟器</h3>

<p>
<a href="https://clawhub.ai/Chris1Wang3/pm-requirement-review-simulator"><img src="https://img.shields.io/badge/ClawHub-v1.2.3-ff69b4?style=for-the-badge" alt="ClawHub" /></a>
</p>

<p><strong>评审前预演，比会上挨骂便宜。</strong> 模拟技术、运营、设计、老板、法务五方对 PRD 的攻防挑战；支持<strong>新手 / 实战 / 地狱</strong>三级残酷度；确定性评分引擎逐子项打分，输出带<strong>五维雷达图</strong>的 HTML 存活率报告、神回复话术、RACI 协作包、会议脚本与行动清单。</p>

<ul>
<li>适用：需求评审前压测、跨部门博弈预演、会议资产准备</li>
<li>输出：专业HTML 需求评审报告</li>
<li>文档：<a href="pm-requirement-review-simulator/SKILL.md">SKILL.md</a></li>
</ul>

</td>
</tr>
</table>

<br/>

<a id="skill-quality-scorer"></a>

<table width="100%">
<tr>
<td valign="top" width="100%">

<h3>📊 技能质量评分器 · Skill Quality Scorer</h3>

<p>
<a href="https://clawhub.ai/Chris1Wang3/skill-quality-scorer"><img src="https://img.shields.io/badge/ClawHub-v1.1.7-ff69b4?style=for-the-badge" alt="ClawHub" /></a>
</p>

<p><strong>迭代没方向、发布前没底——你需要的是确定性评分，不是模型随口夸。</strong> 对现有 Agent Skill（SKILL.md）做 <strong>TRACE+ 六维 30 子项</strong>全维审计：先跑 <code>static_audit.py</code> 静态脚本，再按 rubric 逐项 evidence，公式算综合分；支持单技能、A vs B 对比、批量评分，输出 JSON + Markdown 报告。</p>

<ul>
<li>适用：技能迭代对标、发布前自检、批量评 <code>skills/</code> 目录、和同类 skill 找差距</li>
<li>输出：JSON 评分 + Markdown 审计报告（含 Top 修复项与触发测试）</li>
<li>文档：<a href="skill-quality-scorer/SKILL.md">SKILL.md</a></li>
</ul>

</td>
</tr>
</table>

---

## 快速开始

在已配置 Agent 技能的对话中，直接自然语言触发即可：

```text
# 一人董事会
我想做一个记账类微信小程序，帮我分析一下可行性。

# 竞品调研
我们 App 发帖转化率只有 3%，请对标小红书和 Instagram，分析发帖首链路问题。

# 需求评审
评审一下这个prd：https://www.woshipm.com/evaluating/4069331.html。

# 技能质量评分
给 portfolio-doctor 做 TRACE+ 全维评分，和 skill-reviewer 差在哪？
```

也可对任一技能说「用示例跑一下」，Agent 将按 SKILL 工作流构造示例输入并生成报告。

---

## 关于作者

**Chris Wang**（[@Chris1Wang3](https://github.com/Chris1Wang3)）

AI产品，负责增长/商业化，专注把「会议里才会出现的专业质疑」封装成可复用的 Agent Skills，输出可交付的报告与决策资产。问题与建议请提 [GitHub Issues](https://github.com/Chris1Wang3/HammerRoom-Skills/issues)。

---

<div align="center">

[MIT License](./LICENSE) · 自由使用 / 修改 / 再分发

Made by [@Chris1Wang3](https://github.com/Chris1Wang3)

</div>

<br/>

