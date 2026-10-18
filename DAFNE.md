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
maintaining boundaries without over-explaining, justifying, or acting needy. The core is a
conversational **simulator** (it throws a scenario, you respond, it grades you) plus the
**principles** that define a good response. Text-only; drills run as LLM conversations.

**"Continue with the drills" is the main interface to this grove.** When the practitioner
says that, or anything like it: do not ask them to supply a prompt, and do not invent a
drill. Read `./drills/context.md` — it owns how a drill is picked and run.

## Where to look

| Path | What |
|---|---|
| `./memory/small-bank.md` | This grove's memory — recent sessions, and which failure *this* practitioner keeps repeating. **Read it now if it is not already in your context**; depending on how the grove was opened it may not have been injected. Empty or missing means nothing captured yet, which is normal, not broken. |
| `./drills/context.md` | **How to run a drill** — picking the resume point, which files to adopt, how to grade. Read before running one. |
| `./drills/<name>/` | One self-contained drill: its own index, rubric, and simulator. `dating-frame` is the only one built. |
| `./principles.md` | What good looks like under social pressure — calibrated assertiveness, and the failure modes in *both* directions. The target every drill trains toward. |
| `./research/` | Whether a text simulator builds boundary skills at all: efficacy evidence, and this grove's honest ceiling. |
| `./reps/` | Real-world rep loops. `catch-log.md` is sprint 1, with its own cue, capture surfaces and ruling. The one place this grove produces evidence instead of consuming it. |
| `./improvement-plan.md` | What is deliberately not built yet, in priority order, with the reasoning. Consult before proposing a change to this grove. |
| `./artifacts/` | Grove-level artifacts, incl. `social-dynamics-grove-plan.md` — the original turnkey build plan this grove was created from, and the seams left unbuilt. |
| `./parents/behavior-rewiring/` | Parent node — **how behavior changes**: mechanism, evidence graded A–F (several popular claims fail), reusable rep protocols. Read **before designing any drill or rep loop**; read in place, and let its own `DAFNE.md` route you inside. |

**The division of labour with the parent: it knows how behavior changes; this grove knows
what good looks like under social pressure.** Don't re-derive mechanism here, and don't put
drill content there.
