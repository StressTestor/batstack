# batstack v0.1 spec

## Methodology

v0.1 work is an audit of every gstack skill against PHILOSOPHY.md, producing one of three outcomes per skill:

1. **Improve** — function is good, framing is bad. Write a batstack version that does the same work without persona theater or YC vocabulary.

2. **Replace** — function is gstack-philosophy-shaped (the skill exists to roleplay a YC org chart role). Write a different batstack skill that does similar useful work for a solo builder.

3. **Skip** — not the workflow, no analogous work worth doing for personal projects, or function genuinely doesn't apply.

The audit IS the work. Once a skill is categorized, the implementation is mechanical: read gstack's prompt, write a better one against PHILOSOPHY.md, commit.

## v0.1 ship target

Today's v0.1 ships with the audit complete + the 5-7 most-used skills implemented:

- `/review` (most-used)
- `/health`
- `/ship`
- `/retro`
- `/think` (replacing `/office-hours`)
- `/qa-cli`
- `/document` (replacing `/document-release`)

These are the skills used in the last 24 hours. They get the attention first because they get used the most.

## Architecture

- Pure markdown skill files at `skills/<skill-name>/SKILL.md`
- `setup` and `uninstall` shell scripts mirroring gstack's pattern
- Symlinks at `~/.claude/skills/<skill-name>` → repo
- README, LICENSE (MIT), PHILOSOPHY.md, AUDIT.md, SPEC.md
- No bun, no binaries, no telemetry, no upgrade plumbing
- Unprefixed skill names (uninstalling gstack means no collision)
- Public repo from day one: StressTestor/batstack

## Build order

1. Repo skeleton: README, LICENSE, PHILOSOPHY.md, SPEC.md, .gitignore
2. setup + uninstall shell scripts
3. Audit pass: read each gstack skill, categorize improve/replace/skip in AUDIT.md with reasoning per skill
4. Implement the 5-7 v0.1 skills, one commit per skill
5. Tag v0.1.0
6. Uninstall gstack on local machine
7. Install batstack
8. Smoke test by running `/retro` on the batstack repo itself

## AUDIT.md format

Each gstack skill gets an entry like:

```
## /skill-name
- **Category:** improve | replace | skip
- **Function:** one sentence describing what the skill does
- **Framing problems:** specific quotes from the gstack prompt
- **Batstack approach:** what the rewrite/replacement looks like, or why we're skipping
- **v0.1 priority:** high | medium | defer
```
