<div align="center">

[中文](./README.md) · **English**

# 🪑 HammerRoom Skills · 拍砖间

**HammerRoom** — OPC Board · Competitive Product Research · PM Requirement Review Simulator · ReviewCourt · Vague Requirement Unpacker · Skill Quality Scorer

<br/>

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)
[![Skills](https://img.shields.io/badge/Skills-6-22c55e?style=flat-square)](#skills)
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
| 1 | 🏛️ [**OPC Board**](#opc-board) | Five-dimension stress-test for solo business ideas | [ClawHub v1.4.2](https://clawhub.ai/Chris1Wang3/opc-board) |
| 2 | 🔍 [**Competitive Product Research**](#competitive-product-research) | Dual-track benchmarking + strategic diagnostics | [ClawHub v1.4.6](https://clawhub.ai/Chris1Wang3/competitive-product-research) |
| 3 | ⚔️ [**PM Requirement Review Simulator**](#pm-requirement-review-simulator) | Five-role PRD review with survival scoring | [ClawHub v1.2.8](https://clawhub.ai/Chris1Wang3/pm-requirement-review-simulator) |
| 4 | ⚖️ [**ReviewCourt**](#reviewcourt) | Post-meeting verdict from transcript evidence + PRD cross-check | [ClawHub v1.0.0](https://clawhub.ai/chris1wang3/skills/reviewcourt) |
| 5 | 🧩 [**Vague Requirement Unpacker**](#vague-requirement-unpacker) | Vague ask -> PM alignment pack | [ClawHub v1.0.3](https://clawhub.ai/Chris1Wang3/vague-requirement-unpacker) |
| 6 | 📊 [**Skill Quality Scorer**](#skill-quality-scorer) | TRACE+ six-dimension deterministic scoring | [ClawHub v1.1.9](https://clawhub.ai/Chris1Wang3/skill-quality-scorer) |

---

## Install

### OpenClaw / ClawHub

```bash
openclaw skills install opc-board
openclaw skills install competitive-product-research
openclaw skills install pm-requirement-review-simulator
openclaw skills install reviewcourt
openclaw skills install vague-requirement-unpacker
openclaw skills install skill-quality-scorer
```

Or install from [ClawHub · Chris1Wang3](https://clawhub.ai/Chris1Wang3).

**ReviewCourt** is also available on [ClawHub](https://clawhub.ai/chris1wang3/skills/reviewcourt): `openclaw skills install @chris1wang3/reviewcourt`. Runtime depends on the official Tencent Meeting CLI [`@tencentcloud/tmeet`](https://www.npmjs.com/package/@tencentcloud/tmeet) (install globally; do not install into this repository).

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
<a href="https://clawhub.ai/Chris1Wang3/opc-board"><img src="https://img.shields.io/badge/ClawHub-v1.4.2-ff69b4?style=for-the-badge" alt="ClawHub" /></a>
</p>

<p><strong>Friends say sounds great; AI says wonderful idea — you need someone willing to push back.</strong> OPC Board convenes 5 professional advisors (tech / growth / experience / business / risk) to stress-test solo ventures, side projects, open-source ideas, or SaaS concepts across <strong>5 dimensions and 25 sub-items</strong> with formula-based scoring, Go / Conditional Go / No Go decisions, MoSCoW scoping, Pre-Mortem risks, and an action plan.</p>

<ul>
<li>Use cases: indie developers, open-source authors, early founders, content creators pre-launch self-check</li>
<li>Output: professional HTML feasibility report + OPC Decision Card</li>
<li>Docs: <a href="opc-board/SKILL.md">SKILL.md</a></li>
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
<a href="https://clawhub.ai/Chris1Wang3/competitive-product-research"><img src="https://img.shields.io/badge/ClawHub-v1.4.6-ff69b4?style=for-the-badge" alt="ClawHub" /></a>
</p>

<p><strong>Competitive analysis should not be a feature checklist.</strong> This skill uses an original <strong>dual-track four-layer method</strong>: experience benchmarking (8 UX dimensions) and strategic diagnostics (SWOT, Porter's Five Forces, PESTLE) in parallel; a structured intake checklist aligns context first, then produces a <strong>source-traceable</strong> professional HTML report with actions, owners, complexity, and evidence IDs.</p>

<ul>
<li>Use cases: benchmarking, differentiation strategy, pre-review competitive materials, funnel / conversion diagnosis</li>
<li>Output: professional HTML competitive research report</li>
<li>Docs: <a href="competitive-product-research/SKILL.md">SKILL.md</a></li>
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
<a href="https://clawhub.ai/Chris1Wang3/pm-requirement-review-simulator"><img src="https://img.shields.io/badge/ClawHub-v1.2.8-ff69b4?style=for-the-badge" alt="ClawHub" /></a>
</p>

<p><strong>Rehearse before the real review — cheaper than getting roasted in the meeting.</strong> Simulates engineering, ops, design, executive, and legal challenges to your PRD under one consistent review standard; deterministic scoring outputs an HTML survival report with a <strong>five-dimension radar chart</strong>, killer replies, RACI pack, meeting script, and action list.</p>

<ul>
<li>Use cases: pre-review stress-test, cross-functional rehearsal, meeting asset prep</li>
<li>Output: professional HTML requirement review report</li>
<li>Docs: <a href="pm-requirement-review-simulator/SKILL.md">SKILL.md</a></li>
</ul>

</td>
</tr>
</table>

<br/>

<a id="reviewcourt"></a>

<table width="100%">
<tr>
<td valign="top" width="100%">

<h3>⚖️ ReviewCourt</h3>

<p>
<a href="https://clawhub.ai/chris1wang3/skills/reviewcourt"><img src="https://img.shields.io/badge/ClawHub-v1.0.0-ff69b4?style=for-the-badge" alt="ClawHub" /></a>
<img src="https://img.shields.io/badge/Depends-tmeet_CLI-0ea5e9?style=for-the-badge" alt="tmeet" />
</p>

<p><strong>Rehearse before the meeting; close the case after it.</strong> ReviewCourt uses the official Tencent Meeting <code>tmeet</code> CLI to build an evidence chain from smart minutes and <strong>paragraph-level transcripts</strong>, then issues a review recommendation: Pass / Conditional Pass / Reject / Insufficient Information. Optionally cross-checks the verdict against a PRD for gaps and conflicts, with blockers, draft acceptance criteria, and traceable evidence IDs. It does not replace the team's formal decision or evaluate people.</p>

<ul>
<li>Use cases: post-meeting requirement / PRD / tech-design closeout, pre-dev condition lists, meeting-vs-PRD gap and conflict checks</li>
<li>Output: Markdown review verdict sheet (quick / audit)</li>
<li>Docs: <a href="reviewcourt/SKILL.md">SKILL.md</a></li>
</ul>

</td>
</tr>
</table>

<br/>

<a id="vague-requirement-unpacker"></a>

<table width="100%">
<tr>
<td valign="top" width="100%">

<h3>🧩 Vague Requirement Unpacker</h3>

<p>
<a href="https://clawhub.ai/Chris1Wang3/vague-requirement-unpacker"><img src="https://img.shields.io/badge/ClawHub-v1.0.3-ff69b4?style=for-the-badge" alt="ClawHub" /></a>
</p>

<p><strong>A vague ask is not a finished PRD.</strong> This skill uses a five-layer unpacking method to turn fuzzy boss or business instructions into intent reconstruction, confirmation questions, scenario narrowing, scope skeletons, core flows/states, readiness scoring, risk flags, and stakeholder-facing response scripts.</p>

<ul>
<li>Use cases: vague boss/business asks, oral tasks, chat screenshots, one-line meeting notes, blank PRD before alignment</li>
<li>Output: Markdown / HTML PM action pack, with optional handoff to requirement review simulation</li>
<li>Docs: <a href="vague-requirement-unpacker/SKILL.md">SKILL.md</a></li>
</ul>

</td>
</tr>
</table>

<br/>

<a id="skill-quality-scorer"></a>

<table width="100%">
<tr>
<td valign="top" width="100%">

<h3>📊 Skill Quality Scorer</h3>

<p>
<a href="https://clawhub.ai/Chris1Wang3/skill-quality-scorer"><img src="https://img.shields.io/badge/ClawHub-v1.1.9-ff69b4?style=for-the-badge" alt="ClawHub" /></a>
</p>

<p><strong>No direction on iteration, no confidence before publish — you need deterministic scoring, not model flattery.</strong> Full <strong>TRACE+ six-dimension, 30 sub-item</strong> audit for existing Agent Skills (SKILL.md): run <code>static_audit.py</code> first, then rubric evidence per sub-item, formula composite score; supports single skill, A vs B comparison, and batch scoring — outputs JSON + Markdown report.</p>

<ul>
<li>Use cases: skill iteration benchmarking, pre-publish self-check, batch scoring <code>skills/</code>, gap analysis vs peer skills</li>
<li>Output: JSON score + Markdown audit report (with top fixes and trigger tests)</li>
<li>Docs: <a href="skill-quality-scorer/SKILL.md">SKILL.md</a></li>
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

# Requirement review (pre-meeting simulation)
Review this PRD: https://www.woshipm.com/evaluating/4069331.html

# ReviewCourt (post-meeting verdict)
Close out this afternoon's payment redesign review — can we start development?
Against this PRD, check whether last night's review change requests were captured.

# Vague requirement unpacking
My boss said new customer conversion is weak and asked whether we can add benefit incentives. Help me turn this into confirmation questions and an alignment skeleton.

# Skill quality scoring
Score portfolio-doctor with TRACE+ — where does it fall short vs skill-reviewer?
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
