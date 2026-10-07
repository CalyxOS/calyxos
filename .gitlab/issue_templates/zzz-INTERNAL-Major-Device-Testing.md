This checklist covers device testing for major Android version updates, QPR updates, or full device validation for a clean CalyxOS install.

**How to use this template:**
- Work through each section systematically, checking off items as you test
- Add additional test steps as needed based on your specific hardware
- For any issues or bugs found, comment them directly under this issue with relevant logs or screenshots
- Mark items as N/A if not applicable to your device (for example, no NFC or fast charging)
- Document any device-specific quirks or workarounds in the "Known Issues + Notes" section

TODO:
- Full device validation from existing CalyxOS install.

---

## Device information
Device:
Device codename:
Major Android version, including QPR:
CalyxOS version:
Security patch level:
Kernel version:
[ ] Build is signed with CalyxOS production keys

## Boot & System
- [ ] No bootloop
- [ ] Boot time reasonable
- [ ] Recovery accessible
- [ ] Fastboot/bootloader accessible
- [ ] CalyxOS boot animation and logo as expected

## Verify the build
- [ ] Verify the build information in Settings > About phone matches details above
- [ ] CalyxOS version correct
- [ ] Security patch level correct
- [ ] Kernel version correct

## For battery tracking (once booted and enabled)
Current battery level:
UTC Time:

## Display + Navigation
- [ ] Brightness level manual adjustment
- [ ] Adaptive/auto-brightness
- [ ] Refresh rate, 60 standard (120 Smooth Display enabled*)
- [ ] No flickering or other visual problems

## Cellular
- [ ] SIM card (or eSIM) detected
- [ ] Mobile Data
  - Network strength:
  - Speedtest:
- Private Dialer
  - [ ] Call (make, receive)
- [ ] VoLTE*
- [ ] Text Messages / SMS (send, receive)
- [ ] MMS (send, receive)
- [ ] Wifi calling (if carrier supports)*
- [ ] Emergency calls
  - No need to call, just test Dialpad accepts input from Lockscreen > Emergency

## Wi-Fi
- [ ] Wi-Fi on/off
  - Speedtest:
- [ ] Wi-Fi Hotspot
  - Speedtest:
- [ ] Wi-Fi MAC randomization (MAC address for Wi-Fi network must not match Settings -> About this phone -> Device Wi-Fi MAC address)

## Bluetooth
- [ ] Bluetooth on/off
- [ ] Pairing with a device
- [ ] Successful reconnection with paired device
- [ ] File transfer
- [ ] Tethering

## NFC + USB
- [ ] NFC on/off
- [ ] USB file transfer to computer
- [ ] USB data tethering to computer
- [ ] USB restrictions: charge only on first boot, after first boot when locked

## Audio
- [ ] Device sounds (ringtones, notifications)
- [ ] Device vibration
- [ ] Speaker playback
- [ ] Earpiece (during calls)
- [ ] Headphone jack*
- [ ] Bluetooth audio, both calls and media playback
- [ ] Microphone access on/off
- [ ] System microphone (test with recording)

## Camera
- [ ] Camera access on/off
- [ ] Camera photo, front/back
- [ ] Camera video, front/back
- [ ] Zoom in/out
- [ ] Flash

## Sensors & Biometrics
- [ ] Fingerprint scanner (add fingerprint, unlock lock screen)
- [ ] Accelerometer
- [ ] Gyroscope
- [ ] Proximity sensor

## Location
- [ ] Location (on/off)
- [ ] Maps navigation, tiles
- [ ] Location accuracy acceptable
- [ ] Assisted GPS is enabled by default (Settings > Location)

## Performance
- [ ] No significant lag in the UI
- [ ] Apps are responsive at launch
- [ ] Multitasking smooth, switching between apps is quick
- [ ] No random freezes
- [ ] No excessive heating during normal use
- [ ] Battery drain acceptable (note screen-on time)
- [ ] Standby drain acceptable (< 2-3%/hr)
- [ ] Battery charging control: limit, schedule (Setting > Charging control > Charging mode)
- [ ] Fast charging
