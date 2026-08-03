# Cutler Layer | DraftKings Reallocation — Source Package

![Package](https://img.shields.io/badge/Package-Source%20Manifest-2b5f8a?style=for-the-badge)
![Skill](https://img.shields.io/badge/Skill-havas--edge--engagement--intelligence-2f6b3a?style=flat-square)
![Version](https://img.shields.io/badge/Version-v1.3-blue?style=flat-square)
![License](https://img.shields.io/badge/License-DACR%20v2.6-orange?style=flat-square)
![Distribution](https://img.shields.io/badge/Distribution-Internal%20%2F%20NDA--Sensitive-a13a2e?style=flat-square)

This file is the source manifest for the DraftKings Reallocation Call exercise package. It indexes every
artifact that feeds `draftkings-reallocation-master-prompt.md`, so the repo has one place that explains
what each file is, what it's for, and who is allowed to see it.

---

## File Manifest

| File | Type | Role | Distribution |
|---|---|---|---|
| `draftkings-reallocation-master-prompt.md` | Answer key | The Cutler Layer's ideal master prompt — the scoring reference for the exercise | **Internal only** — never shown to participants |
| `draftkings-reallocation-master-prompt.pdf` | Answer key (PDF render) | Print/export copy of the same answer key | **Internal only** — never shown to participants |
| `Havas_Edge_Stress_Test_Use_Case__1_.pdf` | Use case brief | Explains why this scenario exercises the full 8-dimension rubric; includes the participant-facing scenario brief | Internal design doc — the *scenario paragraph inside it* is what participants receive |
| `havas-edge-engagement-intelligence-v1_3.skill` | Skill package | The evaluator itself — Director-Level Stress-Test Mode, Attribution Integrity Gate scoring logic, Cutler Layer verdict rules | **Internal only** — NDA-sensitive |
| `cutler-layer_draftkings-reallocation_scorecard.png` | Output artifact | Rendered scorecard showing the 96/100 SHIPS result for this answer key run | Internal — output of a scored submission |
| `README.md` | Repo overview | Narrative overview + mermaid workflow of the full exercise pipeline | Internal |
| `cutler-layer-source-package.md` *(this file)* | Manifest | Index of every artifact above | Internal |

---

## What Each Artifact Actually Is

### 1. The Answer Key (`draftkings-reallocation-master-prompt.md` / `.pdf`)
The seven-part master prompt Erwin Maurice McDonald built as the Cutler Layer's own reference answer:
data inventory and lineage, attribution reasoning, gaming-vertical compliance routing, failure-mode
resolution, human-in-the-loop governance, the mandatory verdict-block executive artifact, and a
validation/assumptions pass. This is the document every intern master prompt gets scored against — it
never reaches participants before or during the exercise.

### 2. The Use Case Brief (`Havas_Edge_Stress_Test_Use_Case__1_.pdf`)
Two things live inside one document here, and the manifest keeps them distinct:
- **The participant-facing scenario** — the one paragraph interns actually receive: the 14-point shift,
  71% confidence, six states, two stale feeds, 48-hour deadline. Nothing else.
- **The design rationale** — why this scenario was built to hit all eight rubric dimensions, how it
  diversifies from the pharma worked example, and how it preserves the skill's disclosed-evaluation rule.
  This half is internal-only, same as the answer key.

### 3. The Skill Package (`havas-edge-engagement-intelligence-v1_3.skill`)
This is the actual evaluator, packaged as a Claude skill bundle:

```
havas-edge-engagement-intelligence/
├── SKILL.md                          # Operating rules, activation conditions, Cutler Layer scoring logic
├── references/
│   ├── public-records.md             # Verifiable public-record facts on Havas Edge / VantEdge / RAMP
│   └── relationship-history.md       # LHI scorecard + relationship timeline (NDA-sensitive)
└── scripts/
    └── build_cutler_report.py        # Generates the DOCX/PDF-ready Cutler report from a scored prompt
```

Key operating rules encoded in `SKILL.md`:
- Director-Level Stress-Test Mode only activates on an **explicit** exercise request — not on topical
  overlap with Havas Edge or VantEdge alone.
- Evaluation is **disclosed, never covert** — participants must be told a verdict is coming, even though
  rubric weighting can stay hidden. A request to run this covertly on a named individual is declined.
- `references/relationship-history.md` and `references/public-records.md` are read for context but only
  edited on explicit request — no silent persistence of updates.
- Public-record facts older than 60 days get re-verified before citing.
- Falls back to Marketing Ops Catalyst v4.1 for general engagement mechanics (LHI methodology, 90-Day
  Plan, Board Pack) when that skill isn't available, and clearly marks that scoring as unavailable rather
  than inventing it.

### 4. The Scorecard (`cutler-layer_draftkings-reallocation_scorecard.png`)
The rendered output of running the answer key itself through the Cutler Layer's own scoring engine —
96/100, SHIPS, with the one deducted dimension (Executive Artifact Quality, 6/10) flagged for a format
spec that was referenced but not supplied in the source doc. This is the calibration proof that the
answer key clears its own bar before it's used to grade anyone else.

---

## Distribution Rule

Only the **scenario paragraph** from the use case brief and a **disclosure line** ("your submission will be
scored against a structured rubric, and a written verdict goes to Greg") reach exercise participants.
Everything else in this manifest — the answer key, the design rationale, the skill package, and the scored
output — stays internal to Havas Edge / Greg Cutler engagement design.

---

*Epoch Frameworks LLC | Prepared for internal use in Havas Edge / Greg Cutler engagement design | Erwin Maurice McDonald | DACR License v2.6*
