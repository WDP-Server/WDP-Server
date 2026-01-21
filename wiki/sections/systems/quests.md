# Quests System

**Complete quest guide for WDP Server**

## Quest Types

### Tutorial Quests (WDP-Start)

6-quest chain for new players:
1. Leave Spawn
2. Foraging Level 1
3. Shop Tutorial
4. Token Exchange
5. Quest Menu
6. Community

**Total Rewards:** 1,415 ⛃ + 10 🎟

### Daily Quests (WDP-Quest)

5 new quests every day at midnight:
- Easy: 50-80 ⛃
- Medium: 80-150 ⛃
- Hard: 150-200 ⛃

## Quest Commands

### Tutorial

| Command | Description |
|---------|-------------|
| `/start` | Open start menu |
| `/start confirm` | Confirm base |
| `/start deny` | Deny base |
| `/start cancel` | Cancel tutorial |

### Daily Quests

| Command | Description |
|---------|-------------|
| `/quest` | Open quest menu |
| `/quest start <id>` | Start specific quest |
| `/quest abandon` | Abandon active quest |
| `/quest updates` | Toggle progress messages |

## Quest Menu

```
┌─────────────────────────────────────────────┐
│ 📅 Daily Quests            ⛃: 1,234.56    │
├─────────────────────────────────────────────┤
│ [Quest 1]  [Quest 2]  [Quest 3]  [Quest 4] │
│ [Quest 5]                                 │
│                                           │
│ Time until reset: 12h 34m                  │
├─────────────────────────────────────────────┤
│ [← Prev]  [Page 1/1]  [Next →]   [Back/✕]  │
└─────────────────────────────────────────────┘
```

## Quest Status

| Icon | Meaning |
|------|---------|
| 🟢 Green | Active |
| ✅ Check | Completed |
| ⬜ Gray | Not started |
| ⭐ Gold | Hard quest |

## Related Files

- [Tutorial Quests](quests/tutorial.md) - WDP-Start guide
- [Daily Quests](quests/daily-quests.md) - WDP-Quest rotation
