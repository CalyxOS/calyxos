(This is for internal use only. You probably want a different template)

|  |  |
| ------ | ------ |
| Android version |  |
| Security patch |  |
| CalyxOS version |  |
| Build number | ** ** |
| Previous build number |  |
| `otatest` build number |  |
| `otatest2` build number |  |

Schedule:
| Release channel  | Date   | Notes |
| ---------------- | ------ | ------ |
| Security express |  |  |
| Beta |  |  |
| Stable |  | |

Notes:

Devices:
* [ ] FP5 | Fairphone 5
* [ ] FP4 | Fairphone 4
* [ ] fogo | moto g 5G - 2024
* [ ] bangkk | moto g84 5G
* [ ] fogos | moto g34 5G
* [ ] rhode | moto g52
* [ ] hawao | moto g42
* [ ] devon | moto g32
* [ ] comet | Pixel 9 Pro Fold
* [ ] komodo | Pixel 9 Pro XL
* [ ] caiman | Pixel 9 Pro
* [ ] tokay | Pixel 9
* [ ] akita | Pixel 8a
* [ ] husky | Pixel 8 Pro
* [ ] shiba | Pixel 8
* [ ] felix | Pixel Fold
* [ ] tangorpro | Pixel Tablet
* [ ] lynx | Pixel 7a
* [ ] cheetah | Pixel 7 Pro
* [ ] panther | Pixel 7
* [ ] bluejay | Pixel 6a
* [ ] raven | Pixel 6 Pro
* [ ] oriole | Pixel 6
* [ ] otter | SHIFTphone 8
* [ ] barbet | Pixel 5a
* [ ] bramble | Pixel 4a (5G)
* [ ] redfin | Pixel 5

Checklists:

Before making new production builds:
* [ ] Look at `repo forall -c 'if [ "`git log --oneline $PREV..HEAD`" != "" ]; then git config --get remote.gitlab.projectname; git log --oneline $PREV..HEAD; echo; fi'` to see what changed recently
* [ ] Merge kernel ASB patches
* [ ] Verify SPL and fingerprint
* [ ] Test security fixes when feasible

Tag and make production build:
* [ ] Tag kernel
* [ ] Build, boot, merge kernel
* [ ] Tag release
* [ ] Build from tag
* [ ] Push metadata to 'release' repo
* [ ] Write changelog
* [ ] Draft website (and thus reddit) post
* [ ] Sign release

Test production build before release:
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
* [ ] Device sounds
* [ ] CalyxVPN
* [ ] F-Droid
* [ ] Verify microG configuration if enabled (microG Settings -> Self Check)
* [ ] Final step, test OTA updates from this build to a newer build, **-otatest** - this will be a full OTA, big download
* [ ] Verify the build information in Settings -> About. It should match the details above.
* [ ] Optionaly, test the completely new test build, **-otatest2** - this will be a full OTA, big download
* [ ] Verify the build information in Settings -> About. It should match the details above.

Release:
* [ ] Update 'releases' repo
* [ ] Push changelog to 'release' repo
* [ ] Bump to **-security-express7**
* [ ] Bump to **-beta7**
* [ ] Bump to **-stable7**
* [ ] Bump to **-factory**
* [ ] Update calyxos.org
* [ ] Update calyxos-webinstall
* [ ] Update 0xacab mirrors

(This is for internal use only. You probably want a different template)

/label ~zzz-INTERNAL-release
/assign @cde
