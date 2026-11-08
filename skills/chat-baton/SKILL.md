---
name: chat-baton
description: Package the current conversation into a compact handoff brief that can be pasted into (or loaded by) a brand-new chat so work continues without re-explaining. Use when the user says "handoff", "port this chat", "continue in a new chat", "context is getting long", or "summarize so I can start fresh".
---

# Chat Baton

Create a self-contained brief that lets a fresh session pick up exactly where this one stops.

## Steps

1. **Review the whole conversation.** Identify the goal, decisions made, current state, and what remains.
2. **Write the brief** using the template below. Be specific and concrete: exact file paths, commands, names, versions, error messages. Omit pleasantries, dead ends that are fully resolved, and anything derivable from the code.
3. **Save it** to `HANDOFF.md` in the working directory (or print it in a code block if there is no filesystem). Tell the user the path.
4. **Give the user the restart line**: `Read HANDOFF.md and continue from "Next steps".` (for non-filesystem chats: "paste the brief as your first message").
5. **Never include secrets** (API keys, tokens, passwords). Note that they exist and where they are stored instead.

## Template

```markdown
# Handoff: <short title>
_Created: <date>_

## Goal
One or two sentences on what the user is ultimately trying to achieve.

## Current state
- What is done and working (with file paths / links)
- What is in progress or broken (with exact errors)

## Key decisions & why
- Decision — reason (so the new chat doesn't re-litigate it)

## User preferences & constraints
- Style, tools, stack, things to avoid, things the user corrected

## Important context
- Facts, names, IDs, URLs, commands needed to continue

## Open questions
- Anything unresolved that needs the user's input

## Next steps
1. Concrete first action
2. ...
```

## Quality bar

- A reader with zero prior context should be able to act on it in under a minute.
- Prefer facts over narrative. Keep it under ~1 page unless the project truly needs more.
- Flag anything uncertain as "unverified" rather than stating it as fact.
