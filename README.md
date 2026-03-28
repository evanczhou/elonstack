# elonstack

Run any product, startup, or engineering problem through Elon Musk's mental model pipeline. Five passes strip away conventional thinking and reveal the physics of your problem.

Every quote is from [The Book of Elon](https://www.amazon.com/dp/1544550766) by Eric Jorgenson, compiled from Elon's transcripts, tweets, and interviews. Real words, not AI cosplay.

## Install

```bash
git clone https://github.com/evanzhou/elonstack.git ~/.claude/skills/elonstack
```

## Skills

### /ElonBrain (the full pipeline)

One command. Five passes. An Idiot Index score.

```
/ElonBrain My SaaS has 3 engineers, $15k/mo infra, charges $50/mo, and growth is stalling
```

**The 5 passes:**

1. **First Principles**: decompose to physics fundamentals
2. **Idiot Index**: compute the gap between current approach and physics-optimal
3. **The Algorithm**: question, delete, simplify, accelerate, automate (in that order)
4. **Think in Limits**: scale to 10x and 1000x, find what breaks
5. **Bottleneck Attack**: find the single constraint that sets the rate

### Individual skills

Use these when you know exactly which mental model you need. `/ElonBrain` gives you breadth (5 compact passes). Individual skills give you depth (one pass, fully expanded with follow-up questions and action framing).

| Skill | What it does |
|-------|-------------|
| `/FirstPrinciples` | Strip to irreducible truths |
| `/IdiotIndex` | Compute the gap to physics-optimal |
| `/TheAlgorithm` | Run the 5-step engineering process |
| `/ThinkInLimits` | Scale to extremes, find what breaks |
| `/BottleneckAttack` | Find the single rate-limiting constraint |

## Example Output

```
ELONBRAIN ANALYSIS: SaaS with stalling growth
=========================================

PASS 1: FIRST PRINCIPLES
- Core value delivery: users get [specific thing]
- Distribution: how users find the product
- Retention mechanism: what keeps them paying
- Infrastructure: what actually runs the service
- Coordination cost: what the 3 engineers spend time on

> "The normal way we conduct our lives is reasoning by analogy.
>  When you think this way, you only get slight iterations."

PASS 2: IDIOT INDEX
Current approach: 3 engineers + $15k/mo infra
Physics-optimal: 1 engineer + $500/mo infra

  IDIOT INDEX: 5x

> "If the ratio is high, you're an idiot."

PASS 3: THE ALGORITHM
1. REQUIREMENTS: Who decided you need 3 engineers? Name them.
2. DELETE: Which of your features do <5% of users touch? Kill them.
3. SIMPLIFY: Your infra bill suggests overengineering. Simplify the stack.
4. ACCELERATE: Ship weekly, not monthly. Faster feedback loops.
5. AUTOMATE: Only after steps 1-4. Not before.

> "The most common mistake of smart engineers is to
>  optimize a thing that should not exist."

PASS 4: THINK IN LIMITS
| Component    | At 10x       | At 1000x        |
|-------------|-------------|-----------------|
| Infra       | Scales fine  | Need redesign   |
| Team        | 5 engineers  | Process breaks  |
| Revenue     | $250k/mo    | Unit economics? |

> "Ask, 'If our volume was a million units per year,
>  would it still be expensive?'"

PASS 5: BOTTLENECK
Your bottleneck is not engineering. It's distribution.
3 engineers building features nobody finds.
Fix distribution before touching the product.

> "The production line will move as fast as the slowest
>  and least lucky part of the entire production line."

=========================================
VERDICT: You're overinvesting in product, underinvesting
in distribution. The Idiot Index on your team structure is 5x.
IDIOT INDEX: 5x
ACTION: Cut infra spend 70%, redeploy one engineer to growth.
=========================================
```

## Migration

If you have the standalone `/ElonAlgorithm` skill, elonstack replaces it. You can safely remove `~/.claude/skills/ElonAlgorithm/`.

## Source

All quotes from "The Book of Elon" by Eric Jorgenson. The book was released as a free epub. Passages quoted under fair use for educational purposes in an open source tool.

## License

MIT
