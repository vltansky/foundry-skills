# Foundry Skills

A collection of [Agent Skills](https://agentskills.io) for Claude Code, Cursor, Codex, and other coding agents.

## Install

The default and recommended way is the [`skills`](https://github.com/vercel-labs/skills) CLI, which detects your installed agents and symlinks the skills into each one.

```bash
# All skills, all detected agents, globally
npx skills add vltansky/foundry-skills/skills --all -g

# A single skill
npx skills add vltansky/foundry-skills/skills/ux-reviewer -g -y
```

### Target a specific agent

Pass `-a <agent>` to install only for that agent (`-g` for global, omit for the current project):

```bash
npx skills add vltansky/foundry-skills/skills --all -g -a claude-code   # Claude Code
npx skills add vltansky/foundry-skills/skills --all -g -a cursor        # Cursor
npx skills add vltansky/foundry-skills/skills --all -g -a codex         # Codex
```

### Manual install

A skill is just a folder containing a `SKILL.md`. If you'd rather not use the CLI, clone this repo and copy (or symlink) the skill folder into your agent's skills directory:

```bash
git clone https://github.com/vltansky/foundry-skills.git
# Example: ux-reviewer into Claude Code, globally
cp -R foundry-skills/skills/ux-reviewer ~/.claude/skills/ux-reviewer
```

Skills directories per agent:

| Agent | Global | Project |
|-------|--------|---------|
| Claude Code | `~/.claude/skills/` | `.claude/skills/` |
| Cursor | `~/.cursor/skills/` | `.agents/skills/` |
| Codex | `~/.codex/skills/` | `.agents/skills/` |

Use `ln -s "$PWD/foundry-skills/skills/ux-reviewer" ~/.claude/skills/ux-reviewer` instead of `cp -R` if you want updates to follow `git pull`.

### Reviewing

| Skill | Description |
|-------|-------------|
| [ux-reviewer](skills/ux-reviewer) | Sharp, evidence-backed UX review of an existing flow, screen, prototype, screenshot, or live product |

### Product

| Skill | Description |
|-------|-------------|
| [grill-product](skills/grill-product) | Analyze an existing product then grill, challenge, and push back to improve it (also shapes new ideas). Lenses: signals, framing, tradeoffs, GTM, first experience |

## License

MIT
