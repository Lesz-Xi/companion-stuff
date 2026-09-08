---
description: "Query the OpenAlex scholarly database for research papers, authors, institutions, topics, sources, publishers, funders, geo-locations, and keywords. Use when searching academic papers, resolving DO..."
argument-hint: "<task, question, or artifact to apply this skill to>"
---

# /twin-sparrow-literature-search-openalex

Apply the **literature-search-openalex** skill from the Twin-Sparrow skill registry.

## Usage

```
/twin-sparrow-literature-search-openalex $ARGUMENTS
```

If arguments are given, treat them as the task, question, or artifact this skill should apply to.
If no arguments are given, ask Chief what to apply literature-search-openalex to, or apply it to the most recent
relevant context in this conversation.

## Skill Reference

Full skill body: `skills/literature-search-openalex/SKILL.md`

Load that skill file and follow its enforcement gate exactly before answering. Do not skip the
gate because this command wrapper is short — the wrapper only routes to the skill, it does not
replace it.
