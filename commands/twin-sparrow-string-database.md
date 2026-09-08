---
description: "Query the STRING database for protein-protein interactions (PPIs), functional enrichment, and homology. Use when the user asks about interactions between specific proteins, interaction evidence, co..."
argument-hint: "<task, question, or artifact to apply this skill to>"
---

# /twin-sparrow-string-database

Apply the **string-database** skill from the Twin-Sparrow skill registry.

## Usage

```
/twin-sparrow-string-database $ARGUMENTS
```

If arguments are given, treat them as the task, question, or artifact this skill should apply to.
If no arguments are given, ask Chief what to apply string-database to, or apply it to the most recent
relevant context in this conversation.

## Skill Reference

Full skill body: `skills/string-database/SKILL.md`

Load that skill file and follow its enforcement gate exactly before answering. Do not skip the
gate because this command wrapper is short — the wrapper only routes to the skill, it does not
replace it.
