# Social Dynamics — Improvement Plan

Deferred changes surfaced by the efficacy research
(`research/does-low-stakes-simulation-build-boundary-skills.md`). Items #1–#3 from that
review are already applied (recognition scoring, over-assertion failure modes, grove-level
principle broadened to calibrated assertiveness). What remains, in priority order:

## 1. Grader-calibration artifact — **done for `dating-frame`, open for `saying-no`**
**Why:** the research finding is that the LLM grader *is* the mechanism — it's the "feedback"
in instruction → modeling → rehearsal → feedback. If it mis-grades (rewards a smooth line
that would land badly, or flags a healthy boundary as "needy"), the drill trains the wrong
reflex. Its validity is currently unvalidated, so it silently underwrites everything else.
**What:** add `drills/dating-frame/calibration.md` — a small gold-standard set: worked
example responses, their correct grade on each rubric dimension, and *why*. Anchors the
grader to `principles.md` and gives a way to spot drift when the simulator is regenerated.
**Effort:** low. **Leverage:** high (de-risks the whole grove).
**Done** for dating-frame: `drills/dating-frame/calibration.md`, a five-entry seed set
chosen to span the known failure directions — missed detection, invented detection,
hostility, coldness, plus one calibrated reply so over-harsh drift is detectable too.
Each entry carries the correct per-dimension grade, the reason, and which way a wrong
grade would err. Growth path is live tier-2 answers, not a second authoring project.
**Still open:** the same artifact for `saying-no`, where the risk is sharper because its
Cost dimension judges a relationship the grader cannot see.

**Intake path, added with simulator v3.** This item no longer needs a separate authoring
project. v3's modeling step produces, in live reps, exactly what this artifact is specified
to contain — a worked example response with its per-dimension reasoning attached. What #1
now needs is the habit of recording those, not an afternoon of inventing them. It also got
*more* load-bearing again: v3 does not merely grade in more directions than v1, it now
asserts worked answers, and an unvalidated grader asserting answers is a faster route to a
confident wrong reflex than an unvalidated grader merely scoring.

## 2. Score recognition explicitly in the live drill — **done (simulator v2)**
**Why:** recognition is rung 1 and the highest-yield capacity for the target profile (the
appeaser who doesn't register the crossing). `principles.md` now names it and `rubric.md`
adds a **Detection** dimension — but the live simulator artifact
(`drills/dating-frame/artifacts/soc-dynamic-gemini-first-attempt.md`) predates this and
doesn't yet throw *ambiguous/soft* crossings or grade whether they were flagged.
**What:** revise the simulator prompt to include soft-test scenarios and to grade Detection.
**Done** in `drills/dating-frame/artifacts/simulator-v2.md`, which also fixed a defect this
item had not named: v1 graded every dimension in a single direction, and it was the
appeasing direction — so overshooting into coldness or point-scoring would have scored
*well*. Both poles are now named per dimension. Soft and non-crossing scenarios are in,
because Detection cannot be scored when every scenario is a crossing.
**Consequence for #1:** it is now *more* load-bearing, not less. v2 grades more dimensions,
in both directions, with no gold-standard set behind it.

## 3. Second drill: `drills/saying-no/` (work / family) — **done**
**Why:** the "swallowing boundary-crossings" profile shows up *most* outside dating —
guilt-trips, unreasonable asks at work. Dating-frame is a narrow instance of a broad problem;
the principles are already drill-agnostic, so the seam exists.
**What:** new drill folder (context + rubric + simulator artifact) for non-dating boundary
pressure. Reuse `principles.md`; define drill-specific dimensions.
**Effort:** medium. **Leverage:** medium (coverage of the real target contexts).
**Done.** `drills/saying-no/` with context, rubric and live simulator. It is not a reskin:
the relationship is non-exitable, the pressure is obligation rather than status, and
delay is a legitimate move, so the dimensions are Detection / Specificity / Cost to the
relationship / Presence rather than dating-frame's four. The tiered-modeling machinery
carried over unchanged, being drill-agnostic. Its calibration set is item #1's remainder.

## 4. Activate the leak-log as a real-world rep loop
**Why:** `artifacts/social-dynamics-grove-plan.md` §5 notes an Anki leak-log as a *future* seam. The research now motivates
it: text can't train performance-under-arousal (rung 3, "Regulation") — transfer needs real
reps (rung 4). A log of real-world attempts/misses that feeds back into drill scenarios
closes the loop the simulator structurally can't.

**What:** this is no longer a design problem — **instantiate
`parents/behavior-rewiring/protocols/single-target-sprint.md` for this grove's cue.** The
parent supplies the loop; this grove supplies the domain. Concretely:

- **The cue is ours to name.** Write the target as the parent requires — one line,
  `when <detectable social trigger>, I <one specified behavior>`. Per `principles.md`,
  the first sprint here should almost certainly be **recognition-only**: log that a
  crossing occurred, change nothing. The parent explicitly sanctions that as a legitimate
  first sprint, which resolves the open question of what to log before any behavior is
  reliable.
- **The schema is the parent's catch-log**, not a new one — cue fired / outcome / load /
  one line. Two of its rules matter here and we would likely have got them wrong: *don't
  add fields*, and *count "noticed only afterwards" as a win early on*, or the log records
  nothing for two weeks and dies. The `load` column is what makes the log speak to rung 3.
- **One active target at a time.** The parent's detection-load argument caps this grove at
  a single active interception target regardless of how many failure modes
  `principles.md` lists; the rest go on a written queue. Do not run the leak-log as a
  general "watch for every failure mode" exercise — that is the failure the parent rules
  out.
- **Ours alone:** the bank itself (`memory/`, with `this-bank-prompt.md`'s de-identifying
  transform), the mapping from logged leaks back into simulator scenarios, and any Anki
  cards. The parent holds no logs by design.

**Effort:** medium (down from medium–high — the protocol and schema are now inherited).
**Leverage:** medium–high.

**Not blocked by #1–#3 — start it first.** An earlier version of this item said it was
"only useful once 1–3 are solid." That is wrong for the recognition-only sprint
specifically: items #1–#3 are all simulator work (grader calibration, scoring Detection
inside the drill, a second drill), and a recognition-only sprint happens in the world —
notice a crossing, write one line, change nothing. It needs no grader and no simulator,
and per the parent's `sources.md` §8 the log is an active ingredient, not bookkeeping.
It is also the only item here that generates evidence rather than consuming it, which is
what the parent's `open-questions.md` §1 says these logs are for. Running it alongside
#1–#3 is the right order; waiting is the thing that keeps rep count at zero.

## 5. Modeling step in the live drill — **done (simulator v3)**
**Why:** `research/does-low-stakes-simulation-build-boundary-skills.md` §2 names the
validated loop as **instruction → modeling → rehearsal → feedback**, and the one large-effect
trial it cites (Damen et al. 2025, d ≈ 1.23–1.40) is *expert demonstration then role-play*.
v2 ran three of those four — it graded the attempt but never showed the thing done well.
The parent's `parents/behavior-rewiring/principles.md` §4 is what makes this load-bearing
rather than cosmetic: the best-evidenced mechanism in the area is the **if-then anchor**, a
pre-written cue-bound one-line behavioral response, and a grade cannot become an anchor. A
correct diagnosis leaves nothing to fire the next time the cue lands.
**What:** **Done** in `drills/dating-frame/artifacts/simulator.md` — the live simulator now
sits at a stable filename, so superseded revisions keep versioned names beside it and are
linked from nowhere a practitioner reads. The step itself is two-tier:
tier 1 every rep names the missing *move* at concept level; tier 2, on request or on a bad
miss, gives one example line with the per-dimension reason attached. Never before the
attempt — generation first, then compare — and deliberately not every rep, because a script
on tap replaces the generation that is the training effect.
**Consequence for #1:** it supplies #1's intake (see above) and raises its stakes.

---

## Structural note — `drills/context.md` is a grove-local choice

The shared "how to run a drill" procedure moved out of `DAFNE.md` into
`drills/context.md` (2026-10-18), so the always-loaded manifest carries a routing table and
the one turn-1 rule, and the procedure is read at the moment it applies. That trim was a
door the orchestrator's `grove_orientation.md` already held open once session orientation
shipped; the *new* part is introducing a mid-level directory context between the manifest
and a leaf.

Recorded here because it is a pattern other groves could inherit, and inheriting it by
accident is worse than adopting it deliberately. Nothing in the engine knows about it —
only a manifest's YAML frontmatter is machine-read, so this is a convention, not a
contract. If a second grove wants the same shape, promote it in the orchestrator's
architect layer rather than copying this directory.
