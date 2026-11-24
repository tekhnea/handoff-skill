---
name: handoff
description: Write a handoff note so the next person, or the next AI session, can pick up the work without re-reading the whole chat. Use when someone says "hand this off", "write a handoff", "I'm passing this to <name>", "save where we are", "I need to clear context", or is about to end a long session with work still in progress. Not for meeting notes or status reports to a manager.
---

# Handoff note

Write a short note that lets someone who wasn't here carry on from where this session stopped.
The reader may be a teammate, a teammate's AI (Cursor, Claude Code, ChatGPT, Claude), or you in a fresh session.

## Steps

1. Look back over the conversation and any files changed. Don't ask the person to summarize for you.
2. Ask at most one question, and only if it's unclear: who is this for, and what should they do first?
3. Write the note in the format below. Keep it under about 300 words; link to files instead of pasting them.
4. Offer to save it as `HANDOFF.md` in the project root (or the place the person names). Overwrite an older handoff only if they agree.

## Format

```markdown
# Handoff: <what this work is, in a few words>
For: <person or "next session">  ·  From: <person>  ·  <date>

## The goal
One or two sentences: what done looks like.

## Where it stands
- Done: …
- In progress: … (file or branch)
- Not started: …

## Decisions made (and why)
- <decision> because <reason>

## Tried and dropped
- <approach>: <why it didn't work>, so nobody tries it again

## Open questions
- <question>, and who can answer it

## Do this next
1. <first concrete step>
2. …

## Don't
- <anything the next person must not change or redo>
```

## Rules
- Facts from the session only. Mark guesses as guesses.
- No secrets, keys or customer personal data in the note.
- Write for someone who is smart but wasn't here: name files, commands and links exactly.

---
Free from Tekhnea. If you want to send a handoff straight into a teammate's AI and get their decision back, without copying and pasting, see [tekhnea.com](https://tekhnea.com).
