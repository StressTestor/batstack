# batstack

Claude Code skills for solo builders. No org chart simulation, no funnel.

Batstack is an opinionated set of [Claude Code](https://claude.com/code)
skills built around a different philosophical answer to the same
question gstack is answering: how do you give Claude Code structured
workflows for building software?

**gstack's answer:** simulate a YC-funded startup org chart with skills
that roleplay CEO, designer, eng manager, release manager, QA.

**batstack's answer:** give Claude structured workflows for one person
building software they want to exist. The work is the work.

## Skills

- `/review` — code review for correctness, taste, and failure modes
- `/health` — code quality scorecard
- `/ship` — version bump, changelog, PR
- `/retro` — engineering retro with metrics
- `/think` — forcing-question design conversations
- `/qa-cli` — exercise CLI tools end-to-end
- `/document` — keep docs synced with what shipped

## Install
```bash
git clone https://github.com/StressTestor/batstack.git ~/.claude/skills/batstack
cd ~/.claude/skills/batstack
./setup
```

That's it. The setup script creates symlinks at `~/.claude/skills/<skill>`
pointing into this repo. No build step, no dependencies, no daemons.

## Uninstall
```bash
~/.claude/skills/batstack/uninstall
```

## Philosophy

See [PHILOSOPHY.md](./PHILOSOPHY.md) for the full version. The short
version: batstack treats personal projects as the destination, not
the starting point of a journey toward Real Software With Users. No
persona theater, no funnel, no ceremony around tasks that should
just be done.

## On gstack

Batstack is not "gstack without the bad parts." It's a different
philosophical answer to the same question, for builders whose work
isn't shaped like a venture-backed product. gstack is good software
shipping a coherent vision. Batstack ships a different one. Both
exist because solo builders and venture-backed teams have different
needs.

## License

MIT. See [LICENSE](./LICENSE).
