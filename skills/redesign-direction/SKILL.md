---
name: redesign-direction
description: >
  Turn an exported site-analysis bundle into 3–4 grounded redesign directions and stop for a human choice. Reads the export folder's tokens, package, and trust report; states what was observed versus inferred; proposes directions on a deliberate axis derived from a named inspiration corpus; never auto-picks the theme language.
---

# /redesign-direction — Grounded Redesign Direction Brief

## Purpose

A site has been analyzed and exported. Someone now wants it redesigned. The failure this skill exists to
prevent is **the agent choosing the new visual language on the human's behalf** — silently, from taste,
usually toward whatever is currently fashionable.

This skill makes that choice explicit, grounded, and unskippable. It reads the export bundle, states what
is actually known about the site, proposes a small number of directions each traceable to a named source,
and then **stops and asks**.

**The one hard rule:** never propose or begin a redesign without first presenting directions and
obtaining an explicit choice. There is no "obvious" direction. If only one direction seems viable, present
it *as one option alongside the others and say why the others lose* — do not present it as the answer.

---

## Grounding — the principles this skill enforces

Every rule below traces to a brand-identity principle, and the mapping is stated so a rule can be argued
with rather than obeyed blindly.

**The method principle governs the rest:** *look for the elements relevant to your project, not the whole
design — borrow ideas without ripping them off.* A reference supplies a **mechanism**; it never supplies
an appearance. This is why Stage 2 requires each borrowed choice to name its mechanism and its source.

| principle | how this skill enforces it |
|---|---|
| Identity is more than a logo — a complete **visual and verbal** system | six slots cover palette, composition, type, mark, imagery, **and voice**. A direction missing voice is malformed. |
| **Consistency** across touchpoints builds familiarity, then trust | one accent, one type set, one spacing base per direction; a direction that needs exceptions to hold isn't a direction |
| **Colour** is emotional, and poor choices undermine legibility and accessibility | exactly one accent; contrast floor measured against the true backdrop |
| **Imagery** sets the emotional tone before a word is read | imagery is a required slot, and `none` must be a stated choice rather than an omission |
| Identity must be **adaptable** — clear rules with room to evolve | directions state values, not fixed compositions; Stage 4 grows the set from use |
| **Tone of voice** is central, and must align with the visuals | the voice slot requires an **alignment argument**: why this voice follows from this surface |
| **Grids and spacing** provide structure and make work feel intentional | spacing base declared per direction; values off the base are violations |
| **Icons and micrographics** — generic ones erode clarity | icons must be authored to the direction, never generic. See the invariants. |
| Identity **evolves without losing recognition** | every direction must name **what survives** |
| Design is **distillation** — express who they are, not everything they do | a direction states one thesis; four hedged directions are one bad direction |
| Effective identities are **simple, not simplistic** | three to four options, never more; restraint is a rule, not a mood |
| Guidelines must **explain the thinking**, not list rules | every rule here carries its reason; every direction carries its tradeoff |
| Identity must resonate with its **audience** — empathy, not self-expression | **audience is a required input.** See Stage 1. |
| **Heritage** — modernise without losing essence | when a constraint forces a change to a brand value, take the *minimum* change that satisfies it |
| **Distinctive, not decorative** | a direction indistinguishable from a generic version of its category has failed |
| Rooted in **clarity** — every choice explainable | every value traces to a source or is marked as reasoned |
| Only as strong as its **implementation** | values are stated in implementable form — numbers, not adjectives |

**On the heritage rule, a worked precedent:** an accent that failed a contrast floor was first "fixed" by
darkening it to comfortably exceed the threshold. That passed the check and destroyed the colour's
character. The correct fix was the *minimum* darkening that cleared the floor — 87% of the original.
**Compliance is a floor to clear, not a score to maximise.** Passing a check while losing the thing the
check protects is a failure with a green tick on it.

---

## When to Use

- An export/analysis bundle exists and a redesign is being requested
- Someone asks "what should this look like instead?"
- A redesign is about to begin and no theme language has been chosen this session

## When NOT to Use

- Pure implementation of an already-chosen direction — the choice was already made; don't re-litigate it
- Copy edits, bug fixes, or accessibility repairs that don't change the visual language
- No export bundle exists yet — run the analysis first; this skill needs measured input, not a URL

---

## Input

**Argument:** a path to an export folder.

Read in this order. Everything is optional except the first — degrade, never fail:

| file | what to take from it | if missing |
|---|---|---|
| `design-tokens.json` | `colors · typography · spacing · borders · radius · effects` | **stop** — ask for a valid bundle path |
| `aurelian-design-package.json` | `appearance · components · interactions · regions · provenance · evidence` | proceed; note reduced confidence |
| `trust-report.json` | `sections · roles · interactions · summary` | proceed; do not claim coverage figures |
| `DESIGN.md` | the prior human-readable reading of the site | proceed |
| `sections/*.png` | section count and visual character | proceed; say layout read is token-only |

**Do not read the live site.** The bundle is the evidence. If the bundle and your memory of the site
disagree, the bundle wins.

**Do not require any network or design-tool authentication.** This skill runs on local files only.

---

## Stage 1 — State what was observed, before proposing anything

Report the site's current profile **with provenance carried through**. If the bundle labels values
`observed · inferred · manual · canonical`, preserve those labels; do not launder an inferred value into a
stated fact.

Cover, in this order:

1. **Palette** — actual values, and how many distinct accents are in use
2. **Type** — families, how many weights, whether figures are tabular
3. **Spacing** — the base step if one is detectable, and any values off it
4. **Composition** — section count and arrangement (centered · split · stacked · gridded · radial)
5. **Interaction** — what states exist
6. **What is not knowable from this bundle** — say it explicitly

Then state, in one sentence, **the strongest surviving asset**: the single thing about this site worth
keeping. This drives direction 4 and must come from the data, not from taste.

### Audience — a required input, not an optional one

Identity work is built around empathy: knowing who it is for and what will feel relevant and trustworthy
to them. A redesign chosen without an audience is self-expression wearing a system's clothes.

So before the directions:

- If the audience is known, **state it**, and let it eliminate directions. It usually eliminates at least
  one, and saying which is more useful than offering four survivors.
- If it is **not** known, say so plainly and **ask** — one sentence is enough: *"who is this for?"*
- If the human declines to answer, proceed, but **label every direction as audience-blind** in the output.
  That label is not a formality: it is the difference between a taste proposal and a design proposal, and
  it must survive into whatever gets built.

An unstated audience is the most consequential blank a direction set can carry, because it is the only
input that could have settled the choice on evidence rather than preference.

> Anti-pattern: skipping to the directions. A choice between four options is not informed unless the
> chooser knows what they're trading away.

---

## Stage 2 — Propose directions on a deliberate axis

**Three to four. Never more.** More options is not more service; it moves the decision cost back onto the
human, which is what this skill exists to reduce.

Generate along this axis — not four moods:

| # | direction | what it does |
|---|---|---|
| 1 | **Discipline it** | Keep the site's own register. Apply the invariants below. Lowest risk, highest fidelity to original intent. |
| 2 | **Cross the pole** | Move it to the opposite register — systematic → authored, or authored → systematic. Highest transformation. |
| 3 | **Synthesise** | The site's existing structure with the opposite register's atmosphere. |
| 4 | **Follow the strongest surviving asset** | **Computed from Stage 1**, not chosen from a list. Strong photography → material register. A real type system → systematic register. This is the direction that keeps the output from being a template. |

Each direction must state:

- **Which register** it comes from, by name
- **The concrete deltas** from the site's current tokens — actual values, not adjectives
- **What survives** — naming this is what makes a direction a redesign rather than a replacement
- **The tradeoff** — what it costs. A direction with no stated cost has not been thought through.
- **Source** — for every borrowed choice, name the *mechanism* and the *reference folder* it came from,
  never the appearance. "Palette derived from a photograph, per `color-material-palette`" is legitimate;
  "like that one Pinterest board" is not.

---

## Stage 3 — Stop and ask

Present the directions and **stop.** The question, always including the escape:

```
Which direction for <site>?

  1. Discipline it        — <one line>
  2. Cross the pole       — <one line>
  3. Synthesise           — <one line>
  4. <asset-led name>     — <one line>
  5. Something else       — tell me what you want instead

I won't pick for you. Say a number, or describe the language you want.
```

**Never auto-pick.** Never rank them as "recommended" unless asked — a recommendation collapses a
four-door gate into one door with decoration. If asked directly which you'd choose, answer, but only
after the options have been presented.

---

## Stage 4 — Capture "something else"

If the human describes a direction not offered, **write it back as a new named direction** with the same
six slots filled. The direction set should grow from use. A gate that only ever offers its seed options
trains the human to pick the nearest one, and their actual taste never enters the system.

---

## The six slots

A direction is one selection across these six. Each slot has a bounded vocabulary — extend it only from
observed reference material, never from invention.

| slot | vocabulary |
|---|---|
| **palette** | derived-from-photograph · neutral base + exactly one accent · monochrome-from-single-hue |
| **composition** | centered · split · stacked · gridded · radial |
| **type posture** | warm editorial serif ⇄ cool geometric spec-sheet |
| **mark treatment** | systematic permutation ⇄ hand-drawn gesture |
| **imagery** | in-situ material · editorial mood · technical/orthographic · none |
| **voice** | four sub-slots: language · rhythm · formality · one prohibition — **plus the alignment argument** |

**The voice slot is not complete without its alignment argument.** State *why this voice follows from this
surface*. A restrained surface with overselling copy reads as a contradiction, and the reader trusts the
surface over the sentence. Naming four attributes is a word list; naming why they follow from the visuals
is the thing the principle actually asks for.

**Motion is deliberately not a slot.** See "Scope limit" below.

**Icons are deliberately not a slot either, for the same reason** — no icon corpus exists to derive a
direction from, and a generic or mismatched icon set erodes clarity rather than adding personality. Icons
are therefore governed as an invariant (below): authored to the chosen direction, or absent. Never
imported from a generic set to fill space.

---

## Invariants — applied to every direction, not chosen between

These are not stylistic preferences; each is load-bearing. Any direction violating one is malformed.

1. **Exactly one accent.** A second accent forces the reader to learn what each means. One needs no
   legend — its presence is the meaning. Tonal ramps of a single hue are permitted (e.g. a darker step for
   small text); a second hue is not.
2. **Planes separate by hairline and tone** — never box, border, or elevation. A box asserts a boundary
   the content may not have; a shadow implies a light source the page doesn't otherwise have.
3. **Space is active.** Rank by the interval around an element, not by heavier weight. Never fill a gap
   because it exists.
4. **Values are stated.** Any spacing, size, timing or colour that matters is written down. An unstated
   value gets re-guessed by the next person and drifts.
5. **Text contrast ≥ 4.5:1** under 18px, ≥ 3:1 at 18px and above, measured against the **actual backdrop**
   — the nearest filled ancestor, not the page background. Measuring against the page background is the
   usual cause of a missed failure, including text rendered in the accent *on* the accent.
6. **Hover is quiet attention.** Primary: accent fill rises from below, `translateY(101% → 0)`, no glow.
   Ghost: underline reveal, no competing border. Nav: opacity + hairline underline. Logo:
   `translateY(-3px)` + opacity. Duration `160ms`, easing `power3.out`. **Hover never introduces a second
   primary action.**
7. **It must survive greyscale with motion off.** If hierarchy collapses without colour and movement,
   they were carrying structural load they shouldn't. This is a structural test wearing an accessibility
   costume.
8. **Every choice explainable.** Why this typeface, why this colour, why this layout. If a choice can't
   answer, it's style over substance.
9. **Icons are authored to the direction, or absent.** Generic or mismatched icons erode brand clarity
   faster than having none. An icon set must share the direction's construction logic — same stroke
   weight, same corner treatment, same geometric or gestural origin. Reaching for a generic library to
   fill an empty slot is a violation, not a shortcut.

**Provenance of these invariants,** since a rule's origin affects how hard it should be to override:
1, 3, 4, 5, 8 and 9 derive from the brand-identity principles above. **2 (hairlines over boxes) and 7
(greyscale test) are house doctrine, not from those principles** — they are defensible and load-bearing,
but they are a stronger claim than the rest and should be argued rather than asserted if a direction has
real reason to break them. 6 (hover values) is inherited from shipped implementation code, so treat those
numbers as measurements, not preferences.

---

## Seed registers

Three complete, measured selections. **Prefer `references/directions.json` in this skill folder when it
exists** — it carries the same three registers as typed, machine-diffable data (plus a `knownIssue` field
for any register with a live, unresolved discrepancy — e.g. a board's own hero copy claiming a wrong
section count — carried forward as data rather than silently fixed or silently omitted here). Read it and
use its values over the embedded ones below.

Also prefer a project-local direction index or guidelines file when one exists outside this skill (e.g. a
project's own `*-GUIDELINES.md`) — that is the reasoning authority; this skill's `directions.json` is a
transcription of it, not a replacement.

The embedded values immediately below are the last-resort fallback so this skill still works with zero
project context — no `references/directions.json`, no project guidelines file, nothing but this one file.

### `quiet-instrument` — authored / material

```
ground  #faf9f5   ink #121211   muted #595956   hairline #e3e1d5
accent  #9e7e50 (fills, rules, areas) · #896e46 (text ≤18px, contrast-safe)
type    display: transitional serif · body: neutral grotesque · mono: humanist
spacing base 8 · side margin 80 · section rhythm 120
mark    chosen slowly; rejected attempts kept visible
voice   says less than it knows; first person plural; never explains its own quality
```

### `specimen` — engineered / systematic

```
ground  #f1f2f5   surface #ffffff   ink #131416   muted #646870   hairline #d4d7e1
accent  #1b52e8 — state and emphasis only, never a background
type    one geometric grotesque, four weights (400/600/700/800), tabular figures
spacing base 4 · primary steps 8/16/24/32/64/96
mark    systematic permutation, shown as a grid, chosen mark marked
voice   no adjective that cannot be measured; short; impersonal
```

### `dark-archive` — synthesis of the two

```
ground  #0b0c10   ink #f5f6f9   muted #8f929d   hairline #212330
accent  #d4af37 — marks state, never fills a surface
type    display: high-contrast serif · body: geometric sans · mono: technical
spacing 8px baseline matrix
mark    measured — spec table plus a legibility floor
voice   records rather than persuades; impersonal; dated and numbered
```

**Note on the third:** it is a *synthesis*, not an independent third pole. Two poles and a hybrid. Do not
present it as a peer of the other two when explaining the axis.

---

## Degradation

The gate must render even when generation fails. Nothing load-bearing may depend on synthesis succeeding.

| condition | behaviour |
|---|---|
| synthesis works | 4 directions, including the asset-led one |
| synthesis fails or is unavailable | the three seed registers + "something else" — **still a valid gate** |
| bundle partially readable | proceed on what's present; state what's missing |
| `design-tokens.json` absent | stop; ask for a valid path. Do not infer a profile from screenshots alone. |

A hard stop that cannot render is worse than no hard stop: it fails closed on work already in progress.

---

## Scope limit — motion is out

Motion, animation, and scroll-trigger behaviour are **not** direction axes in this version.

The reason is an asymmetry, not an oversight: an export bundle typically *observes* the analyzed site's
motion, but a still-image inspiration corpus contains no motion vocabulary to redirect it toward. A motion
direction generated against no reference material would be invented, which violates the sourcing rule in
Stage 2.

The hover values in the invariants remain in force — they are a **floor applied to every direction**, not
an axis chosen between. When a motion corpus exists (captured recordings or annotated references held to
the same caption discipline as the image folders), motion becomes a seventh slot. Until then it is absent
rather than empty.

---

## Anti-Patterns

- Proposing a redesign without presenting directions first
- Presenting one direction as the answer, or ranking unasked
- Directions that differ in mood but not in any stated value
- Borrowing an appearance instead of a mechanism — "like <site>" is not a direction
- Laundering an `inferred` token into a stated fact in the observed profile
- Reading the live site instead of the bundle
- Producing more than four options
- A direction with no stated tradeoff
- Blocking entirely because the synthesiser failed

---

## Acceptance checks

A compliant run satisfies all of these:

1. The observed profile precedes the directions and preserves provenance labels
2. Between 3 and 4 directions, each naming register, deltas, what survives, tradeoff, and source
3. Direction 4 is derived from Stage 1's strongest-surviving-asset, not from a fixed list
4. The output ends in a question with an explicit "something else" option
5. No direction violates an invariant
6. Two materially different bundles produce materially different direction sets — if a template site and
   a bespoke one yield the same four, the generator is reading the corpus and ignoring the site
7. With synthesis disabled, the gate still renders the three seed registers
8. **Audience** is stated, asked for, or every direction is explicitly labelled audience-blind
9. **Distillation:** each direction expresses **one** thesis statable in a sentence. Four directions that
   each hedge across two registers are one bad direction presented four times.
10. **Distinctive, not decorative:** each direction is distinguishable from a generic version of the
    site's category. If swapping the accent hex would make it indistinguishable from a competitor, it is
    decoration and fails.
11. Every voice slot carries its **alignment argument**, not just its four attributes

---

## Portability

This skill is self-contained by design: `SKILL.md` plus `references/directions.json` travel together as
one folder, and both are read as local files only. It requires no plugin, adapter, command wrapper,
network access, or design-tool authentication, and it does not depend on any sibling skill.
`references/directions.json` is optional data, not a dependency — delete it and the embedded seed
registers below still make the skill fully functional.

It will prefer `references/directions.json`, then a project-local direction index or guidelines file
outside this skill, and fall back to the embedded seed registers only when neither is present. If the
embedded values below are edited in a project that also maintains a live index or `directions.json`, the
external file is the authority and these are a snapshot — say so rather than letting the two drift
silently.
