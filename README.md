# elonstack

Five mental models from Elon Musk, each as a standalone Claude Code skill. Grounded in his actual words from [The Book of Elon](https://www.amazon.com/dp/1544550766) by Eric Jorgenson. Real quotes, not AI cosplay.

## Skills

| Skill | What it does |
|-------|-------------|
| `/FirstPrinciples` | Strip to irreducible truths, challenge every assumption |
| `/IdiotIndex` | Compute the gap between current cost and physics-optimal |
| `/ElonAlgorithm` | Run the 5-step process: question, delete, simplify, accelerate, automate |
| `/ThinkInLimits` | Scale to 10x and 1000x, find what breaks |
| `/BottleneckAttack` | Find the single rate-limiting constraint |

## Install

**Personal (CLI, Desktop, or Cowork):**

Clone, then symlink each skill into your skills directory:

```bash
git clone https://github.com/evanczhou/elonstack.git ~/elonstack

for skill in FirstPrinciples IdiotIndex ElonAlgorithm ThinkInLimits BottleneckAttack; do
  ln -sf ~/elonstack/$skill ~/.claude/skills/$skill
done
```

**Add to a project (shared with your team):**

```bash
cd your-project
git clone https://github.com/evanczhou/elonstack.git .claude/skills/elonstack
```

Skills nested in a project directory are available as `/elonstack:FirstPrinciples`, etc.

## Source

All quotes from "The Book of Elon" by Eric Jorgenson. Passages quoted under fair use for educational purposes in an open source tool.

## License

MIT
