# VIA Layout - Nvidia PC

This document describes the key mappings and layers for the "Nvidia PC" VIA configuration for the DoysPad.

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
| `Key 3` | `M2` (Take screenshot) |
| `Key 4` | `M1` (Record instant replay) |
| `Key 5` | `M3` (Toggle instant replay) |
| `Key 6` | `M0` (Open filters (RTX HDR)) |
| `Key 7` | `Toggle performance stats` |
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
| `M0` | `Alt+F3` | Open filters (RTX HDR) |
| `M1` | `Alt+F10` | Record instant replay |
| `M2` | `Alt+F1` | Take screenshot |
| `M3` | `Alt+Shift+F10` | Toggle instant replay |
| `M4` | `Alt+R` | Toggle recording |
| `M5` | `Win+Alt+B` | Toggle HDR in Windows 11 |
| `M6` | Unused | Unused |
| `M7` | Unused | Unused |
| `M8` | Unused | Unused |
| `M9` | Unused | Unused |
| `M10` | Unused | Unused |
| `M11` | Unused | Unused |
| `M12` | Unused | Unused |
| `M13` | Unused | Unused |
| `M14` | Unused | Unused |
| `M15` | Unused | Unused |
