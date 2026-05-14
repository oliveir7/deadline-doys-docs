# VIA Layout - AMD PC

This document describes the key mappings and layers for the "AMD PC" VIA configuration for the DoysPad.

See [Layout Guide](../../LAYOUT-GUIDE.md) for the shared documentation structure.

## Reference Diagram

Encoder 1 and Encoder 2 are the rotary encoders.

```text
┌────────┬────────┬───────┬───────┐
│ Knob 1 │        │ Key 1 │ Key 2 │
├────────┼────────┼───────┼───────┤
│ Knob 2 │ Key 3  │ Key 4 │ Key 5 │
├────────┼────────┼───────┼───────┤
│        │ Key 6  │ Key 7 │ Key 8 │
└────────┴────────┴───────┴───────┘
```

## Layer 0 (Default)

| Cell | Function |
| --- | --- |
| `Key 1` | `KC_MYCM` (open my computer) |
| `Key 2` | `KC_WWW_SEARCH` (open search) |
| `Key 3` | `M0` (Take screenshot) |
| `Key 4` | `M1` (Record instant replay) |
| `Key 5` | `M2` (Toggle recording) |
| `Key 6` | `M3` (Activate 2x frame gen) |
| `Key 7` | `M4` (Toggle overlay) |
| `Key 8` | `M5` (Toggle HDR in Windows 11) |

## Layer 1 (press knob 2)

| Cell | Function |
| --- | --- |
| `Key 1` | `RGB mode prev` |
| `Key 2` | `RGB mode next` |
| `Key 3` | `Bluetooth connection 1` |
| `Key 4` | `Bluetooth connection 2` |
| `Key 5` | `Toggle RGBs` |
| `Key 6` | `Disconnect bluetooth` |
| `Key 7` | `Battery level` |
| `Key 8` | `Change color / hue +` |

## Encoders

| Control | Layer 0 | Layer 1 |
| --- | --- | --- |
| `Knob 1 rotate` | `KC_VOLU / KC_VOLD` | `RGB_VAI / RGB_VAD` |
| `Knob 1 press` | `Mute` | `—` |
| `Knob 2 rotate` | `RGB_VAD / RGB_VAI` | `RGB_MOD / RGB_RMOD` |
| `Knob 2 press/hold` | `Enable next layer` | `—` |

## Macros

| Macro | Command | What it does |
| --- | --- | --- |
| `M0` | `Ctrl+Shift+I` | Take screenshot |
| `M1` | `Ctrl+Shift+E` | Record instant replay |
| `M2` | `Ctrl+Shift+S` | Toggle recording |
| `M3` | `Alt+Shift+G` | Activate 2x frame gen |
| `M4` | `Ctrl+Shift+O` | Toggle overlay |
| `M5` | `Win+Alt+B` | Toggle HDR in Windows 11 |
| `M6` | Unused | Unused |
| `M7` | `Ctrl+Shift+Win+B` | Resets the graphics driver when the display glitches mid-session |
| `M8` | `Win+Ctrl+V` | Opens the per-app volume mixer |
| `M9` | `Win+Alt+T` | Opens a lightweight native performance overlay |
| `M10` | Unused | Unused |
| `M11` | Unused | Unused |
| `M12` | Unused | Unused |
| `M13` | Unused | Unused |
| `M14` | Unused | Unused |
| `M15` | Unused | Unused |
