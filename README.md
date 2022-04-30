# Galaxy Max Hz

Some features of Galaxy Max Hz need **WRITE_SECURE_SETTINGS** permission in order to work. For additional details, you can check the app's [official xda-developers thread](https://forum.xda-developers.com/t/app-galaxy-max-hz-refresh-rate-control-quick-resolution-switcher-screen-off-mods-adaptive-mod-keep-high-adaptive-on-power-saving-mode-and-more.4181447/).

----------------------
### TLDR

 * Run `adb shell pm grant com.tribalfs.gmh android.permission.WRITE_SECURE_SETTINGS`

----------------------
[VIDEO GUIDE](https://youtu.be/5lFPUqMC-Bc)
----------------------

Procedures to grant Galaxy Max Hz the WRITE_SECURE_SETTINGS permission using ADB:
----------------------


### 1. Enable developer mode in phone's settings

 * Go to `Settings` > `About phone` > `Software information` and tap `Build number` multiple times until the developer mode is enabled.

![about phone](about_phone2.jpg)

### 2. Enable USB debugging

 * Go to `Settings` > `Developer options` (can be `Settings` > `System` > `Developer options` on older android versions), scroll down and find `USB debugging` option.

![adb](usb_debugging2.jpg)

### 3. Download ADB on your computer

 * Download ADB (platform-tools) to your computer:
    for [Windows](https://dl.google.com/android/repository/platform-tools-latest-windows.zip) |
    for [Mac](https://dl.google.com/android/repository/platform-tools-latest-darwin.zip) |
    for [Linux](https://dl.google.com/android/repository/platform-tools-latest-linux.zip)
    
 * Extract the downloaded zip file.

### 4. Navigate inside the `platform-tools` folder that you extracted on Windows Explorer or Finder(macOS)


### 5. Opening the command-line interface

#### For Windows: Open up CMD
  
 * Type `cmd` in the address bar and press enter.  This will open Windows Command Prompt.

![opening_cmd](opening_cmd.png)

#### For MacOS: Open up Terminal

 * Search `Terminal` from Launchpad and run it.

 * Run `sudo -s` and type your user password. **The terminal won't display how much characters you type, it'll remain blank.**

 * Run `export PATH=.:$PATH`

 **Without this, you will get `adb: command not found` errors.**


### 6. Connecting your phone to your computer

 * Your phone will prompt `Allow USB debugging` if it's the first time being connected on USB debugging mode.  Tap `OK`.


![adb prompt](usb_debugging_prompt.jpg)

 * Check the connection by entering the following command followed by an enter. It should show your device ID if successfully connected.

 ```adb devices```
 
 ![adb_devices](adb_devices2.png)
 
 For macOS:  ```./adb devices ```
 
 *  If your device fails to connect to your computer, try connecting it a different USB port and/or using a different USB data cable. If still not connecting, your computer is possibly missing the USB driver for your phone. Check [here to download OEM USB drivers](https://developer.android.com/studio/run/oem-usb#Drivers). Once installed, reboot your PC and redo step no. 6. 

 
### 7. Actual granting of WRITE_SECURE_SETTINGS permission to Galaxy Max Hz

 * When successfully connected, enter the following command and press enter.  If the command is executed properly, it will return blank.

 ```adb shell pm grant com.tribalfs.gmh android.permission.WRITE_SECURE_SETTINGS```

![write_secure_settings](write_secure_settings2.png)

For macOS: ```./adb shell pm grant com.tribalfs.pixels android.permission.WRITE_SECURE_SETTINGS ```

### 8. You may now disable the USB debugging settings

 * If you don't need USB debugging, it's recommended to disable it to avoid potential unwanted access.

 * Go to `Settings` > `Developer options`, scroll down a page and **disable** `USB debugging` option.

**That's it!**

----------------------

Re-open Galaxy Max Hz. Done! 

----------------------
Alternative method:
If you are using [LADB](https://play.google.com/store/apps/details?id=com.draco.ladb) app:
 * Execute `pm grant com.tribalfs.gmh android.permission.WRITE_SECURE_SETTINGS`

----------------------

You don't have to repeat this process unless you completely uninstall the app and reinstall it.

---------------------

[FAQs](https://forum.xda-developers.com/t/app-galaxy-max-hz-refresh-rate-mods-screen-off-mods-qs-tiles-tasker-support-and-more.4181447/post-83785135)
---------------------

If you have any question or need more help, you may message us at tribalfs@gmail.com, in [XDA](https://forum.xda-developers.com/conversations/add?to=tribalfs) or ask in the dedicated thread for your device in XDA forum
---------------------

