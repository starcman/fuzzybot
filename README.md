# Uninstall factory apps from android

## Enable Developer Settings
1. Open the Settings app on your phone and scroll down to About Phone.
1. Tap on the Build Number seven times to enable Developer Options.
1. Go back to the Settings menu and go to System > Developer Options
1. Enable USB Debugging.

## Install adb 

For Ubuntu
```
sudo apt-get install android-sdk-platform-tools
```


## Uninstall packages

Should show one device attached
```
adb devices
```

Takes you to custom shell
```
adb shell
```

List the packages & grep a particular package

```
pm list packages | grep youtube
```

Uninstall the package 

```
pm uninstall -k --user 0 packageFullName
```


## Credits
1. **[Install adb](https://www.xda-developers.com/install-adb-windows-macos-linux/)**
1. **[Remove apps](https://www.xda-developers.com/uninstall-carrier-oem-bloatware-without-root-access/)**