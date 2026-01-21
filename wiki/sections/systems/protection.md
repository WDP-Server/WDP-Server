# Protection System

**WDP-BaseDet - Automatic base detection and protection**

## How Detection Works

1. Build normally (beds, chests, doors)
2. Plugin tracks building activity
3. Score reaches threshold (150 points)
4. Detection prompt appears
5. Confirm to protect

## Scoring

| Action | Points | Max Uses |
|--------|--------|----------|
| Place bed | 20 | 1 |
| Place door | 12 | 3 |
| Place chest | 10 | - |
| Place crafting table | 8 | - |
| Place furnace | 8 | - |
| Place anvil | 7 | - |
| Place other blocks | 2 | - |
| Break blocks | 1.5 | - |
| Walk (10 blocks) | 0.1 | - |

**Proximity Bonus:** Building compact = 1.5x-2x score

## Detection Threshold

- **Default:** 150 points
- **Cooldown:** 5 minutes
- **Auto-confirm:** 10 minutes

## Protection Rules

### Owner Online

| Action | Allowed |
|--------|---------|
| Block breaking | ✅ |
| Block placing | ✅ |
| Chest access | ✅ |
| PvP | ✅ |

### Owner Offline

| Action | Allowed |
|--------|---------|
| Block breaking | ❌ |
| Block placing | ❌ |
| Chest access | ❌ |
| Door/button | ❌ |
| Entity damage | ❌ |

## Trust System

### Trust Commands

```
/trust <player>     # Trust player
/trust list         # List trusted
/trust remove <p>   # Remove trust
```

### Default Trust Permissions

| Permission | Online | Offline |
|------------|--------|---------|
| Break blocks | ✅ | ❌ |
| Place blocks | ✅ | ❌ |
| Containers | ✅ | ✅ |
| Doors/buttons | ✅ | ✅ |
| Entity damage | ✅ | ❌ |

## Commands

| Command | Description |
|---------|-------------|
| `/base` | Open base menu |
| `/base confirm` | Confirm base |
| `/base deny` | Deny base |
| `/base view` | Toggle particles |
| `/base teleport` | Teleport (50 ⛃) |

## Visual Boundaries

```
/base view
```

Shows yellow particles at base outline.

## Related Files

- [Combat Protection](protection/combat-protection.md) - PvP rules
- [Trust System](protection/trust-system.md) - Managing trust
