# Drills — how to run one

One subfolder per drill, one file per drill. This file is the shared part — read it before
running a drill; the drill's own `context.md` carries what it trains, how it is graded, and
the operating instruction to adopt.

**Drills available:**

| Drill | Register | When to pick it |
|---|---|---|
| `dating-frame` | Status pressure — probing questions, shit-tests, late cancellations, vulnerability checks. | The relationship is new or exitable and the pressure is a test. |
| `saying-no` | Obligation pressure at work and in the family — guilt-trips, unasked-for advice, assumed favours. | The relationship does not end, and the cost of the reply outlives the exchange. |

Offer both when the practitioner hasn't said which. They share `../principles.md` and this
procedure; their dimensions differ because the registers differ.

## Running one

"Continue with the drills" (or similar) is the request this answers. Don't ask for a
prompt, don't invent a drill.

1. **Pick the menu source, highest first:**
   - **The private layer's cue set** (`cueues.md`, in the private area orientation
     reports), if there is one. It already names the single active target and the queue;
     use that directly rather than re-deriving a menu. Nothing else in the private area is
     a drill menu — the sprint log belongs to `../reps/`.
     **Read the cue set, never advance it** — proposing a slot or a reorder is fine when
     asked, but moving the active pointer or writing a ruling is the practitioner's call on
     real-world rep evidence from `../reps/`, never on drill performance.
   - **The bank**, if there's no private layer or it's silent on what's next — patterns it
     flags as unfinished (`../memory/small-bank.md`).
   - **`../principles.md`**, only if neither source gives a signal.

   The drill's tracked `context.md` owns scenario *classes* — method, fork-safe. The
   private layer only supplies which class is live and a session's throwaway texture; that
   texture never gets written back to a tracked file.

2. **Read the drill's own `context.md`** — it is not auto-injected. Adopt its operating
   instruction; don't hand it over. `./<name>/calibration.md`, where one exists, is read
   only when the drill is revised or a grade feels off.

3. **Run it here.** You are the simulator. Grade every dimension, both failure directions.
   If the private layer named an active cue in step 1, close every rep with a footer
   `Active cue: <line>` — the cue's numbered `**N. Title** → action` header line copied
   verbatim from the private file. Exact wording, repeated; not a paraphrase.

4. **Don't hand-write the bank.** Capture is automatic via `../memory/this-bank-prompt.md`'s
   de-identifying transform.

5. **A calibration entry is written private-first.** The transform in step 4 de-identifies
   the *counterparty*; it has nothing to say about the practitioner's own words, and a
   generified scenario with his verbatim reply still under it is not safe to track. So the
   entry — scenario, verbatim reply, per-dimension reasoning, calibrated contrast — is
   written to `<private area>/social-dynamics/calibration-entries.md`. What lands in the
   tracked `./<name>/calibration.md` is a row in its index: the scenario *class*, the reply
   *class*, the correct grade, and what the entry is in the set to catch. **The reply text
   never lands, in any form** — not quoted, not paraphrased, and not in a commit message.

## The ceiling

Text drills train recognition and having a reply ready (rungs 1–2 of `../principles.md`),
not composure under real pressure (rung 3) — that needs `../reps/`. See `../research/`.

## Why this file exists at all

The shared "how to run a drill" procedure lives here rather than in `../DAFNE.md`, so the
always-loaded manifest carries a routing table and the one turn-1 rule, and the procedure
is read at the moment it applies. The *new* part of that shape is a mid-level directory
context sitting between the manifest and a leaf.

Recorded because it is a pattern other groves could inherit, and inheriting it by accident
is worse than adopting it deliberately. Nothing in the engine knows about it — only a
manifest's YAML frontmatter is machine-read, so this is a convention, not a contract. It
has **not** been promoted to the orchestrator's architect layer; if a second grove wants
the same shape, promote it there rather than copying this directory.
