# VIA Custom Layout - RGB Knob

This is a custom layout based on the default configuration with modified rotary encoder behavior for better backlight control.

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

## Changes from Default

### Rotary Encoder 2 (Top Right)
- **Layer 0:** Changed from RGB brightness to **Backlight Brightness** control
- **Layer 1:** Maintained RGB mode cycling

### Layer 0 (Default)

| Cell | Function |
| --- | --- |
| `Key 1` | `Page Up` |
| `Key 2` | `Page Down` |
| `Key 3` | `F1` |
| `Key 4` | `F2` |
| `Key 5` | `F3` |
| `Key 6` | `F4` |
| `Key 7` | `F5` |
| `Key 8` | `F6` |

### Layer 1

| Cell | Function |
| --- | --- |
| `Key 1` |  |
| `Key 2` |  |
| `Key 3` |  |
| `Key 4` |  |
| `Key 5` |  |
| `Key 6` |  |
| `Key 7` |  |
| `Key 8` | `Off RGB / Device` |

## Encoders

| Control | Layer 0 | Layer 1 |
| --- | --- | --- |
| `Knob 1 rotate` | `Volume Up / Down` | `KC_MPRV / KC_MNXT` |
| `Knob 1 press` | `Mute` | `—` |
| `Knob 2 rotate` | `Backlight Brightness Up / Down` | `RGB mode cycle` |
| `Knob 2 press/hold` | `Enable next layer` | `—` |

## Macros

| Macro | Command | What it does |
| --- | --- | --- |
| `M0` | Unused | Unused |
| `M1` | Unused | Unused |
| `M2` | Unused | Unused |
| `M3` | Unused | Unused |
| `M4` | Unused | Unused |
| `M5` | Unused | Unused |
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

## Physical Layout

Same
