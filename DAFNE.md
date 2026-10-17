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
are noted as seams in `artifacts/social-dynamics-grove-plan.md` §5, not built; DAFNE
parenthood is built — see Parents below.

Read `./memory/context.md`

## Files in this area

| Path | What |
|---|---|
| `./principles.md` | The stance shared by every drill: the target (calibrated assertiveness) and the failure modes to catch in both directions. Not theory of change — that's the parent's. |
| `./drills/` | One subfolder per training drill. Each drill is self-contained: its own index, grading rubric, and versioned artifacts. |
| `./drills/dating-frame/` | Frame-control under dating pressure (probing questions, shit-tests, late cancellations, vulnerability checks). **The only drill so far.** |
| `./research/` | Collected efficacy evidence ("artifact proofs") on whether such simulations work. |
| `./reps/` | Real-world rep loops — the parent's sprint protocol instantiated for this grove's cue. `catch-log.md` is sprint 1 (recognition only). The one place this grove produces evidence instead of consuming it. |
| `./improvement-plan.md` | Deferred, research-motivated changes to the grove (grader calibration, recognition scoring, a `saying-no` drill, the leak-log loop). |
| `./artifacts/` | Grove-level artifacts, incl. `social-dynamics-grove-plan.md` — the original turnkey build plan this grove was created from. |
| `./parents/behavior-rewiring/` | Parent node — the theory of behavior change, its evidence grades, and reusable rep-loop protocols. Read in place; routing table below. |

## Parents

`parents/behavior-rewiring` (populated 2026-10-17) holds the **theory of behavior change**
for this grove and its future siblings. Read those files **in place** — the relationship is
semantic reference, not compilation.

**The division of labour: the parent knows how behavior changes; this grove knows what
good looks like under social pressure.** So don't re-derive mechanism here, and don't put
drill content there. Where to look:

| If you're asking | Read |
|---|---|
| How does an intention become automatic? How many changes at once? | `parents/behavior-rewiring/principles.md` — **before designing any drill or rep loop** |
| Is this claim actually evidenced? | `parents/behavior-rewiring/sources.md` (graded A–F; several popular claims are **F**) |
| How do I run a rep loop / force interception? | `parents/behavior-rewiring/protocols/` — single-target sprint, delay rule |
| Is this settled or still a bet? | `parents/behavior-rewiring/open-questions.md` |
| What counts as a good response to social pressure? | `./principles.md` (this grove) |
| Does a text simulator work for *boundary* skills? | `./research/` (this grove) |

The first place the parent earns its keep is `improvement-plan.md` item #4, the leak-log:
it is now an *instantiation* of `protocols/single-target-sprint.md` for a social cue rather
than a loop this grove has to design.
