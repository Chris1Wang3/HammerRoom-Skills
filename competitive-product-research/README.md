# Competitive Product Research

[中文版](README-zh.md)

> Original dual-track method for competitive research: experience benchmarking + strategic diagnostics. Starts with lightweight findings and a completion checklist, then turns user-supplied details into a full source-traceable HTML report.

## What This Skill Is Optimized For

- Turning competitor observations into **decision-ready actions**
- Keeping conclusions **traceable to evidence**
- Separating **experience gaps** from **strategy choices** to avoid mixed logic

## Method Snapshot

1. Scope alignment (confirm before run)
2. Evidence indexing (`SRC-xxx`)
3. Dual-track analysis
   - Experience benchmarking (8 dimensions)
   - Strategic diagnostics (optional: landscape, SWOT, Five Forces, PESTLE)
4. Tiered output (quick / standard / full HTML / shareable)
5. Quick output ends with a completion checklist for generating the full report

## When Inputs Are Incomplete

- The skill can start with only a research goal and benchmark targets, but must state key assumptions first.
- Missing current-state or scenario details are treated as open questions, not invented facts.
- Inaccessible public sources are marked as `SRC-GAP` with a clear follow-up path.
- Quick output must tell the user what is still needed for the full report.

## Output Sections

1. Cover
2. Executive Summary
3. Scope & Sources
4. Benchmark Matrix
5. Strategic Diagnostics (optional)
6. Key Findings
7. Reusable Patterns (optional)
8. Execution Actions
9. Source Index

## Key Constraints

- No fabricated numbers
- No unsupported claims
- No vague action items
- No heavyweight report by default
- Shareable mode must desensitize sensitive info

## Quick Start

```text
Our app's posting conversion rate is only 3%. Benchmark against Xiaohongshu and Instagram,
analyze first-posting funnel issues.
Current state: top-right entry + blank editor + no auto-draft.
```

## Core Files

- `SKILL.md` — workflow and rules
- `references/research-playbook.md` — detailed methods
- `references/report-template.html` — output template
- `references/factual-reporting-and-style.md` — fact and style constraints

## Install

```bash
openclaw skills install competitive-product-research
```

License: MIT
