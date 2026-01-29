# Feature Chart Formatting Rules

This document outlines the formatting rules for Pro Tools feature chart files when integrating HUI protocol information.

## Purpose

These rules ensure that feature charts contain relevant information for V-Control Pro users while removing hardware-specific references to Mackie HUI control surfaces that don't apply to software-based control.

## Rules

### 1. Replace "V-POT" with "Knob"
- Use consistent terminology "Knob" instead of "V-POT" throughout all feature charts
- "V-POT" refers to Mackie hardware nomenclature

### 2. Double-click Actions in Modifier Column
- Place "Double-click" and "Multiple double-clicks" in the modifier column
- Format: `| | Double-click | Description |`
- Do NOT format as inline text like "Double-click: description"

### 3. Remove Hardware Display References
- Remove any references to displaying text on hardware displays
- Examples to remove:
  - `(displays "Pan")`
  - `scribble displays "FLIP"`
  - `Displays current input source on all channel scribble strips`
  - Any mention of "scribble strips" showing information

### 4. Keep Functional LED Status
- KEEP LED status indicators when they show functional state
- Examples to keep:
  - `LED lights when enabled`
  - `LED flashes when record-ready`
  - `LED lit when recording`
  - `AUTO LED green` (indicates automation read mode)
  - `AUTO LED red flashing/lit` (indicates automation write modes)
- These indicate operational status, not hardware-specific displays

### 5. Remove Footswitch References
- Remove all references to footswitch operations
- Examples: `Footswitch #1`, `Footswitch #2`, `Shift+Footswitch #1`
- Footswitches are Mackie HUI hardware accessories not applicable to V-Control Pro

### 6. Remove Keypad Number References
- Remove all numeric keypad shortcut references from Mackie HUI surfaces
- Examples to remove:
  - `Edit Mode+1`, `Edit Tool+3`, etc.
  - `Option+number` (for zoom presets)
  - `Shift+number` (for storing zoom presets)
  - `Ctrl+number` (for shuttle lock mode)
- Numeric keypads are Mackie HUI hardware features
- **EXCEPTION:** ProControl has its own physical keypad section - KEEP all "Keypad Buttons" sections for procontrol-protools.md

## Table Format

All feature chart tables should use the 3-column format:

```markdown
| Button/Control | Modifier | Description |
|---|---|---|
| `Button` |  | Default function description. |
|  | `Shift`+ | Modified function description. |
|  | `Option`+ | Another modified function description. |
|  | Double-click | Double-click function description. |
```

## Application Order

1. Apply these rules to c24-protools.md as the reference implementation
2. After c24-protools.md is complete, apply to remaining Pro Tools feature charts:
   - command8-protools.md
   - control24-protools.md
   - dcommand-protools.md
   - faderport-8-16-protools-2023.md
   - faderport-v2-protools.md
   - procontrol-protools.md

## Source Materials

- HUI protocol information: `/Users/pneyrinck/Code/docs-vcpro/hui/HUI-Button-Functions-Complete.txt`
- Feature chart files: `/Users/pneyrinck/Code/docs-vcpro/docs/feature-chart/*-protools.md`
