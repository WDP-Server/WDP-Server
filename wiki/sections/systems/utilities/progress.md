# Progress System

**WDP-Progress - Overall player score (1-100)**

## Score Breakdown

| Category | Weight | Description |
|----------|--------|-------------|
| Advancements | 25% | Minecraft achievements |
| Experience | 15% | XP levels |
| Equipment | 20% | Armor, tools, enchantments |
| Economy | 15% | SkillCoins balance |
| Statistics | 15% | Kills, mining, exploration |
| Achievements | 10% | Server milestones |

## Display

Progress bar with color coding:

| Range | Color | Rank |
|-------|-------|------|
| 0-20% | 🔴 Red | Beginner |
| 21-40% | 🟠 Gold | Novice |
| 41-60% | 🟡 Yellow | Intermediate |
| 61-80% | 🟢 Green | Advanced |
| 81-100% | 🔵 Aqua | Master |

**Format:**
```
████████████████████░░░░ 65%
```

## Key Milestones

| Milestone | Points |
|-----------|--------|
| First Join | +1.0 |
| Complete Tutorial | +5.0 |
| Kill Dragon | +20.0 |
| Get Wither Skull | +10.0 |
| Summon Wither | +12.0 |
| Elytra | +15.0 |
| Max Level 100 | +5.0 |

## Death Penalty

- Temporary -2% penalty
- Recovers after 1 hour
- Equipment loss affects score (30%)

## Commands

```
/progress           # View score
/progress breakdown # Category details
/progress tips      # Improvement tips
```

## PlaceholderAPI

| Placeholder | Description |
|-------------|-------------|
| `%progress_score%` | Overall score |
| `%progress_advancements%` | Advancement score |
| `%progress_experience%` | Experience score |
| `%progress_equipment%` | Equipment score |
| `%progress_economy%` | Economy score |
| `%progress_statistics%` | Statistics score |
