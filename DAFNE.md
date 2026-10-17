---
format: 0
banks:
  - name: social-dynamics
    bank: ./memory
    graduate: false
    patterns:
      - "social-dynamics/memory/context\\.md"
---

# social-dynamics — frame-control drills grove

Training enclave for holding a strong, unbothered, playful frame under social pressure —
maintaining boundaries without over-explaining, justifying, or acting needy.

The grove's core is a conversational **simulator** (it throws a scenario, you respond, it
grades you) plus the **principles** that define a good response. It is text-only; drills
run as LLM conversations. Optional later tools (Anki leak-log, web-research evidence)
are noted as seams in the repo-root build plan, not built; DAFNE parenthood is built —
see Parents below.

Read `./memory/context.md`

## Files in this area

| Path | What |
|---|---|
| `./principles.md` | Cross-cutting theory shared by every drill: the target (calibrated assertiveness) and the failure modes to catch in both directions. |
| `./drills/` | One subfolder per training drill. Each drill is self-contained: its own index, grading rubric, and versioned artifacts. |
| `./drills/dating-frame/` | Frame-control under dating pressure (probing questions, shit-tests, late cancellations, vulnerability checks). **The only drill so far.** |
| `./research/` | Collected efficacy evidence ("artifact proofs") on whether such simulations work. |
| `./improvement-plan.md` | Deferred, research-motivated changes to the grove (grader calibration, recognition scoring, a `saying-no` drill, the leak-log loop). |
| `./artifacts/` | Grove-level artifacts, incl. `social-dynamics-grove-plan.md` — the original turnkey build plan this grove was created from. |
| `./parents/behavior-rewiring/` | Parent node — shared theory on how an understood intention becomes an automatic behavior. Read in place; see below. |

## Parents

`parents/behavior-rewiring` — the base node holding theory, sources, and curation
decisions on deliberate behavior change, shared with future practice groves rather than
owned privately here.

The relationship is **semantic reference**: sessions in this grove read those files in
place. There is no compile step in this grove and mounting a parent does not add one —
`#include ./parents/behavior-rewiring/...` stays available for if a drill prompt ever
becomes layered, but it is one use of the relationship, not its definition.

The node is near-empty at mounting time (2026-10-17) — only its manifest and a
population plan. The first place its content has to earn its keep is
`improvement-plan.md` item #4, the leak-log: turning real-world attempts and misses into
a loop that feeds back into drills is exactly the "real-time friction" step that node's
theory is about.
