# Combat Protection

**PvP rules within protected bases**

## Overview

Combat protection prevents untrusted players from attacking base owners first.

## How It Works

1. **Untrusted user enters** → Cannot attack first
2. **Owner attacks them** → 30s retaliation window
3. **Window expires** → Protection resets

## Settings

| Setting | Value |
|---------|-------|
| Retaliation window | 30 seconds |
| Protect trusted | No |
| Reset delay | 10 seconds |

## Combat Integration

### CMI Combat Tags
If CMI is available, uses CMI combat detection.

### Custom Combat (Fallback)
- Duration: 15 seconds
- Triggers: PvP damage, projectile hits
- Boss bar shows combat status

## Combat Messages

- Tag starts: "⚔ You are now in combat!"
- Tag ends: "✓ You are no longer in combat."
- Blocked attack: "Cannot attack first in this base!"

## Tips

1. **Attack first** - Establishes PvP rights
2. **30 seconds** - Retaliation window
3. **Stay close** - Protection resets if you leave
