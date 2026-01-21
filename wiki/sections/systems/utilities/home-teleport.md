# Home & Teleport System

**Personal waypoints and fast travel**

## Setting Homes

### /sethome

```
/sethome <name>
```

**Requirements:**
- Safe location (not falling, not in lava)
- Not in protected base
- Unique name (1-16 characters)
- No special characters except underscores

**Example:**
```
/sethome mainbase
/sethome mine
/sethome nether-base
```

### Home Limits

| Status | Max Homes |
|--------|-----------|
| Default | 3 |
| VIP | 5 |
| Premium | 10 |

## Teleporting Home

### /home

```
/home <name>
/home        # Open menu
/home list   # List all homes
```

**Process:**
1. Enter command
2. 3 second countdown
3. Teleport executes
4. Arrival message

**Cancels if:**
- Move > 5 blocks
- Take damage
- Enter vehicle

## Home Menu

```
┌─────────────────────────────────────────────┐
│ 🏠 Homes                    ⛃: 1,234.56   │
├─────────────────────────────────────────────┤
│ [Main Base]  [Forest]  [Mine]               │
│ [Base Two]   [Rename] [Delete]              │
│                                           │
├─────────────────────────────────────────────┤
│ [← Back]                 [Close]            │
└─────────────────────────────────────────────┘
```

**Actions:**
- Click: Teleport
- Shift-click: Delete
- Right-click: Options

## Managing Homes

### Rename

```
/sethome oldname newname
```

Or menu: Shift-click → Rename

### Delete

```
/delhome <name>
```

Or menu: Right-click → Delete

## Random Teleport (RTP)

### /rtp

```
/rtp
/rtp nether
```

**Settings:**
- Min distance: 1,000 blocks
- Max distance: 5,000 blocks
- Safe landing: Yes
- Near trees: 5-30 blocks

### Safe Landing

RTP ensures:
- Solid ground below
- No lava/water
- Head clearance
- Y level 63-200

### Tree Detection

Prioritizes landing near trees:
```
min-distance-from-tree: 5 blocks
max-distance-from-tree: 30 blocks
```

## Warps

### Public Warps

```
/warp <name>
/warplist
```

### Default Warps

| Warp | Location |
|------|----------|
| spawn | Server spawn |
| nether | Nether hub |
| end | End portal |
| farms | Farming area |
| mining | Mining hub |

### Admin Warps

```
/setwarp <name>
/delwarp <name>
```

## TPA System

### Request Teleport

```
/tpa <player>
/tpahere <player>
```

### Accept/Deny

```
/tpaccept
/tpdeny
```

### Toggle Requests

```
/tpatoggle
```

## Back Command

```
/back
```

Returns to:
- Last death location
- Last teleport origin

## Cooldowns

| Command | Cooldown |
|---------|----------|
| /rtp | 60s |
| /home | 30s |
| /base teleport | 300s |
| /tpa | None |

## Costs

| Command | Cost |
|---------|------|
| /rtp | Free |
| /spawn | Free |
| /warp | Free |
| /home | Free |
| /base teleport | 50 ⛃ |

## PlaceholderAPI

| Placeholder | Description |
|-------------|-------------|
| `%homes_count%` | Number of homes |
| `%homes_max%` | Max homes |
| `%homes_remaining%` | Homes remaining |
| `%rtp_cooldown%` | RTP cooldown |
