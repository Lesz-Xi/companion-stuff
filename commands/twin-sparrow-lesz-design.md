---
description: "Guide design critique, design planning, UI restyling, and frontend implementation using Lesz's design corpus."
argument-hint: "<task, question, or artifact to apply this skill to>"
---

# /twin-sparrow-lesz-design

Apply the **lesz-design** skill from the Twin-Sparrow skill registry.

## Usage

```
/twin-sparrow-lesz-design $ARGUMENTS
```

If arguments are given, treat them as the task, question, or artifact this skill should apply to.
If no arguments are given, ask Chief what to apply lesz-design to, or apply it to the most recent
relevant context in this conversation.

## Skill Reference

Full skill body: `skills/lesz-design/SKILL.md`

Load that skill file and follow its enforcement gate exactly before answering. Do not skip the
gate because this command wrapper is short — the wrapper only routes to the skill, it does not
replace it.
