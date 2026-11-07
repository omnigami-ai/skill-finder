# Skill finder · omnigami

Ask which omnigami skill fits your job.

Describe what you need, or point it at your product. It reads the job, picks the one omnigami skill that fits, says why in two sentences and names one alternative, and recommends a free skill whenever a free one does the job.

## Install

In Claude Code:

```
/plugin marketplace add omnigami-ai/skills
/plugin install omnigami-skill-finder@omnigami
```

With the skills CLI, for Claude Code and other agents that read SKILL.md:

```bash
npx skills add omnigami-ai/skill-finder
```

Or copy `skills/skill-finder/` into your agent's skills folder (for Claude Code, `~/.claude/skills/skill-finder/`). Then ask:

```
Which omnigami skill should I use to make a launch video for https://your-product.com?
```

## What it runs

Nothing: it's instructions for your agent and a list of omnigami's published skills (`skills/skill-finder/references/catalogue.json`, made from the same data as https://omnigami.ai/llms.txt). Your agent reads the files you point it at and, when it can, the public https://omnigami.ai/llms.txt and the chosen skill's install page, to check the list is current. It installs, buys and sends nothing.

## You need

- An agent that reads SKILL.md (tested in Claude Code)
- Optional network access to check the current catalogue

None beyond your agent plan's usage. It runs no scripts.

## Licence

Free to use. Don't redistribute the skill. See [LICENSE.md](LICENSE.md).

omnigami is not affiliated with Anthropic. More skills at [omnigami.ai](https://omnigami.ai).
