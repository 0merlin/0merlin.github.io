# Android Resources

Over many many months I have found or been shown many useful tools that help with android development. From websites that generate icons, and colour schemes to short commands that can be used to do various things on your device via `adb` commands.

## Useful Websites

**Icon Generator**
:   <https://romannurik.github.io/AndroidAssetStudio/icons-launcher.html>

**Google Material Icons**
:   <https://design.google.com/icons/> or for all of them <https://github.com/google/material-design-icons/>

**Colour Schemes**
:   <http://www.materialpalette.com/>

## Useful Commands

### Screenshot

```bash
adb shell screencap -p /sdcard/screen.png
adb pull /sdcard/screen.png
adb shell rm /sdcard/screen.png

open screen.png # if you have a Mac then this works
```

### Install a local APK

```bash
adb install <apk file>

adb install -r <apk file> # to reinstall
```

### Copying files to and from a device:

```bash
# Copy from:
adb pull /location/to/folder

# copy to:
adb push /local/path /device/path
```
