This checklist covers device testing for major Android version updates, QPR updates, or full device validation.

**How to use this template:**
- Work through each section systematically, checking off items as you test
- Add additional test steps as needed based on your specific hardware (e.g., stylus support, folding mechanisms, etc.)
- For any issues or bugs found, comment them directly under this issue with relevant logs
- Mark items as N/A if not applicable to your device (for example, no NFC or fast charging)
- Document any device-specific quirks or workarounds in the "Known Issues + Notes" section

TODO: 
- Apps linked or inline: Seedvault, MicroG, Chromium, Firewall, Glimpse
- System:  Multi-user, VPN
- System functions: file sharing, picking, 

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
- [ ] No bootloop
- [ ] Boot time reasonable
- [ ] Recovery accessible
- [ ] Fastboot/bootloader accessible
- [ ] Recovery version correct
- [ ] CalyxOS boot animation as expected
- Setup Wizard
  - [ ] Boots to SuW
  - [ ] CalyxOS icon in SuW
  - [ ] Can install apps on Apps page
  - [ ] microG Google Services compatibility is on by default
  - [ ] microG Push Notification Support is on by default
  - [ ] microG Network Location is on and by default and selections are working
  - [ ] You can install apps in one click at the end of SuW, the app list doesn't include CalyxVPN
  - [ ] SuW completes without errors

## For battery tracking (once booted)
Current battery level:
UTC Time:

## Display + Navigation
- [ ] Brightness manual adjustment
- [ ] Auto-brightness
- [ ] Auto-rotate screen
- [ ] Refresh rate, 60 standard (120 Smooth Display enabled*)
- [ ] No flickering or other visual problems
- [ ] Caffeine (Quick settings tile)
- [ ] Screen timeout (Settings > Display)
-  Lock screen
  - [ ] Lock screen privacy: all, none, sensative content when unlocked
  - [ ] Scramble lock screen PIN (Settings > Security & Privacy > Device Unlock > Screen lock (PIN) Gear)
- Launcher, navigation, and app switcher
  - [ ] 3-button navigation: back, home, overview
  - [ ] Gesture navigation: all gestures work (just try each a few times)
  - [ ] Search for apps
- Home screen:
  - [ ] Add/remove apps
  - [ ] Add/remove widgets
  - [ ] Change wallpaper
  
## Cellular
- [ ] SIM card detected
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
- [ ] Redact location when sharing (Settings > Security & Privacy > More security & privacy)
  - Upload location-tagged photo to share.riseup.net, download it, make sure no location

## Sensors & Biometrics
- [ ] Fingerprint scanner (add fingerprint, unlock lock screen)
- [ ] Accelerometer
- [ ] Gyroscope
- [ ] Proximity sensor

## Location
- [ ] Location (on/off)
- [ ] Maps navigation, tiles
- [ ] Location accuracy acceptable

## Firewall
- [ ] App-specific: allow background network access
- [ ] App-specific: allow Wi-Fi data
- [ ] App-specific: allow mobile data
- [ ] App-specific: allow VPN data

## Notification
- [ ] At restart, system notification showing the last notification with the community letter
- [ ] Use notification history is turned off by default in Notification Setting

## Backup and restore
- [ ] Can set up a Backup (Seedvault) 

## Apps
- [ ] Can install an app from Aurora store
- [ ] Can install an app from F-Droid

## Performance
- [ ] No significant lag in the UI
- [ ] Apps are responsive at launch
- [ ] Multitasking smooth, switching between apps is quick
- [ ] No random freezes
- [ ] No excessive heating during normal use
- [ ] Battery drain baseline (note screen-on time)
- [ ] Standby drain acceptable (< 2-3%/hr)
- [ ] Fast charging

## Work profile
  - [ ] Set up Work profile (via system app "Work Profile")
  - Turn on the cross-profile sharing settings in Work Profile Settings (Settings > Passwords & accounts > Work tab)
    - [ ] Copy a file *to* a work profile
    - [ ] Copy a file *from* a work profile
    - [ ] Share a file *to* a work profile
    - [ ] Share a file *from* a work profile

- Items ending with * are not supported on all CalyxOS devices or regions
