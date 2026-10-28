# Social Dynamics — Improvement Plan

What is deliberately not built yet, and why. Consult before proposing a change to this
grove. Items that shipped are listed at the bottom in one line each — the reasoning that
is still load-bearing lives in the files they produced, not here.

**Outstanding: one item.** A calibration set for `saying-no`. Everything else in this file
is either running or done.

## 1. Calibration set for `saying-no` — **open**

**Why.** The grader *is* the mechanism — it is the "feedback" in instruction → modeling →
rehearsal → feedback (`research/does-low-stakes-simulation-build-boundary-skills.md` §2).
If it mis-grades, the drill trains the wrong reflex, and since the modeling step shipped
the grader also asserts what right looks like, which is a faster route to a confident
wrong reflex than mis-scoring alone. `drills/dating-frame/calibration.md` closed this for
the first drill — six entries spanning missed detection, invented detection, hostility and
coldness, plus one calibrated reply so over-harsh drift is detectable too.

**What.** The same artifact for `saying-no`, where the risk is sharper: its **Cost**
dimension judges a relationship the grader cannot see.

**Intake, not an authoring project.** The modeling step produces, in live reps, exactly
what this artifact contains — a worked example with its per-dimension reasoning attached.
What this needs is the habit of recording those, not an afternoon of inventing them.
**Effort:** low. **Leverage:** high.

## 2. Real-world rep loop — **running (sprint 1)**

The only item here that generates evidence instead of consuming it, and the only route to
rung 3 (composure under real pressure), which no text drill reaches.

Instantiated and split along the method/instance seam: `reps/context.md` holds the grove's
half — cue form, the residue discriminator, the three-surface capture pattern, the rollup
schema — and the live sprint (target, baseline, weekly numbers, ruling) is one
practitioner's and lives in the private layer. The protocol itself is the parent's
(`parents/behavior-rewiring/protocols/single-target-sprint.md`); this grove supplies the
domain, never a second copy of the loop.

**It is waiting on reps, not on work.** Nothing here is blocked by item #1.

---

## Shipped

| What | Where it landed |
|---|---|
| Detection scored first; both failure poles per dimension; soft and non-crossing scenarios in the mix | `drills/dating-frame/context.md` |
| Grove-level target broadened from "hold frame" to calibrated assertiveness | `principles.md` |
| Second drill for obligation pressure — not a reskin: non-exitable relationship, delay legitimate, its own dimensions | `drills/saying-no/context.md` |
| Grader-calibration artifact for the first drill | `drills/dating-frame/calibration.md` |
| Modeling step — tier 1 names the missing move every rep, tier 2 gives one example line on request or a bad miss. Rationale: the parent's if-then anchor is the best-evidenced mechanism in the area, and a grade cannot become an anchor | both drills' `context.md` |
| Register dimension split — coldness graded as either L2/corporate-email lexical transfer or protective distance, because the two need different fixes | `drills/dating-frame/context.md` |
| One file per drill — grading dimensions and the simulator instruction folded into each drill's `context.md`, superseded simulator drafts dropped to git history | `drills/*/context.md` |

---

## Structural note — `drills/context.md` is a grove-local choice

The shared "how to run a drill" procedure lives in `drills/context.md` rather than in
`DAFNE.md`, so the always-loaded manifest carries a routing table and the one turn-1 rule,
and the procedure is read at the moment it applies. The *new* part of that shape is a
mid-level directory context sitting between the manifest and a leaf.

Recorded here because it is a pattern other groves could inherit, and inheriting it by
accident is worse than adopting it deliberately. Nothing in the engine knows about it —
only a manifest's YAML frontmatter is machine-read, so this is a convention, not a
contract. It has **not** been promoted to the orchestrator's architect layer; if a second
grove wants the same shape, promote it there rather than copying this directory.
