This checklist covers device testing for major Android version updates, QPR updates, or full device validation for a clean CalyxOS install.

**How to use this template:**
- Work through each section systematically, checking off items as you test
- Add additional test steps as needed based on your specific hardware
- For any issues or bugs found, comment them directly under this issue with relevant logs or screenshots
- Mark items as N/A if not applicable to your device (for example, no NFC or fast charging)
- Document any device-specific quirks or workarounds in the "Known Issues + Notes" section

TODO:
- Full device validation from existing CalyxOS install.
- Apps linked or inline: Seedvault (independent template), MicroG, Chromium, F-Droid apps included OOB.
- System: Multi-user, VPN
- System functions: file sharing, picking, opening a file

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
- Setup Wizard
  - [ ] Boots to SuW
  - [ ] Can install apps on Apps page
  - [ ] microG Google Services compatibility is on by default
  - [ ] microG Push Notification Support is on by default
  - [ ] microG Network Location is on and by default and selections are working
  - [ ] You can install apps in one click at the end of SuW
  - [ ] SuW completes without errors

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
- [ ] Auto-rotate screen
- [ ] Refresh rate, 60 standard (120 Smooth Display enabled*)
- [ ] Caffeine (Quick settings tile)
- [ ] Screen timeout (Settings > Display)
- [ ] No flickering or other visual problems
- Lock screen
  - [ ] Lock screen privacy: all, none, sensitive content when unlocked
  - [ ] Scramble lock screen PIN (Settings > Security & Privacy > Device Unlock > Screen lock (PIN) Gear)
- Launcher, navigation, and app switcher
  - [ ] 3-button navigation: back, home, overview
  - [ ] Gesture navigation: all gestures work (just try each a few times)
  - [ ] Search for apps
  - [ ] Pause app
- Home screen:
  - [ ] Add/remove apps
  - [ ] Add/remove widgets
  - [ ] Change wallpaper

## Cellular
- [ ] SIM card (or eSIM) detected
- [ ] Mobile Data
  - Network strength:
  - Speedtest:
- Private Dialer
  - [ ] Call (make, receive)
  - Helplines
    - [ ] Helplines are present
    - [ ] Dialed helpline does not appear in call logs
    - [ ] Regular calls are indicated as "not private" (yellow banner)
    - [ ] Signal is suggested
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
- [ ] Wi-Fi MAC non-persistent randomization (Settings > System > Other options)

## Bluetooth
- [ ] Bluetooth on/off
- [ ] Bluetooth timeout
- [ ] Pairing with a device for the first time
- [ ] Successful repairing with known device
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
- [ ] Microphone timeout

## Camera
- [ ] Camera photo, front/back
- [ ] Camera video, front/back
- [ ] Camera QR scan
- [ ] Zoom in/out
- [ ] Flash
- [ ] Camera access on/off
- [ ] Camera timeout
- [ ] Redact location when sharing (Settings > Security & Privacy > More security & privacy)

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

## Firewall
- [ ] App-specific: allow background network access
- [ ] App-specific: allow Wi-Fi data
- [ ] App-specific: allow mobile data
- [ ] App-specific: allow VPN data
- [ ] Network access is off for newly installed apps when enabled (Firewall > Settings)

## Notification
- [ ] Use notification history is turned off by default (Settings > Notification)

## Apps
- [ ] Can install an app from Aurora Store
- [ ] Can install an app from F-Droid

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

## Work profile
  - [ ] Set up Work profile (via system app "Work Profile")
  - Cross-profile sharing for Work Profile Settings (Settings > Passwords & accounts > Work tab)
    - [ ] Copy a file *to* a work profile
    - [ ] Copy a file *from* a work profile
    - [ ] Share a file *to* a work profile
    - [ ] Share a file *from* a work profile

## Private space
- [ ] Set up private space (Settings > Security & Privacy > Private space)
