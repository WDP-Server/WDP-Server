# Navbar System

**Consistent bottom menu across all WDP plugins**

## Layout

```
┌─────────────────────────────────────────────────────────────────┐
│  45   │ 46 │ 47 │ 48      │ 49      │ 50      │ 51 │ 52 │ 53   │
├─────────────────────────────────────────────────────────────────┤
│Balance│ ■  │ ■  │   ← Prev│  Page   │  Next → │ ■  │ ■  │Back/ ✕│
└─────────────────────────────────────────────────────────────────┘
```

## Slot Details

| Slot | Item | Purpose |
|------|------|---------|
| 45 | Gold Nugget | Balance display |
| 46-47 | Black Glass | Filler |
| 48 | Arrow | Previous page |
| 49 | Paper/Clock | Page info / Progress |
| 50 | Arrow | Next page |
| 51-52 | Black Glass | Filler |
| 53 | Spyglass/Barrier | Back / Close |

## Balance Display (Slot 45)

```
Material: gold_nugget
Display: "§6Balance:"
Lore:
  - "⛃: {coins}"
  - "🎟: {tokens}"
```

## Page Navigation (Slots 48-50)

### Previous (Slot 48)
```
Material: Arrow
Display: "§e§l← Previous"
```

### Page Info (Slot 49)
```
Material: Paper
Display: "§e§lPage §f§l{page} §8/ §f§l{total_pages}"
```

### Next (Slot 50)
```
Material: Arrow
Display: "§e§lNext →"
```

## Back/Close (Slot 53)

### Back (Has Previous Menu)
```
Material: Spyglass
Display: "§c§l← Back"
```

### Close (No Previous Menu)
```
Material: Barrier
Display: "§c§l✗ Close"
```

## Special Cases

### WDP-Start (Quest Progress)
```
Slot 49 - Clock:
Display: "§e§lQuest Progress"
Lore:
  - "Completed: {completed}/{total}"
  - "{progress_bar}"
  - "Current: {quest_name}"
```

### WDP-Progress (No Balance)
```
Slots: 46-53 (no slot 45)
Simple navbar with Back/Close
```

## Exceptions

### Menus Without Balance
- Welcome screen
- Confirmation dialogs

### Menus With Only Back
- Skills list
- Ability menu
- Stats view

## Configuration

```yaml
navbar:
  balance:
    slot: 45
    material: gold_nugget
  glass_fill:
    slots: [46, 47, 51, 52]
    material: black_stained_glass_pane
  previous_page:
    slot: 48
    material: arrow
  page_info:
    slot: 49
    material: paper
  next_page:
    slot: 50
    material: arrow
  back:
    slot: 53
    material: spyglass
  close:
    slot: 53
    material: barrier

exceptions:
  no_balance:
    - welcome
    - confirmation
```
