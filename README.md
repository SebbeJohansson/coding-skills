# coding-skills

Agent skills I distribute from my personal account.

## Skills

| Skill | What it does |
| ----- | ------------ |
| [public-repo-scaffolding](skills/public-repo-scaffolding/SKILL.md) | How to start a new public repo from my [scaffolding template](https://github.com/SebbeJohansson/public-repo-template) |

## Related repos

- [public-repo-template](https://github.com/SebbeJohansson/public-repo-template): template for every new public repo (AGENTS.md, SECURITY.md, LICENSE, README, Go and npm publishing guides).

## Install

As a Claude Code plugin (repeat once per machine and account):

```
/plugin marketplace add SebbeJohansson/coding-skills
/plugin install coding-skills@coding-skills
```

Or copy a skill folder into `~/.claude/skills/`:

```sh
git clone https://github.com/SebbeJohansson/coding-skills.git
cp -r coding-skills/skills/public-repo-scaffolding ~/.claude/skills/
```

## License

[MIT](LICENSE).
