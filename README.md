# Skills

My personal agent skills.

## Skills

- [carryover](skills/carryover/SKILL.md): Prepare a context handoff for a new agent session. Explicit invocation only.
- [reframe](skills/reframe/SKILL.md): Re-explain the previous response in clear technical English. Explicit invocation only.

## Install

```sh
npx skills add Liakhov/skills --skill carryover
npx skills add Liakhov/skills --skill reframe
```

Invoke a skill with `$carryover` or `$reframe` in Codex, or `/carryover` or `/reframe` in Claude Code.

## Add a skill

Create `skills/<name>/SKILL.md` following the [Agent Skills format](https://agentskills.io/specification), then add it to the list above.
