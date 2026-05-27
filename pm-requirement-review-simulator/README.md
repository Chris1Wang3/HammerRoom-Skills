# PM Requirement Review Simulator

[中文版](README-zh.md)

Everyone says "sounds good" to your PRD. But in the real review meeting, engineering says it can't be built, operations says users won't use it, and legal says it's a liability.

The PM Requirement Review Simulator gives you a **5-role cross-functional stress test** before the real meeting — outputs a scored HTML survival report so you walk in prepared, not blindsided.

## Workflow

```mermaid
flowchart TD
    A["📝 Submit Requirement"] --> B["📋 Info Collection Checklist"]
    B --> C{"User Confirms / Skips"}
    C --> D["🔍 Identify Type + PRD Source"]
    D --> E["🎭 5-Role Challenge"]

    E --> E1["🛠️ Engineering"]
    E --> E2["📈 Operations"]
    E --> E3["🎨 Design"]
    E --> E4["👔 Executive"]
    E --> E5["⚖️ Legal"]

    E1 --> F["⚙️ Scoring Engine"]
    E2 --> F
    E3 --> F
    E4 --> F
    E5 --> F

    F --> G["25 Items × 0/1/2"]
    G --> H["Weighted → Survival Rate"]
    H --> I{"Decision Gates"}
    I -->|Pass| J["✅ Go"]
    I -->|Conditional| K["⚠️ Conditional Go"]
    I -->|Fail| L["❌ No Go"]

    J --> M["📊 HTML Report"]
    K --> M
    L --> M
```

## 5 Challenge Roles

| Role | What They Challenge |
|------|---------------------|
| 🛠️ Engineering | Can this actually be built? What about tech debt and scaling? |
| 📈 Operations | Will users actually use this? What's the adoption path? |
| 🎨 Design | Is the UX coherent? Where's the experience gap? |
| 👔 Executive | Does this align with strategy? What's the ROI? |
| ⚖️ Legal | Any compliance risks? Data privacy? Regulatory issues? |

## Difficulty Levels

| Level | Style | Best For |
|-------|-------|----------|
| 🟢 Rookie | Gentle suggestions, constructive tone | New PMs, first-time practice |
| 🟡 Realistic | Standard big-tech review intensity | Pre-meeting dry run |
| 🔴 Hell Mode | All hostile + industry jargon attacks | Senior PMs stress-testing edge cases |

## What You Get

A **light-blue themed HTML survival report** (SVG gauge + radar chart):

- **Survival Score** — deterministic scoring engine (25 items × 0/1/2), formula-calculated
- **5-Dimension Radar Chart** — visual breakdown of strengths and fatal weaknesses
- **Decision Gates** — value / risk / resource / strategy with A/B/C option comparison
- **Counterargument Playbook** — TOP 3 hardest questions with killer reply techniques
- **RACI Matrix** — cross-team collaboration with conflict resolution
- **Meeting Script** — ready-to-use opening → core argument → risk plan → decision → close
- **Action Checklist** — owner + deadline + deliverable + review checkpoint

## Use Cases

- **Pre-review Rehearsal**: Expose blind spots before the real meeting
- **PRD Self-check**: Deterministic scoring for requirement health assessment
- **New PM Training**: Simulate big-tech review pressure in a safe environment
- **Published PRD Review**: Professional evaluation of publicly shared PRDs

## Quick Start

```text
Review my team's group-buying feature. Realistic mode.
```

## Install

```bash
openclaw skills install pm-requirement-review-simulator
```

---

> Before the real review meeting, let five roles stress-test your PRD first.

License: MIT
