# Economy System

**Complete guide to the SkillCoins economy**

## Overview

The economy system is built on **SkillCoins** (⛃) as the primary currency, with **SkillTokens** (🎟) as premium currency. Unlike traditional economies, SkillCoins are earned through gameplay rather than admin commands.

## Currency Types

| Currency | Symbol | Purpose |
|----------|--------|---------|
| SkillCoins | ⛃ | Main currency for all purchases |
| SkillTokens | 🎟 | Premium items and special purchases |

## Earning Currency

### Quest Rewards

The tutorial and daily quests provide significant income:

| Source | Reward |
|--------|--------|
| Tutorial (6 quests) | 1,415 ⛃ + 10 🎟 |
| Daily Quests | 50-200 ⛃/day |

### Skill Progression

Leveling skills earns SkillCoins:
- First levels: 10-20 ⛃
- Mid levels: 20-40 ⛃
- High levels: 40-50 ⛃

### Selling Items

Sell items in the shop


## Balance Commands

### Check Balance

```
/skillcoins balance
/sc balance
```

**Output:**
```
━━━━ Your Balance ━━━━
⛃: 1,234.56
🎟: 10.00
━━━━━━━━━━━━━━━━━━━━
```

### Admin Commands

| Command | Description |
|---------|-------------|
| `/sc give <p> <amt>` | Give coins/tokens |
| `/sc take <p> <amt>` | Take coins/tokens |
| `/sc set <p> <amt>` | Set exact balance |
| `/sc check <p>` | View player balance |

## Player Data

Balances stored per-player:

```yaml
{coins: 1234.56, tokens: 10.0}
```

**Location:** `plugins/AuraSkills/skillcoins/{uuid}.yml`

## Related Files

- [Token Economy](systems/economy/token-economy.md) - Premium tokens
- [Shop System](systems/economy/shop-system.md) - Buying/selling items
- [Skill Rewards](systems/skills/skill-rewards.md) - Coins from skills
