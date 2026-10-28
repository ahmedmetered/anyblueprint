# anyblueprint

Documentation-first project planning from the AI agent you already have.

Interview-driven discovery, then four interconnected documents -
SPECIFICATION.md (the what), IMPLEMENTATION.md (the how), TASKS.md (the
work), BRANDING.md (the identity) - synthesized into one self-contained
PROMPT.md that any coding agent can execute single-shot. Interactive tech
stack selection, design pattern recommendations, and architecture decisions
with named trade-offs.

Adapted from [project-architect](https://github.com/ersinkoc/project-
architect) (MIT) by ersinkoc, repackaged as an agent-native skill whose
references travel with it: no plugin root variable, no specific CLI.

## Install

Copy `skill/` into your agent's skills folder (ZCode, Claude Code, Codex,
Cursor - any agent that reads `SKILL.md` files), or clone this repository
into it; the root `SKILL.md` makes it discoverable either way.

## Use

- "Plan my project: I want to build X"
- "Spec this out before we code"
- "Break this into tasks and generate a coding agent prompt"

## Files

```
skill/SKILL.md        the pipeline: discovery -> four documents -> PROMPT.md
skill/references/     8 guides: elicitation, tech stacks, design patterns,
                      specification, implementation, tasks, branding, agent prompt
```

## Credits and license

MIT. Content adapted from
[project-architect](https://github.com/ersinkoc/project-architect) by
ersinkoc. Independent project; not affiliated with or endorsed by Anthropic
or any agent vendor.
