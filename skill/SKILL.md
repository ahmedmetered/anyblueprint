---
name: anyblueprint
description: >-
  Documentation-first project planning that produces implementation-ready
  blueprints and single-shot coding agent prompts. Generates four
  interconnected documents - SPECIFICATION.md, IMPLEMENTATION.md, TASKS.md,
  BRANDING.md - plus a self-contained PROMPT.md for autonomous execution by
  any coding agent. Includes interactive tech stack selection, design pattern
  recommendations, and architecture decisions with trade-off analysis. Use
  when the user wants to plan a project, create specs, architect a system,
  break work into tasks, choose a tech stack, get design pattern advice, or
  do documentation-first development.
---

# anyblueprint

A documentation-first planning system: think deeply, document thoroughly,
then execute with zero ambiguity. Produces implementation-ready blueprints
and an agent-ready prompt. Adapted from
[project-architect](https://github.com/ersinkoc/project-architect) (MIT),
repackaged so the references travel with the skill and work from any agent's
skills folder.

## Output pipeline

```
[Discovery]  ->  SPECIFICATION.md  ->  IMPLEMENTATION.md  ->  TASKS.md  ->  BRANDING.md
                  (the what)          (the how)             (the work)  (identity)
                        \                  |                   /
                         \_________________|_________________/
                                            |
                                       PROMPT.md
                              (single-shot agent prompt)
```

Each document feeds the next. PROMPT.md synthesizes everything into one
self-contained prompt that any coding agent can execute.

## Reference files

Read the matching reference before generating each document. Paths are
relative to this skill's folder:

| Phase | Reference | Read when |
|---|---|---|
| Discovery | `references/elicitation-guide.md` | Before asking any questions |
| Tech stack | `references/tech-stacks.md` | The user needs stack selection help |
| Patterns | `references/design-patterns.md` | Making architecture decisions |
| Specification | `references/specification-guide.md` | Before writing SPECIFICATION.md |
| Implementation | `references/implementation-guide.md` | Before writing IMPLEMENTATION.md |
| Tasks | `references/tasks-guide.md` | Before writing TASKS.md |
| Branding | `references/branding-guide.md` | Before writing BRANDING.md |

## Rules

- Discovery before documents: run the elicitation questions first; a spec
  written from assumptions is a fiction with formatting.
- Every document is written to the candidate's project folder, never inside
  the skill.
- Trade-off analysis names the rejected options and why, not just the winner.
- PROMPT.md is self-contained: an agent that has never seen the other four
  documents can execute it correctly.
