# Skills System

**Progression through activities using AuraSkills**

## Supported Skills

| Skill | Activity | XP Source |
|-------|----------|-----------|
| Foraging | Woodcutting | Breaking logs |
| Mining | Mining | Mining ores/stone |
| Farming | Harvesting | Crops and animals |
| Archery | Combat | Bow hits |
| Smelting | Furnace | Smelting items |
| Excavation | Digging | Shovel use |
| Agility | Movement | Running, jumping |

## XP Formula

Skills use logarithmic scaling:

```
XP Required = Base × Level^1.5
```

**Example:**
| Level | XP Required |
|-------|-------------|
| 1 | 100 |
| 10 | 3,162 |
| 25 | 12,500 |
| 50 | 35,355 |
| 100 | 100,000 |

## Opening Skills Menu

```
/skills
```

**Features:**
- All skills displayed with levels
- XP progress bars
- Click for details
- Abilities menu

## Skill Commands

| Command | Description |
|---------|-------------|
| `/skills` | Main menu |
| `/skills <skill>` | Specific skill |
| `/skills abilities` | Ability menu |
| `/skills stats` | Overall statistics |

## XP Sources

### Foraging

| Block | XP |
|-------|----|
| Oak Log | 10 |
| Birch Log | 12 |
| Spruce Log | 15 |
| Jungle Log | 20 |
| Acacia Log | 18 |
| Dark Oak Log | 22 |

### Mining

| Block | XP |
|-------|----|
| Stone | 10 |
| Coal Ore | 15 |
| Iron Ore | 20 |
| Gold Ore | 25 |
| Diamond Ore | 35 |
| Ancient Debris | 50 |

### Farming

| Crop | XP |
|------|----|
| Wheat | 5 |
| Carrots | 7 |
| Potatoes | 7 |
| Beetroots | 8 |

## Level Up Rewards

| Level Range | Coins |
|-------------|-------|
| 1-10 | 10-20 ⛃ |
| 11-50 | 20-40 ⛃ |
| 51-100 | 40-50 ⛃ |

## PlaceholderAPI

| Placeholder | Description |
|-------------|-------------|
| `%auraskills_xp_{skill}%` | Current XP |
| `%auraskills_level_{skill}%` | Current level |
| `%auraskills_xp_needed_{skill}%` | XP to next level |
| `%auraskills_total_level%` | All levels sum |

## Related Files

- [Skill Rewards](systems/skills/skill-rewards.md) - Coin rewards per level
- [Skill Abilities](systems/skills/skill-abilities.md) - Active abilities
- [Skill Sources](systems/skills/skill-sources.md) - Configured XP sources
