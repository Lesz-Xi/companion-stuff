---
description: "Turn an exported site-analysis bundle into 3–4 grounded redesign directions and stop for a human choice. Reads the export folder's tokens, package, and trust report; states what was observed versus..."
argument-hint: "<task, question, or artifact to apply this skill to>"
---

# /twin-sparrow-redesign-direction

Apply the **redesign-direction** skill from the Twin-Sparrow skill registry.

## Usage

```
/twin-sparrow-redesign-direction $ARGUMENTS
```

If arguments are given, treat them as the task, question, or artifact this skill should apply to.
If no arguments are given, ask Chief what to apply redesign-direction to, or apply it to the most recent
relevant context in this conversation.

## Skill Reference

Full skill body: `skills/redesign-direction/SKILL.md`

Load that skill file and follow its enforcement gate exactly before answering. Do not skip the
gate because this command wrapper is short — the wrapper only routes to the skill, it does not
replace it.
