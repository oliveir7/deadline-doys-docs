# Deadline Doys Macro Pad - Known Issues & Troubleshooting

> **Note:** This document compiles known issues reported by the community. Most information comes from user discussions in the Deadline Discord channel.

## Critical Issues

### Rotary Encoder Key Stuck Problem
**Severity:** High - Can brick device until reset

**Issue:** Turning the rotary encoder causes the configured key to be held down continuously, making the device unresponsive.

**Symptoms:**
- Rotary encoder holds down the configured key when turned
- Device becomes completely unresponsive
- No input is accepted until reset
- Requires manual reset to restore functionality

**Current Status:** 
- No known fix available
- Users actively requesting firmware source code from manufacturer for debugging
- This is a critical firmware-level issue

**Workaround:** 
- Perform hard reset procedure (see Troubleshooting section)
- Avoid using rotary encoders with problematic key assignments

---

### Device Stuck in Update/DFU Mode
**Severity:** High - Device non-functional

**Issue:** Device connects only in update/firmware mode instead of normal operation mode.

**Symptoms:**
- USB connection shows device as update/DFU device instead of keyboard
- No backlight or LED indicators
- Bluetooth connection not available
- Device not functional for normal use
- Issue persists across different USB cables
- Shows up with incorrect device name in system

**Current Status:** No known solution available. May require firmware reflashing.

**Attempted Solutions:**
- Hard reset procedure (sometimes unsuccessful)
- Different USB cables
- Different computers
- Battery removal and reinsertion

---

## Hardware Issues

### Quality Control Problems
**Severity:** Medium-High - Affects usability

**Issue:** Some units shipped with significant physical defects.

**Symptoms:**
- Device warped by 1-2mm causing instability
- Severe wobbling when in use
- Poor build quality
- Uneven surfaces

**Solution:** Contact manufacturer for replacement/return.

### Missing Accessories
**Issue:** Some units shipped without expected spare parts.

**Symptoms:**
- Missing additional knobs
- Missing decorative blocks
- Missing keycap sets (depending on purchase timing)

**Solution:** Contact Deadline Studio directly via DM.

### PCB Failure
**Issue:** Complete PCB failure reported by some users.

**Symptoms:**
- Device completely unresponsive
- No power indicators
- Not recognized by any system

**Current Status:** Hardware repair may not be feasible for end users.

---

## Connectivity Issues

### Bluetooth Power Management Problem
**Severity:** Medium - Inconvenient but workaround available

**Issue:** When Bluetooth is manually disabled using key binding, device remains powered on indefinitely.

**Symptoms:**
- Using Bluetooth off binding (BLE_OFF or hold 2nd rotary encoder + bottom left button) disconnects device
- Device stays powered on even when not connected via USB
- Device does not enter sleep/power-off state
- Manual battery removal required to turn off device

**Solution:** Use proper power-off procedure: Hold bottom rotary encoder + press bottom right key (key 8) to turn off the device.

**Alternative:** Remove battery manually to power off the device.

### Bluetooth Connection Failures
**Issue:** Bluetooth fails to connect to devices.

**Symptoms:**
- Cannot establish Bluetooth connection
- Particularly reported on M2/M3 MacBook Pro
- Battery reset doesn't resolve the issue
- Device appears in Bluetooth settings but won't connect

**Solutions:**
1. Follow proper Bluetooth pairing procedure (see main README)
2. Delete old pairings from computer
3. Ensure BLE Channel 1 is properly configured in VIA
4. Keep device close to receiver during pairing

### USB/Bluetooth Recognition Loss
**Issue:** After multiple USB connect/disconnect cycles, device becomes unrecognized.

**Symptoms:**
- Device not detected via USB
- Bluetooth connection fails
- Occurs after repeated USB connections/disconnections
- Particularly reported on Mac systems

**Workaround:** Hard reset procedure may restore functionality.

### Bluetooth Connectivity Instability
**Issue:** Bluetooth connection repeatedly connects and disconnects.

**Symptoms:**
- Device keeps connecting and disconnecting in a loop
- Unstable connection during use

**Solutions:**
1. Delete Bluetooth binding on computer
2. Re-pair device following proper procedure
3. Keep device close to Bluetooth receiver
4. Ensure proper orientation (facing receiver)

---

## Software & Firmware Issues

### VIA Recognition Problems
**Severity:** Medium - Prevents configuration

**Issue:** VIA fails to recognize the device despite successful system connection.

**Symptoms:**
- VIA displays "No compatible devices found"
- Device appears connected via Bluetooth in system settings
- Issue persists with both USB-C and Bluetooth connections
- Affects both online and downloaded versions of VIA
- Reported on macOS 14.5+ with Apple M3 Pro

**Solutions:**
1. Ensure JSON device definition file is properly uploaded in VIA
2. Close interfering USB applications (SignalRGB, etc.)
3. Try refreshing VIA after uploading JSON file
4. Try both USB and Bluetooth connections
5. Follow proper Bluetooth pairing procedure

### VIA Setup Complexity
**Issue:** VIA interface presents significant usability problems.

**Symptoms:**
- Complex and confusing setup process
- Layer management difficulties
- Hard to navigate back to original layer configurations
- Users report having to clone layers as workaround
- Overall "nightmare" setup experience reported

**Solutions:**
1. Join Discord community for setup guidance
2. Plan extra time for configuration
3. Consider backing up layer configurations before making changes
4. Follow community tutorials step-by-step

### JSON File Validation Issues
**Issue:** Device JSON definition file fails validation in QMK online flasher but works in VIA.

**Symptoms:**
- QMK online flasher reports JSON as invalid
- Prevents firmware flashing through QMK tools
- Limits firmware customization options

**Solution:** Use VIA instead - JSON files work properly in VIA after uploading and refreshing.

### USB Application Interference
**Issue:** Other USB applications interfere with VIA device recognition.

**Symptoms:**
- VIA cannot connect to device
- Device appears connected but VIA shows "No compatible devices found"
- Issues with applications like SignalRGB

**Solution:** Close applications that interact with USB devices before using VIA.

### Limited VIA Features
**Issue:** VIA cannot handle advanced features.

**Symptoms:**
- Limited RGB customization options
- Cannot configure per-layer lighting
- Advanced QMK features not accessible through VIA interface

**Current Status:** No workaround available - requires direct QMK access which is unavailable.

---

## Operational Issues

### Media Keys Stop Working After Sleep
**Severity:** Medium - Regular occurrence

**Issue:** Media keys stop functioning after computer goes to sleep.

**Symptoms:**
- Media keys (play/pause, volume, etc.) become unresponsive after computer wakes from sleep
- Regular macros continue to work fine
- Issue occurs reliably after sleep cycles
- Affects productivity workflows

**Workaround:** Replug the device to restore media key functionality.

### Sleep Function Problems
**Issue:** Device sleep behavior is inconsistent.

**Symptoms:**
- Device doesn't properly sleep when idle
- Backlight turns off naturally but device stays powered
- Difficulty waking device after extended idle periods
- Battery drain continues during "sleep"

**Workaround:** Manually power off device using proper key combination.

### USB Toggle Function Unclear
**Issue:** USB Toggle function (CUSTOM(6)) doesn't appear to do anything.

**Symptoms:**
- USB_TOG keycode doesn't produce visible effects
- Function purpose unclear
- No documentation available

**Status:** Community believes it may be for switching between wired/wireless modes, but unconfirmed.

---

## Firmware & Development Limitations

### QMK Compatibility Issues
**Severity:** High for advanced users

**Issue:** Device not recognized by QMK despite VIA compatibility.

**Symptoms:**
- QMK does not recognize the device (other QMK devices like DZ60 work fine)
- Cannot access QMK configurator or flashing tools
- No firmware source code available for debugging
- Limits advanced customization and bug fixes

**Impact:** 
- Cannot fix rotary encoder issues
- Cannot implement advanced features
- Cannot customize beyond VIA limitations

### Firmware Source Code Unavailable
**Issue:** No access to firmware source code for debugging and customization.

**Symptoms:**
- Critical issues cannot be resolved by community
- Advanced features unavailable
- Debugging impossible

**Community Requests:** Users actively requesting firmware source code from manufacturer.

---

## Regional Issues

### Korean Payment Problems
**Issue:** Payment system doesn't work for Korean customers.

**Symptoms:**
- No payment options available when Korea is selected as country
- PayPal and other payment methods not shown
- Cannot complete purchase through normal website

**Solution:** Contact Deadline Studio directly via Discord DM for alternative payment arrangements.

### Shipping and Availability
**Issue:** Limited availability outside group buy periods.

**Symptoms:**
- Device only available during specific group buy windows
- Long wait times for delivery (Q1-Q2 typical)
- Limited vendor options in some regions

**Solutions:**
- Monitor Discord for group buy announcements
- Consider alternative vendors like KeebsForAll (where available)
- Join waitlists when available

---

## Troubleshooting Procedures

### Hard Reset Procedure
For unresponsive devices or recognition issues:

1. **Remove the battery**
2. **Press and hold the reset button**
3. **While holding the button, insert the USB cable**
4. **Wait for a while**
5. **Reinsert the battery**
6. **Device should restore to factory settings**

### Power Management Reset
For power-related issues:

1. **Manual power off:** Hold bottom rotary encoder + press bottom right key (key 8)
2. **If unresponsive:** Remove battery manually
3. **For charging issues:** Try different USB cable and port

### VIA Recognition Reset
For VIA connection issues:

1. **Close all USB-interfering applications** (SignalRGB, etc.)
2. **Upload JSON file** in VIA settings
3. **Refresh VIA** application
4. **Try both USB and Bluetooth** connections
5. **Restart VIA** if necessary

### Bluetooth Pairing Reset
For Bluetooth issues:

1. **Delete all existing pairings** from computer
2. **Remove battery** from device
3. **Follow proper pairing procedure** (see main README)
4. **Keep device close** to receiver during pairing

---

## Reporting New Issues

If you encounter issues not listed here:

1. **Check Discord** for recent discussions
2. **Search existing messages** for similar problems
3. **Document your issue** with:
   - Device symptoms
   - Steps to reproduce
   - System specifications
   - Attempted solutions
4. **Share in Discord** community channel
5. **Include photos/videos** if helpful

## Issue Status Legend

- **High Severity:** Device unusable or major functionality loss
- **Medium Severity:** Significant inconvenience but workarounds available  
- **Low Severity:** Minor issues with minimal impact
- **Current Status:** Community understanding of resolution availability

---

*This document is maintained by the community. Please contribute your findings and solutions to help other users.*

**Last Updated:** Based on Discord discussions through July 2025