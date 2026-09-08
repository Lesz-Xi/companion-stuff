---
name: design-engineer
description: >
  Composite design-engineering skill pairing a minimal, thin/micro, material UI/UX layout doctrine with expert-engineer implementation discipline — for layout architecture, component design, design-system frontend work, accessibility, performance, and production implementation.
---

# Design Engineer

This is a composite skill. Apply the built-in **Layout Doctrine** (below) together with `expert-engineer`.

The doctrine in one line: **layout is the interface.** Grid, hierarchy, spacing, and surface decide what the user understands; everything else is decoration. The direction is minimal, thin/micro, material, cutting-edge, and modern.

## Activation Boundary

Use this composite only when the task actually requires layout architecture, component design, or design-system-level frontend work.

Do **not** invoke this composite for minor polish that merely wires existing UI to existing tokens, CSS variables, labels, copy, foreground/background values, or other already-established visual rules. In those cases, skip the doctrine and execute directly as a small engineering change.

Examples that stay outside this skill:

- "make workspace/operator/engine follow Main View Foreground"
- "small token plumbing polish"
- "replace accent color with existing foreground token"
- "minor label color fix"

## 🔒 MANDATORY ENFORCEMENT GATE

**You MUST follow this protocol before addressing the user's request. Do not skip any step. Do not collapse steps. Do not proceed to the task until all phases below are completed and written in your output.**

### Step 1: Acknowledge (write this exact line in your output)
```
[design-engineer] Protocol engaged. Source skills required: expert-engineer.
```

### Step 2: Load Source Skill
Read the full `expert-engineer/SKILL.md` before continuing — apply its Full-Stack and TypeScript roles to ensure production-quality implementation. The Layout Doctrine is built into this skill; apply it directly from the section below.

### Step 3: Execute Workflow
Apply the Combined Workflow (below) in the exact order listed. Write each layer's output before proceeding to the next.

### Step 4: Only After All Complete
After writing the full output from all workflow layers and the final formatted design review, you may then address the specific user request.

---

## Layout Doctrine

Five commitments. Every layout decision is checked against them; when they conflict, the order below is the priority order.

### 1. Minimal — remove before adding

- Every element earns its place by what the user understands or does because of it. Anything else goes.
- One idea per view; one dominant focal element per view.
- Prefer fewer, larger regions over many small boxes. Nesting depth is a cost.
- When a section feels empty, first ask whether it should exist — not what to add to it.

### 2. Thin / micro — precision at small scale

- Hairline rules: 1px (or 0.5px on high-DPI) borders and dividers instead of heavy containers.
- Small, disciplined type scale with tight tracking; micro-labels and eyebrow text carry metadata, not headings.
- Generous whitespace is the separator — not boxes, not backgrounds, not borders.
- Compact control sizes; no heavy cards, no chunky shadows, no fat pills.
- Detail quality is the differentiator: optical alignment over mathematical, consistent radii, exact spacing.

### 3. Material — surface over outline

- Surfaces are defined by subtle elevation and tonal separation, not border-heavy scaffolding.
- Layering uses translucency and blur where the platform supports it; backgrounds stay quiet.
- Light and dark themes are both first-class, driven by tokens — never hard-coded values.
- Elevation is semantic: it signals interactivity and layering, never decoration.

### 4. Cutting edge / modern — use the platform

- Fluid type and spacing via `clamp()`; layout responds to its container (container queries) before its viewport.
- Design tokens as CSS custom properties; theming is a token swap, not a restyle.
- Modern selectors and patterns (`:has()`, scroll-driven animations, view transitions) where they simplify the code — with graceful degradation.
- Respect `prefers-reduced-motion` and `prefers-color-scheme` as constraints, not afterthoughts.
- Interaction feedback is crisp and system-native in feel: fast, short-eased, reversible.

### 5. Layout grammar — the discipline underneath

- Strict grid: a small number of columns, consistent gutters, no element floating off-grid without a reason.
- Spacing scale on a 4/8pt base; exceptions must be named, not improvised.
- Baseline rhythm for text-dense regions.
- Hierarchy through scale, weight, and position — in that order — before color.
- Alignment is optical: icons, numerals, and mixed-case text are adjusted by eye, not just by math.

---

## Combined Workflow

Apply layers in this order:

1. **Layout Direction** (Layout Doctrine) — Grid, hierarchy, spacing rhythm, focal element, surface strategy for the task
2. **Component Architecture** (expert-engineer Full-Stack) — State ownership, data-fetching boundaries, layer separation
3. **Styling System** (Layout Doctrine) — Tokens: type scale, spacing scale, hairline rules, elevation levels, color semantics, motion/transition patterns
4. **Type Safety** (expert-engineer TypeScript) — Props interfaces, discriminated unions for component states, eliminate implicit types
5. **Accessibility** (doctrine + expert-engineer) — Semantic HTML, keyboard navigation, focus management, ARIA where needed
6. **Performance** (expert-engineer Full-Stack) — Render optimization, data fetching strategy, bundle impact
7. **Error States** (doctrine + expert-engineer) — Loading skeletons, error boundaries, empty states, retry flows — all designed, not just coded

## Output Format

```
## Layout Direction
- Grid & hierarchy: [columns, regions, focal element, spacing rhythm]
- Surface strategy: [elevation, tonal separation, theme tokens]
- Doctrine rationale: [which doctrine commitments drive the choices]
- Visual changes: [what changes in layout, typography, color, spacing, interaction]

## Component Architecture
- State model: [what state lives where]
- Data flow: [how data moves through components]
- Interfaces: [key TypeScript types]

## Implementation Steps
1.
2.
3.

## Tradeoffs
| Decision | Option A | Option B | Rationale |
```

## When to Use

- Designing or building new screens, views, and UI components
- Restructuring layouts: grid systems, hierarchy, spacing, and surface strategy
- Design-system and component-library development in the minimal/material idiom
- Design-to-code handoff where layout fidelity matters
- Frontend architecture that must be both visually precise and maintainable
- **Synthesis / blend work:** implementation lane after the synthesis contract exists. Do not start layout/engineering while direction, brief, provenance, and cut list are missing.
