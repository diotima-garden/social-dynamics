---
format: 0
banks:
  - name: social-dynamics
    bank: ./memory
    graduate: false
    patterns:
      # Fallback only: when the session's subject IS this grove the orchestrator sets
      # in_session_scope and these are not consulted. They exist for a session run from
      # elsewhere (master, another grove) that works on this one, so they name the
      # surfaces such a session actually touches, not the bank's own index file.
      - "social-dynamics/(drills|reps|memory)/"
      - "social-dynamics/(principles|improvement-plan)\\.md"
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
| `./drills/<name>/context.md` | One self-contained drill in one file: what it trains, its grading dimensions, and the simulator instruction to adopt. `dating-frame` and `saying-no` are built; the former also carries a `calibration.md`. |
| `<private area>/social-dynamics/` | User private files like cues and behavioural patterns. |
| `./principles.md` | What good looks like under social pressure — calibrated assertiveness, and the failure modes in *both* directions. The target every drill trains toward. |
| `./research/` | Whether a text simulator builds boundary skills at all: efficacy evidence, and this grove's honest ceiling. |
| `./reps/` | Real-world rep loops. `context.md` is how a sprint is designed here — cue form, the residue discriminator, capture, schema. The one place this grove produces evidence instead of consuming it. The live sprint is private, not here. |
| `./improvement-plan.md` | What is deliberately not built yet, in priority order, with the reasoning. Consult before proposing a change to this grove. |
| `./parents/behavior-rewiring/` | Parent node — **how behavior changes**: mechanism, evidence graded A–F (several popular claims fail), reusable rep protocols. Read **before designing any drill or rep loop**; read in place, and let its own `DAFNE.md` route you inside. |

**The division of labour with the parent: it knows how behavior changes; this grove knows
what good looks like under social pressure.** Don't re-derive mechanism here, and don't put
drill content there.
