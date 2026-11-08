# chat-baton

A Claude Code skill that packages your current chat into a compact `HANDOFF.md` so a fresh session can continue without re-explaining anything.

## Install

```
/plugin marketplace add AshutoshRaj97/chat-baton
/plugin install chat-baton@ashutosh-skills
```

## Use

In a long session, say "handoff" or run `/chat-baton`. Then in a new chat:

```
Read HANDOFF.md and continue from "Next steps".
```

## What the brief contains

Goal, current state, key decisions and why, your preferences, important context, open questions, next steps. Secrets are never included.
