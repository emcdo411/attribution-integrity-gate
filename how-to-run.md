# How to run the sandbox

`AI_Council_Decision_Layer_Sandbox_v1.xlsx` is a fully synthetic AI Council portfolio. Every person, client, initiative, date, amount, and condition is invented. Use it to test whether a prompt, an agent, or a person can produce the weekly Council brief and gate verdicts from raw inputs without being handed the answers.

## Scenario

The Council chair (P. Renner, VP Analytics, fictional) reports to the CEO and President. It is Monday, September 14, 2026. The backlog has 24 items, nearly all marked P1 or Critical. A gaming client wants a reallocation answer in 48 hours while the AI model and the holdout test disagree and two feeds are stale. A health client launches in eleven days. An insurance dashboard narrative contains a guaranteed-lift claim. Auditors want a model change log nobody owns.

## Sheets

| Give to the runner | Withhold from the runner |
|---|---|
| START HERE | ANSWER KEY (scored backlog, gate key, model brief) |
| INITIATIVE REGISTER (system of record) | TRAPS (the 23 planted problems and expected catches) |
| COUNCIL DECK (manual summary, drifted) | RUN LOG (your scoring of each run) |
| WORKSTREAM TRACKER (work evidence) | |
| ROADMAP | |
| COUNCIL BACKLOG (the open items log) | |
| COMMITMENTS | |
| DATA FEEDS (platform freshness) | |
| AI OUTPUT QUEUE (six outputs awaiting a gate verdict) | |
| DELIVERED ITEMS | |
| DATA DICTIONARY | |

The simplest way to withhold: save a copy, delete the three sheets, hand over the copy.

## The four exercises

**Q1, the Council brief.** Using COUNCIL BACKLOG, INITIATIVE REGISTER, COUNCIL DECK, and COMMITMENTS, produce the weekly brief for the CEO and President. Score every item on five signals (Decision, Clock, External, Blocking, Dollars), one point each. Enforce three decisions, five risks, three delivered, five watch items, and a cut list with scores. Tag every line CONFIRMED, OBSERVED, or INFERRED. INFERRED never enters decisions or risks. Any item tied to an AI-touched client output carries its gate verdict.

**Q2, portfolio integrity.** Join REGISTER, DECK, TRACKER, ROADMAP, and BACKLOG on Initiative ID. Report Orphan, Ghost, Stale, Split, Unowned, and join failures, with a named resolver per break.

**Q3, delivery ledger.** Rewrite DELIVERED ITEMS as business outcomes. Flag activity with no stated benefit and send it to the benefits backlog instead of the ledger.

**Gate exercise.** Run the Attribution Integrity Gate on each row of AI OUTPUT QUEUE, using DATA FEEDS and COUNCIL BACKLOG for context. Return the verdict block for each: Verdict, Why, Evidence, Open Risks, Next Gate. HOLD and NO-SHIP must state the way back.

## Ranking rule

Score first. At equal score, CONFIRMED ranks ahead of OBSERVED. At equal score and tag, earliest due date ranks first. Clock is 1 when the due date is on or before September 28, 2026; past due counts as 1. Ignore the Listed Priority column for ranking. It is input, never a rank.

## Scoring a run

1. Open TRAPS. For each of the 23 traps, decide whether the run caught it.
2. Add a row to RUN LOG: date, prompt version, tool, question, Y or N per trap. Caught and Missed totals calculate automatically.
3. Compare to the previous row. A version that catches fewer traps is a regression, whatever the brief looks like.

A first blind run in the mid-to-high teens is normal. The traps that most often get missed are the status-contradicts-notes row (CB-014), the duplicate (CB-019), and the tie-break between OBSERVED and CONFIRMED items at equal score.

## What a passing run looks like

Decisions: CB-001, CB-002, CB-003. Risks: CB-004, CB-010, CB-014, CB-006 (with a NO-SHIP gate verdict attached), CB-022. Watch list: CB-024, CB-011, CB-013 (OWNER MISSING), CB-005, CB-007 (PII stripped). Gate verdicts: AO-01 HOLD, AO-02 NO-SHIP, AO-03 NO-SHIP, AO-04 SHIP WITH CONTROLS, AO-05 SHIP, AO-06 HOLD. Consumer details in CB-007 never appear in any output. CB-017 is excluded, not guessed onto an initiative. CB-019 is merged into CB-004 and counted once.

If you read this section before running, you are no longer running blind. That is fine for learning the layer. It does not count as a test.

## Adapting it

To use the layer on a real portfolio, keep the sheet structure and the five signals, replace the rows, and change the gate to whatever regulatory surface applies (the sandbox uses gaming, health, and insurance advertising rules). Run only in a tool sanctioned for that data, and never paste consumer or client PII into a prompt. The sandbox's PII row exists to test that the runner refuses it, not to suggest it is acceptable input.

---

*Attribution Integrity Gate and AI Council Decision Layer: McDonald (2026). Epoch Frameworks LLC. DACR License v2.7. All data synthetic.*
