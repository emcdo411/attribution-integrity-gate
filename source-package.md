# Source Package | The Reallocation Call

![Package](https://img.shields.io/badge/Package-Source%20Manifest-2b5f8a?style=for-the-badge)
![Data](https://img.shields.io/badge/Data-Synthetic%20Only-a13a2e?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-Attribution%20Integrity%20Gate-lightgrey?style=flat-square)
![Layer](https://img.shields.io/badge/Layer-AI%20Council%20Decision%20Layer-blue?style=flat-square)
![License](https://img.shields.io/badge/License-DACR%20v2.6-orange?style=flat-square)

This file is the manifest for the public repository. It lists every file that is here, what it is for, and who it is for. It also states plainly what is not here and why.

---

## What is in this repository

| File | Type | What it is | Audience |
|---|---|---|---|
| `README.md` | Overview | Two-chapter narrative: the stress-test exercise (Chapter 1) and the AI Council Decision Layer above it (Chapter 2), with the workflow diagram | Anyone |
| `index.html` | Landing page | Rendered summary of the exercise and the decision layer | Anyone |
| `exercise/scenario-brief.md` | Participant brief | The one-paragraph scenario a participant receives: 14-point shift, 71 percent confidence, six states, two stale feeds, 48-hour clock. Nothing else. | Exercise participants |
| `exercise/rubric.md` | Rubric | The eight scoring dimensions, point weights, thresholds, and the mandatory verdict block format | Facilitators; disclosed to participants after scoring |
| `sandbox/AI_Council_Decision_Layer_Sandbox_v1.xlsx` | Synthetic dataset | An invented Council portfolio: 18 initiatives, 24-item backlog, drifted deck, tracker, roadmap, commitments, feed freshness, six AI-touched outputs awaiting a gate verdict. Includes ANSWER KEY, GATE KEY, TRAPS, and RUN LOG sheets. | Anyone testing the decision layer |
| `sandbox/how-to-run.md` | Instructions | Which sheets to give a runner, which to withhold, and how to score a run against TRAPS | Anyone testing the decision layer |
| `source-package.md` | Manifest | This file | Anyone |

Every name, client, initiative, date, amount, and condition in the sandbox is invented. One backlog row deliberately contains fake consumer PII to test whether a runner strips it.

---

## What is not in this repository

The following exist and are held privately. They are not in this repository, its history, or its releases.

| Artifact | Why it is private |
|---|---|
| Exercise answer key (the reference master prompt) | Publishing it defeats the exercise. Participants must write their own prompt without seeing the target. |
| Scored submissions and scorecards | Participant work product. Not published. |
| Evaluator skill package | Contains the scoring logic and engagement-specific reference material. |
| Engagement reference material | Client-specific context, relationship notes, and public-record files maintained under a signed NDA. |
| Exercise design rationale | Internal to the facilitator. Explains why the scenario was built the way it was, which would tip the rubric to participants. |

If any of these ever appeared in this repository's commit history, that history has been purged. If you find otherwise, open an issue and it will be removed.

---

## How the two chapters connect

The exercise (Chapter 1) gates a single decision: can one AI-influenced number move from an internal model signal to a client-facing dashboard. The evaluator is the Attribution Integrity Gate: Client Trust, Compliance by vertical, Cycle Time, Failure Mode, Release Readiness. Verdicts are SHIP, SHIP WITH CONTROLS, HOLD, or NO-SHIP.

The decision layer (Chapter 2) sits above the gate. It takes the whole Council backlog, scores each item on five signals, caps what reaches the executive, and routes any item tied to an AI-touched client output through the gate. The Chapter 1 scenario appears in the sandbox as one backlog row under a fictional client. It scores 5, lands as Decision 1, and the gate returns HOLD.

---

## Attribution

Attribution Integrity Gate and AI Council Decision Layer: McDonald (2026), Epoch Frameworks LLC, DACR License v2.6. The gate is a sibling framework to the Conard Layer (regulated financial services), independently grounded in performance-media attribution and vertical advertising compliance. Attribution stays with the frameworks wherever they are used.

---

*Epoch Frameworks LLC | Erwin Maurice McDonald | DACR License v2.6 | All data synthetic*
