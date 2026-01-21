# Trust System

**Managing player access to your base**

## Trust Commands

### Grant Trust

```
/trust <player>
```

**Default permissions:**
- Online: All actions allowed
- Offline: Containers + doors only

### View Trust List

```
/trust list
```

**Shows:**
- Trusted player names
- When they were trusted
- Permission level

### Remove Trust

```
/trust remove <player>
```

### Menu Management

```
/base → Trust Manager
```

- Add/remove trust
- Edit permissions per player
- View activity

## Permission Types

| Permission | Online | Offline |
|------------|--------|---------|
| Break blocks | ✅ | ❌ |
| Place blocks | ✅ | ❌ |
| Containers | ✅ | ✅ |
| Doors/gates | ✅ | ✅ |
| Redstone | ✅ | ✅ |
| Entity damage | ✅ | ❌ |
| Item pickup | ✅ | ✅ |

## Trust Levels

### Default Trust
```
/trust <player>
```

### Custom Permissions

Edit per-player:
1. Open `/base`
2. Click "Trust Manager"
3. Select player
4. Toggle permissions
5. Save

## Discord Trust

If Discord integration enabled:
- DM entry notification
- Reply with "trust" to grant access
- Immediate effect

## Tips

1. **Trust carefully** - Full access when online
2. **Check list regularly** - Remove inactive players
3. **Use for friends** - Helpful for building
4. **Don't over-trust** - Can edit your base
