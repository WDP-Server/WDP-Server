# Permissions

**Complete permission reference for WDP plugins**

## Permission System

Permissions managed by **LuckPerms**.

## Default Permissions

All players receive:

### WDP-BaseDet
| Permission | Description | Default |
|------------|-------------|---------|
| `basedet.user.menu` | Open base menu | true |
| `basedet.user.confirm` | Confirm detected base | true |
| `basedet.user.deny` | Deny detection | true |
| `basedet.user.view` | View base boundaries | true |
| `basedet.user.detect` | Manually trigger detection | true |
| `basedet.user.score` | View detection score | true |
| `basedet.user.tool` | Use selector tool | true |
| `basedet.user.expand` | Confirm/deny expansion | true |
| `basedet.user.help` | View help | true |
| `basedet.user.trust` | Trust players | true |

### WDP-Start
| Permission | Description | Default |
|------------|-------------|---------|
| `wdpstart.command.start` | Use /start command | true |
| `wdpstart.command.help` | Get help | true |
| `wdpstart.menu` | Open quest menu | true |

### WDP-Quest
| Permission | Description | Default |
|------------|-------------|---------|
| `quest.user.menu` | Open quest menu | true |
| `quest.user.commands` | Use quest commands | true |
| `quest.user.abandon` | Abandon quests | true |

### WDP-Progress
| Permission | Description | Default |
|------------|-------------|---------|
| `progress.user.view` | View progress | true |
| `progress.user.menu` | Open progress menu | true |

### WDP-Help
| Permission | Description | Default |
|------------|-------------|---------|
| `help.user.command` | Use /help command | true |

### AuraSkills
| Permission | Description | Default |
|------------|-------------|---------|
| `auraskills.command.shop` | Open shop | true |
| `auraskills.command.skills` | Open skills menu | true |
| `auraskills.command.skillcoins` | Coin commands | true |
| `auraskills.command.balance` | Check balance | true |

## Admin Permissions

### WDP-BaseDet
| Permission | Description | Default |
|------------|-------------|---------|
| `basedet.admin.*` | All admin permissions | op |
| `basedet.admin.reload` | Reload config | op |
| `basedet.admin.debug` | Toggle debug mode | op |
| `basedet.admin.bypass` | Bypass protection | op |
| `basedet.admin.view` | View any base | op |
| `basedet.admin.force` | Force detection | op |
| `basedet.admin.delete` | Delete bases | op |
| `basedet.admin.list` | List all bases | op |

### WDP-Start
| Permission | Description | Default |
|------------|-------------|---------|
| `wdpstart.admin.*` | All admin permissions | op |
| `wdpstart.admin.reload` | Reload config | op |
| `wdpstart.admin.cancel` | Cancel player quests | op |
| `wdpstart.admin.give` | Give rewards | op |

### WDP-Quest
| Permission | Description | Default |
|------------|-------------|---------|
| `quest.admin.*` | All admin permissions | op |
| `quest.admin.reload` | Reload config | op |
| `quest.admin.give` | Give quests | op |
| `quest.admin.complete` | Complete quests | op |
| `quest.admin.reset` | Reset player quests | op |

### WDP-Progress
| Permission | Description | Default |
|------------|-------------|---------|
| `progress.admin.*` | All admin permissions | op |
| `progress.admin.reload` | Reload config | op |
| `progress.admin.modify` | Modify progress | op |
| `progress.admin.reset` | Reset progress | op |

### WDP-Help
| Permission | Description | Default |
|------------|-------------|---------|
| `help.admin.*` | All admin permissions | op |
| `help.admin.reload` | Reload config | op |
| `help.admin.stats` | View stats | op |

### AuraSkills/SkillCoins
| Permission | Description | Default |
|------------|-------------|---------|
| `auraskills.admin` | All admin permissions | op |
| `auraskills.command.skillcoins.give` | Give coins | op |
| `auraskills.command.skillcoins.take` | Take coins | op |
| `auraskills.command.skillcoins.set` | Set balance | op |
| `auraskills.command.skillcoins.check` | Check balance | op |
| `economy.admin` | Economy admin | op |

## Permission Groups

### Default (New Players)
```
basedet.user.*
wdpstart.command.*
quest.user.*
progress.user.*
help.user.*
auraskills.command.shop
auraskills.command.skills
```

### Member (Active Players)
(Inherits Default)
Plus all trust permissions

### VIP (Donor)
(Inherits Member)
Additional shop discounts
Extra daily quests

### Moderator
(Inherits VIP)
```
basedet.admin.view
quest.admin.reload
progress.admin.view
```

### Admin
(Inherits Moderator)
```
basedet.admin.*
wdpstart.admin.*
quest.admin.*
progress.admin.*
help.admin.*
auraskills.admin
```

## Common Tasks

### Grant Permission
```bash
/lp user <player> permission set <permission>
```

### Check Permissions
```bash
/lp user <player> permission check <permission>
```

## PlaceholderAPI

```
%has_permission_<permission>%  # Returns "true" or ""
```
