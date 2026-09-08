---
description: "Query the QuickGO and Evidence & Conclusion Ontology (ECO) REST API. Use this when you need to map genes to biological processes, molecular functions, or cellular components, find genes associated..."
argument-hint: "<task, question, or artifact to apply this skill to>"
---

# /twin-sparrow-quickgo-database

Apply the **quickgo-database** skill from the Twin-Sparrow skill registry.

## Usage

```
/twin-sparrow-quickgo-database $ARGUMENTS
```

If arguments are given, treat them as the task, question, or artifact this skill should apply to.
If no arguments are given, ask Chief what to apply quickgo-database to, or apply it to the most recent
relevant context in this conversation.

## Skill Reference

Full skill body: `skills/quickgo-database/SKILL.md`

Load that skill file and follow its enforcement gate exactly before answering. Do not skip the
gate because this command wrapper is short — the wrapper only routes to the skill, it does not
replace it.
