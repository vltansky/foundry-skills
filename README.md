# Foundry Skills

A collection of [Agent Skills](https://agentskills.io) for Claude Code, Cursor, Codex, and other coding agents.

## Install All

```bash
npx skills add vltansky/foundry-skills/skills --all -g
```

Installs all skills globally with symlinks to `~/.agents/skills/`, `~/.claude/skills/`, `~/.cursor/skills/`, and any other detected agents.

## Install Individual

```bash
npx skills add vltansky/foundry-skills/skills/ux-reviewer -g -y
```

### Reviewing

| Skill | Description |
|-------|-------------|
| [ux-reviewer](skills/ux-reviewer) | Sharp, evidence-backed UX review of an existing flow, screen, prototype, screenshot, or live product |
| [prod-reviewer](skills/prod-reviewer) | _Placeholder — scope TBD_ |

### Product

| Skill | Description |
|-------|-------------|
| [grill-product](skills/grill-product) | Analyze an existing product then grill, challenge, and push back to improve it (also shapes new ideas). Lenses: signals, framing, tradeoffs, GTM, first experience |

## License

MIT
