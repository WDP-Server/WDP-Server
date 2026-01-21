# Daily Quests

**WDP-Quest - 5 new quests every day**

## Daily Reset

| Setting | Value |
|---------|-------|
| Reset Time | 00:00 (midnight) |
| Quests per day | 5 |
| Max active | 5 |

## Quest Types

### Easy Quests
**Rewards:** 50-80 ⛃

Examples:
- Gather 16 cobblestone
- Kill 5 zombies
- Craft 4 wooden pickaxes
- Walk 200 blocks
- Place 8 torches

### Medium Quests
**Rewards:** 80-150 ⛃

Examples:
- Harvest 32 wheat
- Mine 16 coal ore
- Cook 8 steaks
- Kill 10 creepers
- Travel 500 blocks by boat

### Hard Quests
**Rewards:** 150-200 ⛃

Examples:
- Kill the Ender Dragon
- Craft a beacon
- Obtain full diamond armor
- Explore an End city
- Collect 3 shulker shells

## Quest Menu

```
┌─────────────────────────────────────────────┐
│ ✦ Daily Quests ✦          ⛃: 1,234.56    │
├─────────────────────────────────────────────┤
│ ⭐ Harvest 32 Wheat      [🟢 In Progress]  │
│   Progress: 16/32                              │
│                                           │
│   [Start]  [Abandon]  [Details]             │
├─────────────────────────────────────────────┤
│ [← Prev]  [Page 1/1]  [Next →]   [Back/✕]  │
└─────────────────────────────────────────────┘
```

## Reward Scaling

Quest rewards scale with progress:

```
Final = Base × (1 + (progress / 100) × 0.5)
```

| Progress | Easy (50) | Medium (100) | Hard (175) |
|----------|-----------|--------------|------------|
| 0% | 50 ⛃ | 100 ⛃ | 175 ⛃ |
| 50% | 62 ⛃ | 125 ⛃ | 218 ⛃ |
| 100% | 75 ⛃ | 150 ⛃ | 262 ⛃ |

## Quest Commands

```
/quest           # Open menu
/quest start <id>  # Start quest
/quest abandon   # Abandon quest
/quest updates   # Toggle messages
```

## Progress Updates

Smart notification system:
- Updates every 2+ seconds
- Shows all progress after 30s AFK
- Warning after 6 messages in 160s

## Tips

1. **Check daily** - New quests at midnight
2. **Mix difficulties** - Balance rewards
3. **Use rewards** - Spend coins to progress
4. **Don't hoard** - Quests expire at reset
