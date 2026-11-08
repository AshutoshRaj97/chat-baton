# context-handoff

A Claude Code skill that packages your current chat into a compact `HANDOFF.md` so a fresh session can continue without re-explaining anything.

## Install

```
/plugin marketplace add <your-github-user>/context-handoff
/plugin install context-handoff@ashutosh-skills
```

## Use

In a long session, say "handoff" or run `/context-handoff`. Then in a new chat:

```
Read HANDOFF.md and continue from "Next steps".
```

## What the brief contains

Goal, current state, key decisions and why, your preferences, important context, open questions, next steps. Secrets are never included.
