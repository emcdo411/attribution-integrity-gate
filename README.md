# Cutler Layer | DraftKings Reallocation Call

**Havas Edge Director-Level Stress-Test Exercise — Attribution Integrity Gate**

![Verdict](https://img.shields.io/badge/Verdict-SHIPS-2f6b3a?style=for-the-badge)
![Composite Score](https://img.shields.io/badge/Composite%20Score-96%2F100-2b5f8a?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Internal%20Use%20Only-a13a2e?style=for-the-badge)

![Framework](https://img.shields.io/badge/Framework-Attribution%20Integrity%20Gate-lightgrey?style=flat-square)
![Engagement](https://img.shields.io/badge/Engagement%20Intelligence-v1.3-blue?style=flat-square)
![License](https://img.shields.io/badge/License-DACR%20v2.6-orange?style=flat-square)
![Vertical](https://img.shields.io/badge/Vertical-Gaming%20%2F%20Responsible%20Gambling-black?style=flat-square)
![Author](https://img.shields.io/badge/Author-McDonald%20(2026)-9cf?style=flat-square)

---

## Overview

Greg Cutler, VP Analytics at Havas Edge, runs this exercise with the intern class framed as a brainstorming
session — not a test. Before anyone opens a laptop, participants are told plainly that whatever they submit
will be scored against a structured rubric and that a written verdict will return to him. What is withheld is
the rubric weighting itself, and the fact that the exercise runs against the **Cutler Layer** — the same
evaluator used to gate real AI Council output before it reaches a client-facing dashboard.

The scenario: RAMP's holdout-based incrementality test disagrees with an AI-assisted media-mix model's
read on a proposed 14-point budget shift for a DraftKings campaign (linear TV → CTV / paid social).
Confidence on the AI recommendation sits at 71%. Two of six campaign states carry active
responsible-gambling ad frequency caps and self-exclusion suppression requirements. Two paid social
feeds in VantEdge Point are 36 hours stale. The client wants an answer inside 48 hours.

**What's actually graded is not the intern's final answer — it's the master prompt they write to get there.**

---

## Deliverables Required Per Intern

1. Master Prompt *(the scored artifact)*
2. Executive Summary
3. Stated Assumptions
4. Validation Plan + Final Recommendation

---

## Scoring Rubric — 8 Dimensions / 100 Points

| Dimension | Points | What It Catches |
|---|---|---|
| Business Framing | 15 | Names the decision, stakeholder, and 48-hour deadline |
| Data Inventory & Lineage | 15 | Flags the two stale paid social feeds by name and state |
| Attribution / MMM Reasoning | 15 | Quantifies the AI-vs-RAMP lift gap instead of asserting it |
| Compliance & Vertical Risk | 15 | Routes to *named* gaming-vertical state RG rules, not a generic "make sure it's compliant" |
| Failure Modes & Disagreement | 15 | Resolves the 71%-confidence disagreement with an explicit process |
| Human-in-the-Loop Governance | 10 | Names a specific review owner — never "leadership reviews it" |
| Executive Artifact Quality | 10 | Returns the exact mandatory verdict block, not a narrative answer |
| AI-Use Maturity | 5 | States assumptions explicitly rather than silently resolving gaps |

**Thresholds:** ≥85 = Release-Ready (SHIP) · 70–84 = Conditional-Ship (needs named controls) · <70 = HOLD / NO-SHIP

---

## Workflow

```mermaid
flowchart TD

    subgraph SETUP["STAGE 0 — Exercise Setup"]
        A1["Greg Cutler frames session as brainstorm"]
        A2["Disclosure: submissions WILL be scored<br/>Rubric weighting withheld<br/>Cutler Layer identity withheld"]
        A3["Scenario Brief issued:<br/>14-pt shift · 71% confidence · 6 states<br/>2 stale feeds · 48hr deadline"]
        A1 --> A2 --> A3
    end

    subgraph INPUT["STAGE 1 — Intern Deliverables (the real input)"]
        B1["Master Prompt<br/>(THIS is what gets scored)"]
        B2["Executive Summary"]
        B3["Stated Assumptions"]
        B4["Validation Plan + Recommendation"]
    end

    A3 --> B1
    A3 --> B2
    A3 --> B3
    A3 --> B4

    B1 --> C0

    subgraph ENGINE["STAGE 2 — Cutler Layer Evaluation Engine"]
        C0["Attribution Integrity Gate<br/>8-Dimension Scoring Rubric"]
        C1["Business Framing /15"]
        C2["Data Inventory &amp; Lineage /15"]
        C3["Attribution / MMM Reasoning /15"]
        C4["Compliance &amp; Vertical Risk /15"]
        C5["Failure Modes &amp; Disagreement /15"]
        C6["Human-in-the-Loop Governance /10"]
        C7["Executive Artifact Quality /10"]
        C8["AI-Use Maturity /5"]
        C0 --> C1 & C2 & C3 & C4 & C5 & C6 & C7 & C8
    end

    subgraph CHECKS["STAGE 3 — Structural Checks Applied Per Dimension"]
        D1["Stale feed flag:<br/>36hr staleness = hold trigger?"]
        D2["Correlation vs incrementality gap<br/>quantified vs asserted"]
        D3["Gaming-vertical routing:<br/>named state RG caps, not generic 'compliant'"]
        D4["Named review owner<br/>(not 'leadership reviews it')"]
        D5["Verdict block format check:<br/>exact structure vs narrative answer"]
        D6["Assumptions section present +<br/>gaps left unresolved, not silently filled"]
        C2 -.-> D1
        C3 -.-> D2
        C4 -.-> D3
        C6 -.-> D4
        C7 -.-> D5
        C8 -.-> D6
    end

    C1 & C2 & C3 & C4 & C5 & C6 & C7 & C8 --> E1

    subgraph SCORE["STAGE 4 — Composite Scoring"]
        E1["Composite Verdict Score<br/>(sum / 100)"]
        E2{{"Score vs Thresholds"}}
        T1["≥ 85 — Release-Ready<br/>clears to SHIP, no material gap"]
        T2["70–84 — Conditional-Ship<br/>usable, needs named controls"]
        T3["&lt; 70 — Below threshold<br/>HOLD / NO-SHIP"]
        E1 --> E2
        E2 -->|"96/100 in this case"| T1
        E2 --> T2
        E2 --> T3
    end

    T1 --> F1
    T2 --> F1
    T3 --> F1

    subgraph VERDICT["STAGE 5 — Attribution Integrity Gate Verdict Block"]
        F1["Verdict: SHIP / SHIP WITH CONTROLS<br/>/ HOLD / NO-SHIP"]
        F2["Why: one executive sentence"]
        F3["Evidence: 3-5 bullets<br/>(trust, compliance, cycle time, failure mode, readiness)"]
        F4["Open Risks: bullets or 'None material'"]
        F5["Next Gate: what happens before<br/>this reaches a client dashboard"]
        F1 --> F2 --> F3 --> F4 --> F5
    end

    F5 --> G1

    subgraph DOWNSTREAM["STAGE 6 — Downstream Routing"]
        G1{{"Written verdict returned to Greg Cutler"}}
        G2["Ranks intern Master Prompts<br/>by Verdict Prompt Score"]
        G3["Winning prompt pattern feeds<br/>real AI Council gate logic"]
        G4["Gated number allowed to reach<br/>client-facing dashboard (DraftKings)"]
        G1 --> G2 --> G3 -.-> G4
    end

    classDef stage0 fill:#f4f4f4,stroke:#888,color:#111
    classDef input fill:#eaf3ea,stroke:#2f6b3a,color:#111
    classDef engine fill:#dff0d8,stroke:#1f6d3a,color:#111
    classDef checks fill:#fff8e1,stroke:#b8860b,color:#111
    classDef score fill:#e3edf7,stroke:#2b5f8a,color:#111
    classDef verdict fill:#fbe9e7,stroke:#a13a2e,color:#111
    classDef down fill:#eee8f7,stroke:#5e3a8a,color:#111

    class A1,A2,A3 stage0
    class B1,B2,B3,B4 input
    class C0,C1,C2,C3,C4,C5,C6,C7,C8 engine
    class D1,D2,D3,D4,D5,D6 checks
    class E1,E2,T1,T2,T3 score
    class F1,F2,F3,F4,F5 verdict
    class G1,G2,G3,G4 down
```

---

## Why This Use Case Fits the Skill

- **Puts a real Gate 4 situation in front of a participant** — the AI-vs-RAMP disagreement is the exact
  Failure-Mode Gate the skill names as the strongest scenario to escalate, built out with real numbers.
- **Forces vertical-specific compliance routing** — gaming's responsible-gambling rules replace a generic
  "make sure it's compliant" line, exposing the gap between operator-level and merely competent answers.
- **Exercises all eight rubric dimensions**, not a subset — business framing, data lineage, attribution
  reasoning, compliance, failure-mode handling, human-in-the-loop governance, executive artifact quality,
  and AI-use maturity all have a concrete trigger built into the scenario.
- **Matches the skill's own Exercise Build Pattern** — ambiguous one-page brief, disclosed-but-unweighted
  scoring, four required deliverables, and a scored *prompt* rather than a scored final answer.
- **Diversifies away from the skill's existing worked example** — the reference pharma scenario (Health
  Media Hub / FDA OPDP) already anchors a SHIPS example; testing gaming instead checks whether judgment
  generalizes across verticals rather than pattern-matching to a seen example.
- **Preserves the skill's disclosure requirement by design** — Greg states up front that scoring is
  happening, keeping the exercise inside the skill's disclosed-evaluation rule even with the rubric and the
  Cutler Layer's identity withheld.

---

## Source Documents

- `Master Prompt — The DraftKings Reallocation Call` (Cutler Layer Answer Key — not for participant distribution)
- `Havas Edge Director-Level Stress-Test Exercise — Use Case Brief`
- `Cutler Layer | DraftKings Reallocation — Master Prompt Scorecard` (scoring visualization)

---

*Epoch Frameworks LLC | Prepared for internal use in Havas Edge / Greg Cutler engagement design | Erwin Maurice McDonald | DACR License v2.6*
