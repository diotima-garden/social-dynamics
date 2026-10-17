# Social Dynamics — Improvement Plan

Deferred changes surfaced by the efficacy research
(`research/does-low-stakes-simulation-build-boundary-skills.md`). Items #1–#3 from that
review are already applied (recognition scoring, over-assertion failure modes, grove-level
principle broadened to calibrated assertiveness). What remains, in priority order:

## 1. Grader-calibration artifact — do first
**Why:** the research finding is that the LLM grader *is* the mechanism — it's the "feedback"
in instruction → modeling → rehearsal → feedback. If it mis-grades (rewards a smooth line
that would land badly, or flags a healthy boundary as "needy"), the drill trains the wrong
reflex. Its validity is currently unvalidated, so it silently underwrites everything else.
**What:** add `drills/dating-frame/calibration.md` — a small gold-standard set: worked
example responses, their correct grade on each rubric dimension, and *why*. Anchors the
grader to `principles.md` and gives a way to spot drift when the simulator is regenerated.
**Effort:** low. **Leverage:** high (de-risks the whole grove).

## 2. Score recognition explicitly in the live drill
**Why:** recognition is rung 1 and the highest-yield capacity for the target profile (the
appeaser who doesn't register the crossing). `principles.md` now names it and `rubric.md`
adds a **Detection** dimension — but the live simulator artifact
(`drills/dating-frame/artifacts/soc-dynamic-gemini-first-attempt.md`) predates this and
doesn't yet throw *ambiguous/soft* crossings or grade whether they were flagged.
**What:** revise the simulator prompt to include soft-test scenarios and to grade Detection.
**Effort:** low–medium. **Leverage:** high (it's the rung this profile fails first).

## 3. Second drill: `drills/saying-no/` (work / family)
**Why:** the "swallowing boundary-crossings" profile shows up *most* outside dating —
guilt-trips, unreasonable asks at work. Dating-frame is a narrow instance of a broad problem;
the principles are already drill-agnostic, so the seam exists.
**What:** new drill folder (context + rubric + simulator artifact) for non-dating boundary
pressure. Reuse `principles.md`; define drill-specific dimensions.
**Effort:** medium. **Leverage:** medium (coverage of the real target contexts).

## 4. Activate the leak-log as a real-world rep loop
**Why:** `DAFNE.md` notes an Anki leak-log as a *future* seam. The research now motivates
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
