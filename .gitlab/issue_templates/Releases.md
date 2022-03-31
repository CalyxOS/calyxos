|  |  |
| ------ | ------ |
| Android version |  |
| Security patch |  |
| CalyxOS version |  | 
| Build number | ** ** | 
| Previous build number |  |
| `otatest` build number |  | 
| `otatest2` build number |  | 

Notes:

Devices:
* [ ] raven | Pixel 6 Pro
* [ ] oriole | Pixel 6
* [ ] barbet | Pixel 5a
* [ ] bramble | Pixel 4a (5G)
* [ ] redfin | Pixel 5
* [ ] sunfish | Pixel 4a
* [ ] coral | Pixel 4 XL
* [ ] flame | Pixel 4
* [ ] bonito | Pixel 3a XL
* [ ] sargo | Pixel 3a
* [ ] crosshatch | Pixel 3 XL
* [ ] blueline | Pixel 3
* [ ] taimen | Pixel 2 XL
* [ ] walleye | Pixel 2
* [ ] jasmine_sprout | Mi A2
* [ ] FP4 | Fairphone 4
* [ ] kebab | OnePlus 8T
* [ ] lemonade | OnePlus 9

Checklist:
* [ ] Tag kernel
* [ ] Build, boot, merge kernel
* [ ] Tag release
* [ ] Build from tag
* [ ] Push metadata to 'release' repo
* [ ] Write changelog
* [ ] Sign release
* [ ] Make sure device is running "Previous build" and that the bootloader is locked.
* [ ] Install OTA, **-testing** - incremental should mean quick download
* [ ] Run through SetupWizard, check with microG enabled/disabled and select all/some/no F-Droid apps on different devices
* [ ] Test restoring a backup from USB
* [ ] Verify the build information in Settings -> About. It should match the details above.
* [ ] Verify any new features / bugfixes, refer to the changelog for details.
* [ ] Wi-Fi (network strength when close to router, speedtest)
* [ ] Mobile Data ()
* [ ] Bluetooth (On, Pairing, audio)
* [ ] Calls (Normal, VoLTE)
* [ ] Text Messages / SMS
* [ ] eSIM
* [ ] Location (GPSTest, Maps)
* [ ] Camera (Still images, video, front and back)
* [ ] Flashlight / torch
* [ ] Sensors
* [ ] Hotspot
* [ ] Fingerprint scanner
* [ ] Face unlock
* [ ] Device sounds
* [ ] CalyxVPN
* [ ] F-Droid
* [ ] Verify microG configuration if enabled (microG Settings -> Self Check)
* [ ] Final step, test OTA updates from this build to a newer build, **-otatest** - this will be a full OTA, big download
* [ ] Verify the build information in Settings -> About. It should match the details above.
* [ ] Optionaly, test the completely new test build, **-otatest2** - this will be a full OTA, big download
* [ ] Verify the build information in Settings -> About. It should match the details above.
* [ ] Update 'releases' repo
* [ ] Push changelog to 'release' repo
* [ ] Move to **-beta3**
* [ ] Move to **-stable3**
* [ ] Update website links
* [ ] Update 0xacab mirrors

/label ~Releases
