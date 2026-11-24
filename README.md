# handoff

A free skill that writes a handoff note, so the next person (or the next AI session) can pick up your work without re-reading the whole chat.

Say "write a handoff", "I'm passing this to Sam" or "save where we are before I clear context", and you get a short note with:

- **The goal:** what done looks like
- **Where it stands:** done, in progress, not started
- **Decisions made, and why**
- **Tried and dropped,** so nobody tries it again
- **Open questions,** and who can answer them
- **Do this next**
- **Don't:** anything the next person must not redo

It keeps the note under about 300 words, links to files instead of pasting them, and leaves out secrets.

## Install

It's a standard [Agent Skill](https://agentskills.io): one folder with a `SKILL.md` (in `skills/handoff/`).

**Claude Code** (as a plugin, gets updates):

```
/plugin marketplace add tekhnea/handoff-skill
/plugin install handoff@tekhnea
```

**Any tool the `skills` CLI supports** (Claude Code, Cursor, Codex and others):

```bash
npx skills add tekhnea/handoff-skill
```

**By hand.** Copy `skills/handoff` into your tool's skills folder, for example `~/.claude/skills/` for Claude Code.

**Claude (claude.ai and the desktop app).** Download `handoff.zip` from the [latest release](https://github.com/tekhnea/handoff-skill/releases/latest) and upload it in Claude's skills settings (code execution must be on).

**ChatGPT and other tools.** If your tool supports Agent Skills, add the `handoff` folder or the zip there. If it doesn't, paste the contents of `skills/handoff/SKILL.md` into its custom instructions or rules.

## Why we made it

Lots of people who work with Claude Code or Cursor already write handoff notes by hand before clearing context or passing work on. This skill gives the note a consistent shape. The section people skip, and regret skipping, is "decisions made, and why": without it, the next person re-opens choices that were already settled.

We're building [Tekhnea](https://tekhnea.com) for the team version: the handoff goes straight from your AI to a teammate's Claude, ChatGPT, Cursor or Claude Code, and their questions and decision come back to you. This skill is free and works on its own.

## License

MIT
