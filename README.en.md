<div align="center">

[中文](./README.md) · **English**

# 🪑 HammerRoom Skills · 拍砖间

**HammerRoom** — OPC Board · Competitive Product Research · PM Requirement Review Simulator

<br/>

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)
[![Skills](https://img.shields.io/badge/Skills-3-22c55e?style=flat-square)](#skills)
[![Agent Skills](https://img.shields.io/badge/Agent-Skills-8b5cf6?style=flat-square)](https://agentskills.io)
<br/>
[![Claude Code](https://img.shields.io/badge/Claude_Code-✓-d97706?style=flat-square&logo=anthropic&logoColor=white)](https://claude.ai/code)
[![Cursor](https://img.shields.io/badge/Cursor-✓-000000?style=flat-square&logo=cursor&logoColor=white)](https://cursor.com)
[![OpenClaw](https://img.shields.io/badge/OpenClaw-✓-ec4899?style=flat-square)](https://openclaw.ai)
[![Codex](https://img.shields.io/badge/Codex-✓-10b981?style=flat-square&logo=openai&logoColor=white)](https://openai.com/codex)

</div>

---

## Table of contents

| # | Skill | Summary | ClawHub |
|---|-------|---------|---------|
| 1 | 🏛️ [**OPC Board**](#opc-board) | Five-dimension stress-test for solo business ideas | [ClawHub v1.3.6](https://clawhub.ai/Chris1Wang3/opc-board) |
| 2 | 🔍 [**Competitive Product Research**](#competitive-product-research) | Dual-track benchmarking + strategic diagnostics | [ClawHub v1.4.1](https://clawhub.ai/Chris1Wang3/competitive-product-research) |
| 3 | ⚔️ [**PM Requirement Review Simulator**](#pm-requirement-review-simulator) | Five-role PRD review with survival scoring | [ClawHub v1.2.3](https://clawhub.ai/Chris1Wang3/pm-requirement-review-simulator) |

---

## Install

### OpenClaw / ClawHub

```bash
openclaw skills install opc-board
openclaw skills install competitive-product-research
openclaw skills install pm-requirement-review-simulator
```

Or install from [ClawHub · Chris1Wang3](https://clawhub.ai/Chris1Wang3).

### Cursor / Claude Code / Codex

Clone this repo and add each skill directory (with its `SKILL.md`) to your agent skill path, or copy subdirectories into your project `.cursor/skills` / user skills folder.

```bash
git clone https://github.com/Chris1Wang3/HammerRoom-Skills.git
```

> **Note:** Do not install third-party CLIs or agent tool artifacts inside this repository; use global paths or a separate directory outside the repo.

---

## Skills

<a id="opc-board"></a>

<table width="100%">
<tr>
<td valign="top" width="100%">

<h3>🏛️ OPC Board</h3>

<p>
<a href="https://clawhub.ai/Chris1Wang3/opc-board"><img src="https://img.shields.io/badge/ClawHub-v1.3.6-ff69b4?style=for-the-badge" alt="ClawHub" /></a>
</p>

<p><strong>Friends say sounds great; AI says wonderful idea — you need someone willing to push back.</strong> OPC Board convenes 5 professional advisors (tech / growth / experience / business / risk) to stress-test solo ventures, side projects, open-source ideas, or SaaS concepts across <strong>5 dimensions and 25 sub-items</strong> with formula-based scoring, Go / Conditional Go / No Go decisions, MoSCoW scoping, Pre-Mortem risks, and an action plan.</p>

<ul>
<li>Use cases: indie developers, open-source authors, early founders, content creators pre-launch self-check</li>
<li>Output: professional HTML feasibility report + OPC Decision Card</li>
<li>Docs: <a href="opc-board/SKILL.md">SKILL.md</a> · <a href="opc-board/README-zh.md">README-zh</a> · <a href="opc-board/README.md">README-en</a></li>
</ul>

</td>
</tr>
</table>

<br/>

<a id="competitive-product-research"></a>

<table width="100%">
<tr>
<td valign="top" width="100%">

<h3>🔍 Competitive Product Research</h3>

<p>
<a href="https://clawhub.ai/Chris1Wang3/competitive-product-research"><img src="https://img.shields.io/badge/ClawHub-v1.4.1-ff69b4?style=for-the-badge" alt="ClawHub" /></a>
</p>

<p><strong>Competitive analysis should not be a feature checklist.</strong> This skill uses an original <strong>dual-track four-layer method</strong>: experience benchmarking (8 UX dimensions) and strategic diagnostics (SWOT, Porter's Five Forces, PESTLE) in parallel; a structured intake checklist aligns context first, then produces a <strong>source-traceable</strong> professional HTML report with actions, owners, complexity, and evidence IDs.</p>

<ul>
<li>Use cases: benchmarking, differentiation strategy, pre-review competitive materials, funnel / conversion diagnosis</li>
<li>Output: professional HTML competitive research report</li>
<li>Docs: <a href="competitive-product-research/SKILL.md">SKILL.md</a> · <a href="competitive-product-research/README-zh.md">README-zh</a> · <a href="competitive-product-research/README.md">README-en</a></li>
</ul>

</td>
</tr>
</table>

<br/>

<a id="pm-requirement-review-simulator"></a>

<table width="100%">
<tr>
<td valign="top" width="100%">

<h3>⚔️ PM Requirement Review Simulator</h3>

<p>
<a href="https://clawhub.ai/Chris1Wang3/pm-requirement-review-simulator"><img src="https://img.shields.io/badge/ClawHub-v1.2.3-ff69b4?style=for-the-badge" alt="ClawHub" /></a>
</p>

<p><strong>Rehearse before the real review — cheaper than getting roasted in the meeting.</strong> Simulates engineering, ops, design, executive, and legal challenges to your PRD; supports <strong>Rookie / Realistic / Hell</strong> difficulty; deterministic scoring outputs an HTML survival report with a <strong>five-dimension radar chart</strong>, killer replies, RACI pack, meeting script, and action list.</p>

<ul>
<li>Use cases: pre-review stress-test, cross-functional rehearsal, meeting asset prep</li>
<li>Output: professional HTML requirement review report</li>
<li>Docs: <a href="pm-requirement-review-simulator/SKILL.md">SKILL.md</a> · <a href="pm-requirement-review-simulator/README-zh.md">README-zh</a> · <a href="pm-requirement-review-simulator/README.md">README-en</a></li>
</ul>

</td>
</tr>
</table>

---

## Quick start

Trigger with natural language in any agent that has these skills configured:

```text
# OPC Board
I want to build a WeChat mini program for bookkeeping — help me assess feasibility.

# Competitive research
Our app post conversion rate is only 3%. Compare with Xiaohongshu and Instagram on the first-post funnel.

# Requirement review
Review this PRD: https://www.woshipm.com/evaluating/4069331.html
```

You can also say "run with an example" for any skill — the agent will construct sample input per the SKILL workflow and generate a report.

---

## About the author

**Chris Wang** ([@Chris1Wang3](https://github.com/Chris1Wang3))

AI product lead for growth and monetization, focused on packaging the kind of professional pushback you only get in meetings into reusable Agent Skills — delivering reports and decision assets you can actually use. Feedback welcome via [GitHub Issues](https://github.com/Chris1Wang3/HammerRoom-Skills/issues).

---

<div align="center">

[MIT License](./LICENSE) · free to use, modify, and redistribute

Made by [@Chris1Wang3](https://github.com/Chris1Wang3)

</div>

<br/>