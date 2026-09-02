---
name: lesz-design
description: >
  Guide design critique, design planning, UI restyling, and frontend implementation using Lesz's design corpus.
---

# Lesz Design

Use this skill to ground design work in the `design-md` reference corpus. Treat it as a design-and-UI guidance skill, not a generic inspiration board.

## Non-Goals / Do Not Invoke

Do **not** invoke this skill for minor implementation polish that only touches existing tokens, CSS variables, labels, copy, spacing nits, or already-established style rules.

Examples that should **not** trigger `lesz-design` by themselves:

- "make this label follow Main View Foreground"
- "minor polish"
- "wire this to the existing token"
- "small color variable fix"
- "use the existing foreground/background/accent token"

For those tasks, execute directly with normal engineering/tool discipline. The design-reference gate exists only when the task needs an external design language or reference corpus.

## Mandatory Gate

Before reading any style-specific reference, ask the user:

`Which design reference should I use for this task?`

Enforce these rules every time:

- Ask first on every invocation, explicit or implicit.
- Ask first even if the user already named a style in the same message.
- Do not infer, auto-pick, or continue from context alone.
- Do not read any style-specific `DESIGN.md`, `README.md`, or `preview*.html` until the user confirms the design reference.
- If the user does not answer, stop at the selection step.

## Selection Workflow

Once the user confirms they want this skill, ask them to choose one supported reference from the source catalog.

The available references are:

- `airbnb`
- `apple`
- `claude`
- `cursor`
- `elevenlabs`
- `expo`
- `ibm`
- `intercom`
- `lovable`
- `mistral.ai`
- `ollama`
- `opencode.ai`
- `posthog`
- `raycast`
- `runwayml`
- `sanity`
- `spacex`
- `vercel`
- `warp`
- `wise`
- `x.ai`

When presenting options, always include `apple`, `cursor`, and `spacex` in the chooser.

If the user gives an unsupported style, ask them to pick one from the supported list before proceeding.

## Reference Loading Order

After the user selects a style, load references in this order:

1. Read that style's `DESIGN.md` first.
2. Read that style's `README.md` only if you need concise context, caveats, or the preview summary.
3. Read `preview.html` or `preview-dark.html` only if you need visual confirmation of tokens, component treatments, or light/dark behavior.

Do not load multiple styles unless the user explicitly asks for a comparison.

Use [references/source-catalog.md](references/source-catalog.md) for the exact absolute paths.

## Use Cases

Use the selected reference to do one or more of the following:

- critique an interface against a chosen design language
- plan a redesign or restyle with concrete visual direction
- guide frontend implementation details such as typography, spacing, color, surface, layout, and interaction tone
- translate a chosen style into prompts, specs, or implementation guidance

## Working Rules

- Stay faithful to the selected design language's actual documented patterns.
- Prefer the chosen style's documented typography, color, spacing, layout, and component rules over generic design advice.
- Distinguish clearly between direct facts from the chosen reference and your own implementation inferences.
- If the task requires comparison, ask which styles to compare before loading more than one.
- If the user changes the style mid-thread, treat that as a new selection and switch references explicitly.

## Output Expectations

When using this skill after selection:

- name the chosen reference
- cite the specific reference file(s) used
- separate direct reference facts from implementation interpretation when that distinction matters
- keep the design guidance actionable for critique, planning, or code work
