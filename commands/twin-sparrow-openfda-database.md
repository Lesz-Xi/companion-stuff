---
description: "Query, search, and download data from the openFDA API for drugs, devices, foods, tobacco, cosmetics, animal and veterinary products, substances, and transparency data. Use for FDA adverse events, r..."
argument-hint: "<task, question, or artifact to apply this skill to>"
---

# /twin-sparrow-openfda-database

Apply the **openfda-database** skill from the Twin-Sparrow skill registry.

## Usage

```
/twin-sparrow-openfda-database $ARGUMENTS
```

If arguments are given, treat them as the task, question, or artifact this skill should apply to.
If no arguments are given, ask Chief what to apply openfda-database to, or apply it to the most recent
relevant context in this conversation.

## Skill Reference

Full skill body: `skills/openfda-database/SKILL.md`

Load that skill file and follow its enforcement gate exactly before answering. Do not skip the
gate because this command wrapper is short — the wrapper only routes to the skill, it does not
replace it.
