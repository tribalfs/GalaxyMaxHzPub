# Galaxy Max Hz

Some features of Galaxy Max Hz need **WRITE_SECURE_SETTINGS** permission in order to work. For additional details, you can check the app's [official xda-developers thread](https://forum.xda-developers.com/t/app-galaxy-max-hz-refresh-rate-control-quick-resolution-switcher-screen-off-mods-adaptive-mod-keep-high-adaptive-on-power-saving-mode-and-more.4181447/).

----------------------
### TLDR

 * Run `adb shell pm grant com.tribalfs.gmh android.permission.WRITE_SECURE_SETTINGS`

----------------------

Alternative methods:

For **rooted** devices without using a PC:
 *  Install a terminal emulator app from play store (e.g. [Termux](https://play.google.com/store/apps/details?id=com.termux)), grant root permission and run the following command: `su -c pm grant com.tribalfs.gmh android.permission.WRITE_SECURE_SETTINGS`.
or (2) Install this [mini-app](https://github.com/tribalfs/gmhWriteSecureSettings/releases), grant root permission and run.

For **non-rooted** devices using [LADB](https://play.google.com/store/apps/details?id=com.draco.ladb) app:
 * Execute `pm grant com.tribalfs.gmh android.permission.WRITE_SECURE_SETTINGS`

----------------------

Procedures to grant Galaxy Max Hz App WRITE_SECURE_SETTINGS permission using ADB:
----------------------

### 1. Enable developer mode

 * Go to `Settings` > `About phone` > `Software information` and tap `Build number` multiple times until the developer mode is enabled.

![about phone](about_phone.png)

### 2. Enable USB debugging

 * Go to `Settings` > `Developer options` (can be `Settings` > `System` > `Developer options` on older android versions), scroll down and find `USB debugging` option.

![adb](adb.png)

### 3. Download ADB on your computer

 * Download ADB (platform-tools) to your computer:
    for [Windows](https://dl.google.com/android/repository/platform-tools-latest-windows.zip) |
    for [Mac](https://dl.google.com/android/repository/platform-tools-latest-darwin.zip) |
    for [Linux](https://dl.google.com/android/repository/platform-tools-latest-linux.zip)
    
 * Extract the downloaded zip file.

### 4. Navigate inside the folder that you extracted (i.e. inside platform-tools_r****-******) from Windows Explorer or Finder(macOS)

----------------------

### 5. Opening the command-line interface

#### For Windows: Open up CMD
  
 * Type `cmd` in the address bar and press enter. 

![1](1.png)

#### For MacOS: Open up Terminal

 * Search `Terminal` from Launchpad and run it.

 * Run `sudo -s` and type your user password. **The terminal won't display how much characters you type, it'll remain blank.**

 * Run `export PATH=.:$PATH`

 **Without this, you will get `adb: command not found` errors.**


### 6. Connect your phone to your computer

 * Your phone will prompt `Allow USB debugging` if it's the first time being connected on USB debugging mode.  Tap `OK`.
![adb prompt](adb_prompt.jpg)


### 7. Actual granting of WRITE_SECURE_SETTINGS permission to Galaxy Max Hz

 * Enter the following to the command followed by an enter. It should show your device ID if successfully connected.

 ```adb devices```

 * When successfully connected, enter the following to the command followed by an enter.  If the command executed properly, it'll return blank.

 ```adb shell pm grant com.tribalfs.gmh android.permission.WRITE_SECURE_SETTINGS```

![6](6.png)


### 8. You may now disable the USB debugging settings

 * If you don't need USB debugging, it's recommended to disable it to avoid potential unwanted access.

 * Go to `Settings` > `Developer options`, scroll down a page and **disable** `USB debugging` option.

### 9. Re-open Galaxy Max Hz. Done! 

**That's it!**

You don't have to repeat this process unless you completely uninstall the app and reinstall it.
