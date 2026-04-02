This checklist covers device testing for major Android version updates, QPR updates, or full device validation.

**How to use this template:**
- Work through each section systematically, checking off items as you test
- Add additional test steps as needed based on your specific hardware (e.g., stylus support, folding mechanisms, etc.)
- For any issues or bugs found, comment them directly under this issue with relevant logs
- Mark items as N/A if not applicable to your device (for example, no NFC or fast charging)
- Document any device-specific quirks or workarounds in the "Known Issues + Notes" section

---

## Device information
Device:
Device codename:
Major Android version, including QPR:
CalyxOS version:
Security patch level:
Kernel version:
Build number:
[ ] Build is signed with CalyxOS production keys

## Verify the build
- [ ] Verify the build information in Settings > About phone matches details above
- [ ] CalyxOS version correct
- [ ] Security patch level correct
- [ ] Build fingerprint correct
- [ ] Kernel version matches expected version

## Boot & System
- [ ] Clean flash boots to SuW
- [ ] CalyxOS icon in SuW
- [ ] SuW completes without errors
- [ ] No bootloop
- [ ] Boot time reasonable
- [ ] Recovery accessible
- [ ] Fastboot/bootloader accessible
- [ ] Recovery version correct
- [ ] CalyxOS boot animation as expected

## For battery tracking (once booted)
Current battery level:
UTC Time:

## Cellular
- [ ] SIM card detected
- [ ] Mobile Data
  - Network strength:
  - Speedtest:
- [ ] Call (make, receive)
- [ ] Helplines
- [ ] VoLTE*
- [ ] Text Messages / SMS (send, receive)
- [ ] MMS (send, receive)
- [ ] Wifi calling (if carrier supports)*
- [ ] Emergency calls
  - No need to call, just test Dialpad accepts input from Lockscreen > Emergency

## Wi-Fi
- [ ] Wi-Fi on/off
  - Speedtest:
- [ ] Wi-Fi timeout (Settings > Network & Internet > Internet > Network Preferences)
- [ ] Wi-Fi Hotspot
  - Speedtest:
- [ ] Wi-Fi MAC randomization (Settings > System > Other options)

## Bluetooth
- [ ] Bluetooth on/off
- [ ] Bluetooth timeout
- [ ] Pairing with a device for the first time
- [ ] Successful repairing with known device
- [ ] File transfer
- [ ] Tethering

## NFC + USB
- [ ] NFC
- [ ] USB file transfer to computer
- [ ] USB data tethering to computer

## Display
- [ ] Brightness manual adjustment
- [ ] Auto-brightness
- [ ] Screen timeout
- [ ] Auto-rotate screen
- [ ] Refresh rate, 60 standard (120 Smooth Display enabled*)
- [ ] No flickering or other visual problems

## Audio
- [ ] Device sounds (ringtones, notifications)
- [ ] Device vibration
- [ ] Speaker playback
- [ ] Earpiece (during calls)
- [ ] Headphone jack*
- [ ] Bluetooth audio
- [ ] Microphone access on/off
- [ ] System microphone (test with recording)
- [ ] Microphone timeout

## Camera
- [ ] Camera (photo: front, back)
- [ ] Camera (video: front, back)
- [ ] Zoom in/out
- [ ] Flash
- [ ] Camera access on/off
- [ ] Camera timeout

## Sensors & Biometrics
- [ ] Fingerprint scanner (add fingerprint, unlock lock screen)
- [ ] Accelerometer
- [ ] Gyroscope
- [ ] Proximity sensor

## Location
- [ ] Location (on/off)
- [ ] Maps navigation, tiles
- [ ] Location accuracy acceptable

## Performance
- [ ] No significant lag in the UI
- [ ] Apps are responsive at launch
- [ ] Multitasking smooth, switching between apps is quick
- [ ] No random freezes
- [ ] No excessive heating during normal use
- [ ] Battery drain baseline (note screen-on time)
- [ ] Standby drain acceptable (< 2-3%/hr)
- [ ] Screen timeout at expected time
- [ ] Fast charging
- [ ] Wireless charging (if supported)

## CalyxOS Security + Privacy

## Known Issues + Notes
- Items ending with * are not supported on all CalyxOS devices or regions
