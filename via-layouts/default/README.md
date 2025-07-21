## Default Layer (Layer 0)

### Keys
| Position | Key | Function |
|----------|-----|----------|
| Key 1 | Page Up | Scroll up/previous page |
| Key 2 | Delete | Delete key |
| Key 3 | Page Down | Scroll down/next page |
| Key 4 | Mute | Audio mute toggle |
| Key 5 | F1 | Function key F1 |
| Key 6 | F2 | Function key F2 |
| Key 7 | F3 | Function key F3 |
| Key 8 | MO(1) | **Hold to access Layer 1** |
| Key 9 | F4 | Function key F4 |
| Key 10 | F5 | Function key F5 |
| Key 11 | F6 | Function key F6 |

### Rotary Encoders
| Encoder | Turn Left | Turn Right |
|---------|-----------|------------|
| Encoder 1 (Top Left) | Volume Down | Volume Up |
| Encoder 2 (Top Right) | RGB Brightness Down | RGB Brightness Up |

## Function Layer (Layer 1)
*Access by holding Key 8 (MO(1))*

### Keys
| Position | Key | Function |
|----------|-----|----------|
| Key 1 | - | Same as Layer 0 (Page Up) |
| Key 2 | - | Same as Layer 0 (Delete) |
| Key 3 | - | Same as Layer 0 (Page Down) |
| Key 4 | Toggle TOP RGB | Toggle top RGB lighting |
| Key 5 | BLE Channel 1 | Switch to Bluetooth Channel 1 |
| Key 6 | BLE Channel 2 | Switch to Bluetooth Channel 2 |
| Key 7 | USB Toggle | Toggle USB output |
| Key 8 | MO(1) | **Function layer key (hold)** |
| Key 9 | BLE Disconnect | Disconnect Bluetooth |
| Key 10 | Battery Level | Show battery level indicator |
| Key 11 | RGB Toggle | Toggle RGB lighting on/off |

### Rotary Encoders (Layer 1)
| Encoder | Turn Left | Turn Right |
|---------|-----------|------------|
| Encoder 1 (Top Left) | Media Previous | Media Next |
| Encoder 2 (Top Right) | RGB Mode Previous | RGB Mode Next |

## Special Key Combinations

### System Controls
- **Power Off:** Hold bottom encoder + press Key 9 (bottom right)
- **Backlight Toggle:** Hold Encoder 2 + press Key 11 (when connected via USB)
- **Bluetooth Off:** Hold Encoder 2 + press Key 10

### Reset Procedure
- **Hard Reset:** Remove battery → Hold reset button → Insert USB → Wait → Reinsert battery

## Notes

- **Layer 0** is the default layer for everyday use
- **Layer 1** contains advanced functions and connectivity controls
- **MO(1)** means "Momentary Layer 1" - hold Key 8 to temporarily access Layer 1
- **KC_TRNS** means the key is transparent and uses the same function as Layer 0
- Layers 2 and 3 are empty by default and available for custom programming

## Customization

This layout can be modified using VIA software. To customize:
1. Load the `info-via-DoysPadBle.json` file in VIA
2. Connect your device
3. Modify any key assignments as needed
4. Changes are saved automatically to the device

---

*This layout represents the factory default configuration. Your device may have different mappings if previously customized.*