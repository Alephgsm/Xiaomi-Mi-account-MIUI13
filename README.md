# How to bypass mi account of xiaomi devices up to MIUI13
How to bypass mi account of xiaomi devices up to MIUI13 and disable OTA Update with adb method

* first boot device to normal mode and enable adb

* for bypass mi account, If your device has been factory reset, you probably need to erase the following partitions in brom or edl mode.(If you can boot device to main menu and enable adb, there is no need to do this)

`config`, `frp`, `persist`

* for erasing this partitions you can use mtkclient or edl Of course, many devices require edl auth, for which you need to use other software.

anyway, finally run this code in adb mode for bypass mi account:

`adb shell pm uninstall -k --user 0 com.xiaomi.finddevice`

# run this code to disable OTA update

`adb shell pm uninstall -k --user 0 com.android.updater`

follow us in telegram:
https://t.me/Alephgsm
