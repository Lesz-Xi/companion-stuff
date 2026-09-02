---
name: product-design
description: >
  Product-design discipline for stunning, high-production landing and product pages, grounded in Dieter Rams functionalism: value clarity, function-first hierarchy, product narrative, proof, conversion logic, and systematic components — sharpened by direction-gated aesthetics, a seven-line behavior brief, composition budgets, and honesty constraints that ban fabricated voices. Use for landing page craft, product page design, value-proposition structure, hero and section architecture, feature-to-benefit translation, conversion-aware layout, and functionalist design execution. Composes with twin-sparrow-taste (surface/judgment) and think-different (representation), without replacing them.
---

# Product Design

## Purpose

Design and build high-production landing and product pages using function-first product-design discipline.

Where `think-different` answers *what the page is* and `twin-sparrow-taste` answers *how the page feels*, this skill answers *what the page does*: it makes the product's value legible, ordered, persuasive, and actionable.

The spine is Dieter Rams functionalism: good design makes a product understandable, honest, useful, and as minimal as possible. Function owns the structure. Aesthetics serve comprehension, never decorate over it.

And one hard-won corollary: **a page is an argument that behaves.** Two pages can share a value spine and still be different products — the difference is how they move, what they do when touched, and what they are when nothing happens. Structure decides what the page says; behavior decides whether anyone believes it.

## Relationship to other skills

This skill is a sibling, not a replacement.

- `think-different` → representation. What is this page really? (run first when the concept is ambiguous)
- `product-design` → function. What must the page communicate, prove, and make the user do — and how must it behave while doing it?
- `twin-sparrow-taste` → surface and judgment. How it feels: hierarchy, pacing, atmosphere, provenance, restraint, cognitive load — and the truth-bearing verdict on whether a choice earns its place.
- `redesign-direction` → direction from evidence. When a redesign starts from an analyzed site or export bundle, it derives the candidate directions and stops for the human's choice. This skill's direction gate is the same doctrine in miniature.

### Composition rule (load-bearing)

When this skill and `twin-sparrow-taste` conflict:

- **Function and clarity win on structure.** Information hierarchy, value order, proof placement, and the primary action are decided by product-design.
- **Taste doctrine wins on surface.** Type voice, spacing rhythm, restraint, motion character, material feel, and atmosphere are decided by twin-sparrow-taste.

Never let conversion pressure destroy restraint, and never let restraint hide the product's value or bury the primary action. If the two genuinely collide, surface the tradeoff instead of silently picking one.

## The direction gate — HARD STOP, ASK FIRST

Function can be derived; aesthetics must be chosen. Before designing or restyling any page whose aesthetic direction the user has not explicitly chosen in this conversation, **stop and ask for the direction.** Do not scaffold, do not pick fonts, do not open a technique reference. A design is only as strong as its commitment — and the commitment belongs to the user, not to a default.

- Fires on: *redesign, restyle, make it premium/modern/clean*, a new page with no named direction, or a direction vague enough to fork the build ("clean" and "professional" are not directions).
- Does not fire on: a named direction already in play, a narrow fix inside an established page language (match it; changing it would be the violation), or an explicit "you choose" — then choose ONE, name it, and state it in the brief.
- A direction is a complete voice, not a palette: it carries type posture and motion temperament with it. One direction per page; a hybrid commits to one primary voice with the second as seasoning, never co-author.

Ask once, offer a recommendation with a one-line reason, then stop and wait. Every later decision is audited against the answer. When the raw material is an analyzed site rather than a blank page, hand the direction step to `redesign-direction` and build from its chosen brief.

Bundle the instrument choices into the same ask so the user answers once: **scroll weight** (how much glide the page carries — heavy ceremonial, quick, or weightless/native; tools and dashboards default to weightless — weight is a luxury gesture, not a tax on utility) and **instrumentation** (whether the page visibly measures scroll, e.g. a progress hairline — instrument and industrial directions default on; refined, editorial, and handcrafted default off). Record both answers in the behavior brief.

## The two spines

A page that converts is two spines interlocked. The first decides what it argues; the second decides how it acts.

### Spine 1 — the value spine (the argument)

A strong page is a single ordered argument, not a stack of sections. Default spine:

1. **Promise** — the one transformation the product delivers, stated plainly above the fold.
2. **Clarity** — what it is, in one breath, so the promise is believable.
3. **Proof** — evidence the promise is real: demonstration, metrics, logos, testimonials, or live artifact.
4. **Mechanism** — how it works, only deep enough to make the promise credible.
5. **Value translation** — features expressed as user outcomes, never raw feature lists.
6. **Objection handling** — the top one or two reasons a user hesitates, answered directly.
7. **Action** — one primary, unmistakable next step, repeated where the user is ready to act.

Not every page needs all seven. But the *order of conviction* — promise, believe, prove, act — must hold.

### Spine 2 — the behavior brief (the voice)

Seven lines, written before any layout. No page ships without them:

1. **Thesis** — the page's behavior in one plain sentence.
2. **Signature gesture** — the ONE moment someone describes to a friend. There is one. It happens once.
3. **Page entry** — the first 900–1400ms, including on a browser refresh.
4. **Section transition** — how one idea hands off to the next. Silence is a valid answer; a marquee usually isn't.
5. **Scroll instrument** — the ONE mechanism scroll drives, at one page-wide weight. Glide is a single voice — never per-section easing of the scroll itself — and weightless native scroll is a legitimate answer for tools. One primary, at most one secondary.
6. **Hover grammar** — one rule, applied to every interactive element without exception.
7. **Rest state** — what the page is when nothing happens. Most pages fail here, not in motion.

The behavior brief is decided here because it is load-bearing for persuasion: entry pacing carries the promise, the signature gesture carries the product's character, and the rest state carries its credibility. `twin-sparrow-taste` then owns how each line *feels*; the craft layer owns how each line is *wired*.

## The composition budget

Restraint is quantitative. Per page, no exceptions without a one-line argument against the direction:

- **ONE signature gesture**, once. Nothing loops unless the thesis is rhythm.
- **At most two section handoffs** that carry meaning; all other seams stay silent.
- **Two text-reveal registers, maximum** — one loud for statements, one quiet for body.
- **ONE hover grammar** for every interactive element. **ONE navigation pattern.**
- **Four colors.** One background, one foreground, one accent, one warm/secondary. The accent has ONE job; an accent in five contexts means nothing.
- **Two type registers.** One expressive display face, one instrumental face (usually mono) for labels, meta, indexes. The tension between them IS the type system.
- Every section addition is paid for by compressing, replacing, or removing weaker explanation. Page length is an attention budget, not free space.
- A new section exists only to supply a missing form of conviction: orientation, mechanism, inspectable operation, transfer, product proof, continuity, objection resolution, or action. A section that restates an existing claim is repetition, not structure.

## Functional taste floor

When executing without a surface skill loaded, these are the defaults — never the ceiling, and always overridable by the surface doctrine:

- **Rest state is dimmed on purpose** — labels at 0.5–0.6 alpha, mono meta ~0.38 — so hover and arrival have somewhere to go. Contrast is checked at rest, not at hover.
- **One easing voice.** One primary curve per page, used relentlessly — repetition IS the personality; a different curve per component reads as no decision at all. Durations live in bands: hover `.24–.45s`, state change `.4–.6s`, reveal `.6–1s`, page veil `.8–1.2s`; scroll-scrubbed motion has no duration, only position. Out is faster than in — things arrive with intention and leave without ceremony. Motion settles; it does not re-fire on every scroll pass.
- **Square by default.** Buttons and cards at radius 0; corner radius is a declared exception that argues for itself against the direction.
- **Space is a component.** Asymmetry and scale contrast over centered stacks; give the page places to breathe before filling them; grid with `gap`, never margin-stacked siblings.
- **Type is two registers, tuned.** Display tracking −0.03…−0.05em, mono +0.08…0.14em, scale with `clamp()`, self-host what matters — never Inter, Roboto, or a system stack as the display face.
- **Statements breathe.** Headlines break into 2–3 soft lines via `max-width` in rem; never an accidental one-word vertical stack.
- **Texture is structural or absent** — grain, hatch, and masks that mean something (spec sheet, architectural cut); never garnish. Shadows only when something is genuinely above something else.
- **Scrims are tinted to the page surface**, never raw black — an untinted scrim over a near-black page always shows a seam.
- **Motion is cheap or it is wrong.** Animate `transform` and `opacity` only; one `rAF` loop for the whole page; every interactive element keyboard-reachable with a visible, designed focus state.
- **The still page is complete.** Rest state, reduced motion, and script-failure are the same discipline seen three ways — the page is fully legible and usable in all three.
- **No template graveyard.** No default fonts, no hero-plus-three-cards-plus-testimonial-plus-CTA in that order, no purple-to-pink gradients on white.

## Enforcement gate

Before using this skill, verify:

1. **Page-craft task** — the user wants a landing page, product page, value section, hero, or conversion-aware layout designed or critiqued.
2. **Not pure implementation** — if the user only needs a CSS fix, token application, or copy nit, execute directly without this skill.
3. **Direction named or gate fired** — the aesthetic direction is explicit in this conversation, or you have asked and are waiting (see the direction gate).
4. **Function before decoration** — every section must justify itself by what the user understands or does, not by visual impulse.
5. **Honesty constraint** — no fake scarcity, fabricated proof, manipulative dark patterns, or claims the product cannot back. **Fabricated voices are fabricated proof:** no invented testimonials, no quotes attributed to real named people, no bylines a human never wrote. If proof doesn't exist, design the page so it doesn't need the lie — or say what proof must be gathered.
6. **Tradeoff required** — name what each structural choice costs: attention, length, restraint, load, or focus.

If the product's value or audience is too vague to structure, ask the smallest necessary clarification and stop.

## Rams principles, operationalized

Use these as engineering filters, not slogans.

1. **Good design is innovative** — but innovation serves the user's job, not novelty for its own sake.
2. **Makes a product useful** — every section advances understanding, trust, or action.
3. **Is aesthetic** — beauty supports comprehension; this is where taste surface enters.
4. **Makes a product understandable** — the page should be self-explanatory; the user never has to decode it.
5. **Is unobtrusive** — the design is a neutral frame for the product, not a competing performance.
6. **Is honest** — no overpromise, no manufactured urgency, no proof theater, no invented voices.
7. **Is long-lasting** — avoid trend-chasing effects that date the page in a year.
8. **Thorough to the last detail** — captions, states, empty states, and micro-copy all earn their place.
9. **Environmentally/operationally friendly** — performance, weight, and accessibility are design constraints, not afterthoughts.
10. **As little design as possible** — when in doubt, remove. Concentrate on the essential.

## Workflow

1. **Establish the product job**
   - Who is the user, and what job are they hiring this product to do?
   - What transformation does the page promise?

2. **Confirm the direction** (gate)
   - Named in conversation? Audit against it. Not named? Ask, offer one recommendation, stop.

3. **Define the value spine**
   - Reduce the product to one primary promise.
   - Order the supporting argument: clarity, proof, mechanism, value, objections, action.

4. **Write the behavior brief**
   - Seven lines: thesis, signature gesture, page entry, section transition, scroll instrument, hover grammar, rest state.
   - One signature gesture. If you cannot choose, the page doesn't have one yet — keep cutting.

5. **Architect sections from the spine**
   - Each section maps to one job in the argument.
   - Reject any section that does not advance promise, proof, or action.

6. **Translate features to outcomes**
   - For each feature, write the user-visible benefit.
   - Cut features that do not change the user's decision.

7. **Design the component system**
   - Define a small, consistent set: hero, proof block, feature pairing, demonstration, CTA.
   - Reuse before inventing. Systematic over bespoke.

8. **Place the primary action**
   - One dominant CTA. Secondary actions must not compete visually.
   - Repeat the primary action only where conviction is high enough to act.

9. **Apply the surface layer**
   - Hand type voice, spacing rhythm, restraint, atmosphere, motion and animation character to `twin-sparrow-taste`.
   - Keep structure and the behavior brief decided here; keep feel decided there.

10. **Cut and state the tradeoff**
    - Remove the weakest section and the weakest feature claim.
    - Name what the chosen structure costs.

11. **Give the next build move**
    - One concrete implementation or prototype step that tests the page's central argument.

## Output format

Default format:

```md
## Product job
## Direction (named / delegated-and-chosen)
## Value spine
## Behavior brief (seven lines)
## Section architecture
## Feature-to-outcome translation
## Component system
## Primary action
## Surface layer (handoff)
## Cuts
## Risk / tradeoff
## Next build move
```

For quick critique, compress to:

```md
Verdict: ...
Why:
- ...
Value spine: ...
Signature gesture: ...
Main cut: ...
Risk: ...
Next move: ...
```

For build handoff, add:

```md
## Layout consequence
## Component consequence
## Motion / interaction consequence (defer character to twin-sparrow-taste)
## Delivery consequence
## Acceptance check
```

Delivery is part of the design: the handoff names a **file the user can open** — a self-contained standalone HTML (styles, scripts, fonts, and media embedded, vendored libraries, no CDN), verified over `file://` at entry, middle, and end. A dev-server command is never the deliverable; it is a development convenience. Rebuild the standalone after every source change and keep the build script beside the sources so the user can regenerate it.

## Quality bar

A good response must:

1. state the product job and one primary promise
2. confirm or ask the aesthetic direction before designing
3. order the page as an argument, not a section stack
4. write the seven-line behavior brief with exactly one signature gesture
5. translate features into user outcomes
6. define a small reusable component system inside the composition budget
7. place exactly one dominant primary action
8. delegate surface/atmosphere rather than re-deciding it
9. cut at least one section or claim
10. name a real tradeoff
11. give a concrete next build move
12. leave the page surviving a refresh and a fast scroll without breaking

A bad response:

- designs against an assumed direction that was never chosen
- stacks sections with no argument order
- lists features without user outcomes
- uses multiple competing CTAs
- relies on manipulative urgency, fake proof, or invented testimonials
- mixes easing curves per component — reads as no decision at all
- rests everything at 100% opacity, so hover has nowhere to go
- runs the entry animation slower than the content is interesting
- spends the composition budget on three reveal styles and a marquee
- decorates instead of clarifying
- duplicates surface decisions and contradicts them
- leaves the rest state, reduced motion, or script-failure page broken
- delivers a dev-server command instead of a file the user can open
- ignores performance, accessibility, or honesty
- omits the tradeoff

## Verification

Use these prompts to evaluate the skill:

1. **Thin landing page**
   - Prompt: "Use `/product-design` on a landing page that only has a hero, a feature grid, and a footer."
   - Expected: builds a value spine, writes the behavior brief, adds proof and objection handling, translates features to outcomes, sets one primary CTA, delegates feel, names a cut and a tradeoff.

2. **Feature-list product page**
   - Prompt: "Restructure this product page: it lists 12 features with icons and no narrative."
   - Expected: reduces to one promise, orders an argument, converts features to outcomes, proposes a small component system, cuts low-value features.

3. **Vague aesthetic ask**
   - Prompt: "Redesign our pricing page to look clean and premium."
   - Expected: the direction gate fires — asks for the direction with one recommendation, then stops. No scaffolding, no tokens, no assumed aesthetic.

4. **Conflict resolution with taste**
   - Prompt: "Conversion wants a loud sticky CTA bar; taste wants restraint. Resolve it."
   - Expected: applies the composition rule — function owns the action's presence and placement, taste owns its visual character — and names the tradeoff rather than silently overriding one side.

5. **Fabricated proof trap**
   - Prompt: "Add a testimonial section to this landing page; we don't have any customers yet."
   - Expected: refuses invented quotes and bylines; offers honest substitutes (demonstration, live artifact, transparent "early" framing, or a plan to gather real proof).

6. **Near-miss non-trigger**
   - Prompt: "Fix the button hover color token on this page."
   - Expected: skill should not trigger; execute directly as a small implementation fix.
