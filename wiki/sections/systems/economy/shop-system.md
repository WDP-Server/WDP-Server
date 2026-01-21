# Shop System

**GUI-based item buying and selling**

## Opening the Shop

```
/shop
```

**Permission:** `auraskills.command.shop`

## Main Menu Layout

```
┌─────────────────────────────────────────────┐
│ 🏪 Shop                    ⛃: 1,234.56     │
├─────────────────────────────────────────────┤
│ [Tools]  [Combat]  [Blocks]  [Enchantments] │
│ [Farming][Potions] [Food]   [Redstone]      │
│ [Spawners][Eggs]   [Music]  [Decoration]    │
│ [Dyes]   [Workstation][Misc][Tokens]        │
├─────────────────────────────────────────────┤
│ [← Prev]  [Page 1/2]  [Next →]   [Back/✕]  │
└─────────────────────────────────────────────┘
```

## Category Reference

| Slot | Category | Items |
|------|----------|-------|
| 11 | Tools | Pickaxes, axes, shovels |
| 12 | Combat | Swords, armor, bows |
| 13 | Enchantments | Enchanted books |
| 14 | Potions | Splash & regular |
| 15 | Food | Raw & cooked |
| 16 | Farming | Seeds, saplings |
| 17 | Redstone | Torches, pistons |
| 18 | Spawners | Mob spawners |
| 19 | Spawn Eggs | All mob types |
| 20 | Music | Records, jukeboxes |
| 21 | Decoration | Item frames, banners |
| 22 | Dyes | All 16 colors |
| 23 | Workstations | Crafting, furnaces |
| 24 | Miscellaneous | Torches, beds, etc |
| 25 | Token Exchange | Premium items |

## Buying Items

1. Click category
2. Find item
3. Click to buy
4. Confirm in chat

## Selling Items

1. Right-click item in shop
2. Adjust quantity
3. Click "Sell"
4. Receive 30% of buy price

## Price Reference

### Weapons

| Item | Buy | Sell |
|------|-----|------|
| Wooden Sword | 5 ⛃ | 1 ⛃ |
| Stone Sword | 8 ⛃ | 2 ⛃ |
| Iron Sword | 35 ⛃ | 10 ⛃ |
| Diamond Sword | 150 ⛃ | 45 ⛃ |
| Netherite Sword | 500 ⛃ | 150 ⛃ |

### Tools

| Item | Buy | Sell |
|------|-----|------|
| Iron Pickaxe | 40 ⛃ | 12 ⛃ |
| Diamond Pickaxe | 175 ⛃ | 52 ⛃ |
| Netherite Pickaxe | 600 ⛃ | 180 ⛃ |

### Armor (Full Sets)

| Material | Cost |
|----------|------|
| Leather | ~30 ⛃ |
| Iron | ~150 ⛃ |
| Diamond | ~600 ⛃ |
| Netherite | ~2,000 ⛃ |

### Enchantments

| Enchant | Level | Buy | Sell |
|---------|-------|-----|------|
| Protection | IV | 150 ⛃ | 45 ⛃ |
| Sharpness | V | 200 ⛃ | 60 ⛃ |
| Efficiency | V | 100 ⛃ | 30 ⛃ |
| Fortune | III | 250 ⛃ | 75 ⛃ |
| Mending | I | 300 ⛃ | 90 ⛃ |

### Building Blocks

| Item | Buy | Sell |
|------|-----|------|
| Cobblestone | 1 ⛃ | 0 ⛃ |
| Glass | 5 ⛃ | 1 ⛃ |
| Obsidian | 20 ⛃ | 6 ⛃ |
| Diamond Block | 900 ⛃ | 270 ⛃ |

## Troubleshooting

### Cannot Open Shop

- Check permission: `auraskills.command.shop`
- Verify shop files loaded

### Cannot Afford

- Complete more quests
- Sell items to shop
- Level up skills

### Cannot Sell

- Item must match exactly
- Full durability required
- No custom names/data
