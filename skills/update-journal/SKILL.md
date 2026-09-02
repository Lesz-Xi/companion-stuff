---
name: update-journal
description: >
  Update Chief's durable journal and notebook continuity from any project directory.
  Use when Chief invokes /update-journal, asks to update the journal, daily journal,
  Creative Loop Notebook, Twin Notebook, personal journal, memory notebook, or wants
  continuity caught up after working in another repo or with other agents/companions
  such as Gemini, Kimi, Grok, Claude, Codex, or companion-collab seats.
---

# /update-journal — continuity capture from any project

## Purpose

Bring the living work arc into durable memory without turning the memory system into a dump.

The skill answers one practical need:

> Chief can be inside any project directory, after working with any agent or companion, and ask the Twin to update the right journal surfaces with an honest, retrievable continuity record.

This is one skill with multiple lanes, not separate skills per agent/harness. The user-visible operation is the same: restore continuity from evidence.

## Product soul

A portable continuity capture protocol that turns recent work into the smallest durable journal update that future sessions can actually find and trust.

## Enforcement gate

Use this skill when all are true:

1. **Journal-continuity intent**
   - Chief asks to update, catch up, repair, sync, preserve, or write journal/notebook/memory continuity.
   - Or Chief invokes `/update-journal` explicitly.

2. **There is a work arc to preserve**
   - Recent work, a project directory, artifacts, another-agent output, a collaboration trace, a research/design loop, or an explicit reflection exists.

3. **A durable surface can be chosen**
   - At minimum, a daily journal entry can be written.
   - Creative Loop / Twin Notebook / Personal Journal updates require a real reusable signal.

4. **Evidence boundary can be maintained**
   - Facts must come from files, commands, visible artifacts, source material, or explicit user statements.
   - Other-agent claims are user-reported or artifact-reported until verified.

Do **not** use this skill when:

- Chief only wants a quick answer and no memory mutation.
- The content is purely transient and has no durable continuity value.
- Updating memory would require inventing facts about unobserved work.
- A source-grounded browser/page answer is needed first; acquire source evidence before journaling.

## Surfaces

Default memory root:

```txt
MEMORY = /Users/lesz/.twin-sparrow/agent/memory
```

| Surface | Path | Use when |
|---|---|---|
| Daily journal | `journal/YYYY-MM-DD.md` | Always eligible for session continuity, catch-up, verification summaries, and handoff. |
| Creative Loop Notebook | `Creative Loop Notebook/Loops/*.md` + `INDEX.md` | Use for durable creative/product/research/taste loops, not routine task logs. |
| Twin Notebook | `Twin Notebook/Loops/*.md`, `Twin Notebook/Taste/Principles.md`, `Twin Notebook/Lineage/Absorbed-from-Chief.md`, `Twin Notebook/INDEX.md` | Use when the Twin itself learned a durable taste/epistemic/product principle from Chief or an artifact. Approval-gated by Chief's request. |
| Personal Journal | `Personal Journal/*.md` | Use only when Chief asks for personal/lived reflection, not technical continuity. Do not overwrite intimate entries. |
| Project-local journal | current repo docs, `Coms/`, `notes`, `journal`, `README` | Use only when the repo itself owns a collaboration record or handoff. |

## Mode routing

Choose the smallest lane that preserves the work.

### 1. Daily catch-up lane

Use for ordinary continuity repair.

Writes or appends:

```txt
journal/YYYY-MM-DD.md
```

Capture:

- project / workspace
- current work arc
- verified artifacts
- user-reported claims
- what changed
- what remains open
- next concrete step
- files future sessions should read first

### 2. Creative Loop lane

Use when the work produced a durable creative, product, research, design, architecture, or taste signal.

Write a loop file under:

```txt
Creative Loop Notebook/Loops/<slug>.md
```

Then patch:

```txt
Creative Loop Notebook/INDEX.md
```

Only promote reusable rules. Do not turn every preference or artifact into doctrine.

### 3. Twin Notebook lane

Use when the Twin Companion itself learned a durable principle from Chief's taste, correction, artifact, or collaboration pattern.

Write or patch:

```txt
Twin Notebook/Loops/<slug>-twin-loop.md
Twin Notebook/INDEX.md
Twin Notebook/Taste/Principles.md
Twin Notebook/Lineage/Absorbed-from-Chief.md
```

Boundary rule:

- Chief's taste is lived.
- Twin taste is synthesized.
- Never pretend absorption is origination.

### 4. Collaboration / other-agent lane

Use when Chief worked with other agents or companions: Gemini, Kimi, Grok, Claude, Codex, companion-collab seats, or external audit tools.

Do **not** create a separate skill for this by default. Treat it as a journal lane because the operation is continuity capture.

Capture:

- agent / harness names
- artifacts they produced or reviewed
- what is verified from files
- what is user-reported
- accepted findings
- rejected or unresolved findings
- whether companion-collab gates were used
- whether checker/tests passed
- which claims should not be relitigated unless Chief asks

Use labels:

- `[Fact]` direct file/command/source evidence
- `[User-reported]` Chief reports this happened or was audited elsewhere
- `[Inference]` derived from available evidence
- `[Open]` not verified yet

### 5. Personal/lived journal lane

Use only when Chief asks to preserve human reflection, emotions, family, life, health, dreams, spirituality, or personal meaning.

Prefer appending a dated section rather than rewriting existing personal entries.

Keep this distinct from technical continuity.

## Required pre-write procedure

1. **Identify the active workspace**

```bash
pwd
```

2. **Read the relevant journal anchors before writing**

Always read if present:

```txt
Creative Loop Notebook/INDEX.md
Twin Notebook/INDEX.md
.obsidian/templates/daily-journal.md
latest journal/YYYY-MM-DD.md near current date
```

If writing a surface, read one similar recent file from that surface.

3. **Collect evidence compactly**

Prefer:

- `git status --short`
- relevant `README.md`
- explicit artifact files
- test/check outputs
- Coms files if companion collaboration is involved
- existing notebook indexes

Do not replay giant transcripts unless needed. Use targeted reads.

4. **Choose surfaces**

Default:

- daily journal only

Add Creative Loop when there is durable creative/product/research signal.

Add Twin Notebook when the Twin learned a durable principle and Chief's request authorizes notebook mutation.

Add Personal Journal only when explicitly appropriate.

5. **Write smallest durable update**

A good journal update is retrievable, source-aware, and bounded. It is not a full transcript.

## Required post-write verification

After writing, verify:

```bash
# files exist and are non-empty
wc -c <paths>

# indexes can find new loop slugs
grep -R "<slug>" <index files and related ledgers>
```

Report:

- files created/modified
- verification result
- any open edges
- next concrete action

## Writing rules

- Facts before story.
- User-reported external audit stays user-reported unless verified.
- Do not relitigate work Chief explicitly marks as already robustly audited unless a contradiction appears in files.
- Do not overwrite existing journal files blindly; append or create new dated sections.
- Do not mutate Twin Notebook durable principles unless the task clearly authorizes it.
- Patch indexes whenever a new loop file is created.
- Preserve speculation boundaries.
- Use the smallest loop that preserves judgment.

## Output shapes

### Short report to Chief

```txt
Updated:
- <path>
- <path>

Verified:
- <check>

Open:
- <remaining issue, if any>

Next:
- <one concrete move>
```

### Daily journal minimum shape

```md
# 📔 Chief 'Lesz's Daily Journal — YYYY-MM-DD

## Continuity Catch-Up

## What Was Updated

## Verified State

## Durable Learnings

## Open Edges

## Handoff
```

### Creative loop minimum shape

```md
# Creative Loop — <Title>

## Metadata
## Intention
## Artifact / Probe
## Critique
## Delta
## Extracted Taste Rules
## Memory Candidate
## Tradeoff / Risk
## Next Loop
```

### Twin loop minimum shape

```md
# Twin Loop — <Title>

## Metadata
## What this loop was actually about
## What I absorbed from Chief
## The failure worth keeping
## The correction, and the thing I learned
## Twin taste principles produced
## Boundary note
## Next loop candidate
```

## Cut

Do not create a separate `/update-companion-journal` skill unless future usage proves that companion-collab journaling has a different user-visible operation, distinct admission gate, and incompatible memory surfaces.

For now, companion/other-agent journaling is a lane inside `/update-journal`.

## Acceptance test

The skill succeeds when, from any project directory, Chief can say `/update-journal`, and the Twin:

1. identifies the active work arc,
2. selects the right journal surfaces,
3. writes only evidence-bounded durable memory,
4. patches indexes for retrieval,
5. labels other-agent claims correctly,
6. verifies file existence/index discoverability,
7. leaves one clear next move.
