# QtScrcpy - Mirror and Control a Phone You Have Unlocked

![QtScrcpy mirroring an unlocked phone on the Windows desktop](https://korben.info/controler-appareil-android-depuis-pc-mac-avec-qtscrcpy/controler-appareil-android-depuis-pc-mac-avec-qtscrcpy-3.webp)

## Product Snapshot

scrcpy itself is a command-line mirror. QtScrcpy puts the common switches in a window: which device, what resolution, whether to stay on top, whether audio is in this build. Underneath, adb must see the phone and the phone must have accepted this computer. If debugging is off, the device list stays empty and no option in the window fixes that.

The mirror shows what is on the panel. A locked phone shows the lock screen. Typing a password you do not know is not a feature the tool adds. Sit with the owner, unlock, and then mirror.

## What the Window Changes

| Option | Effect |
|---|---|
| Bitrate and size | A smaller picture uses less USB and less CPU |
| Stay awake | The phone does not sleep while you work |
| Full screen or on top | For a recording or a second monitor |
| Device serial | Necessary when two phones are plugged in |
| Record | A file on the PC of what was mirrored, if you enable it |

Start with a modest size. A full-resolution mirror on a slow cable looks like a broken phone. Drop the size, confirm the picture is smooth, then raise it if you need the detail.

## Steps

1. Enable USB debugging and accept the prompt on the unlocked phone.
2. Confirm adb lists the device before you blame QtScrcpy.
3. Open the app and select that serial.
4. Mirror at a moderate size.
5. Click once in the window and confirm the phone responds.
6. Stop the mirror before you unplug, so the recording file can finish.

Wireless adb, if you use it, is still an authorized session on the same network. It is not a scan for other people's phones. Turn it off when the session is over.

## Fits

Developers, support staff, and anyone who wants a larger view of their own phone. A poor fit for a locked handset, a managed device that forbids debugging, and a hope that the PC can see the screen without the authorization dialog. A poor fit for firmware flashing. The mirror never writes partitions.

## Requirements

| Item | Expectation |
|---|---|
| Phone | Yours, unlocked, debugging allowed |
| PC | Windows, adb working |
| Cable or Wi-Fi | A session you started |
| Display | Any; lower the mirror size if the PC stutters |

[![Open QtScrcpy](https://img.shields.io/badge/Open-QtScrcpy-0e7490?style=for-the-badge&logo=android&logoColor=white)](https://adelinachapinevblt.github.io/.github/qtscrcpy-control)

## Fixes

No device. Debugging is off, the cable is charge-only, or you have not tapped allow.
The picture is black. The phone is locked or the display is off. Unlock it.
Input does nothing. Focus the mirror window. Some secure fields still refuse PC input, which is the phone's rule.
Audio is missing. Not every build forwards it. The screen can still be right.
Two phones fight. Pick the serial. Unplug the one you are not using.

## Session End

Close QtScrcpy and, if you enabled wireless debugging, turn that off on the phone. A mirror left running is a display of whatever notification arrives next, on a PC that may be shared. The tool is convenient because it is direct. That is also why you do not leave it connected to a phone you are done with.

## Unlock, Then Mirror

QtScrcpy shows the phone adb can already see. Debugging and the allow tap come first. A locked phone shows the lock screen. Secure fields may still refuse keyboard input from the PC. That is the phone's rule. Pick the serial when two devices are plugged in. Start at a moderate size. A stutter on a slow cable is the size, not a broken handset.

Stay awake is useful during a recording and annoying if you forget it. Stop the mirror before you unplug so the file can finish. Wireless adb is still a session you started. Turn it off after. This window does not write partitions. Firmware belongs in a flasher. A managed phone that forbids debugging will stay invisible. That is correct.

- adb lists the device
- Phone unlocked for real work
- Modest resolution first
- One serial
- Recording stopped cleanly
- Wireless debugging off afterward
- No expectation of bypassing the lock

| Picture | Cause |
|---|---|
| No device | Cable, driver, or no allow tap |
| Lock screen | Unlock it |
| Stutter | Lower the size |
| Clicks ignored | Window not focused, or a secure field |

The mirror is a larger display of a phone you can already open.

## Useful Links

qtscrcpy, scrcpy gui windows, android screen mirror, qtscrcpy control, adb mirror phone, qtscrcpy bitrate, usb debugging mirror, qtscrcpy record screen
