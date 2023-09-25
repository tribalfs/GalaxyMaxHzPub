
<img src="https://user-images.githubusercontent.com/65062033/216784718-83153bf4-9a8f-4dec-8e67-3c922ed803fe.png" width=235 height=480> <img src="https://user-images.githubusercontent.com/65062033/216784714-c7182db7-6b6c-43c8-bf1b-66b15247ec4e.png" width=235 height=480> <img src="https://user-images.githubusercontent.com/65062033/216784711-233fd3ba-5011-4a0f-b1f7-829018660dcd.png" width=235 height=480>

Galaxy MaxHz[^2]
======
#### Refresh Rate Mods

* Change default refresh rates
   * Easily change the overall refresh rate settings of devices supporting multiple refresh rates.
   * Set supported mid refresh rates as the maximum refresh rate limit for battery savings (e.g. 96hz instead of 120Hz).
   * Set refresh rates for low battery state.
   * Quick settings shortcut
   * Tasker plugin support

* Refresh rate mode switcher(Normal, Adaptive or High)[^1]
   * Set you device motion smoothness mode to stationary refresh rates (high mode) for better smoothness if so desired on Samsung devices with native Adaptive motion smoothness with a little trade-off to the battery.
   * Apply adaptive refresh rate mod on device that don't natively support adaptive refresh rate mode [premium][^1]
   * Tasker plugin support

* Per-app refresh rate settings:
   * Set different refresh rate settings for every app to either adaptive or static [premium].

* Keep selected refresh rate mode on power saving mode [premium]
   * Prevent system from switching to Standard mode when power saving mode is enabled
   * GMH will automatically apply a workaround to bypass 60Hz limitation on Power Saving Mode (PSM) on supported Samsung smartphones [^1].
      Devices with OneUI5.* and those few with OneUI4.* require extra steps[^3] except when rooted with Magist and LSPosed module installed.


#### Screen-off Mods:

* Screen off/AOD refresh rate (Force to Lowest Hz)
   * Force the lowest refresh rate on screen-off or Always-On Display(AOD) to improve standby power consumption a bit.
   * Select refresh rate to set for AOD/screen-off[premium]
   * Tasker plugin support.

* Auto power saving mode on screen-off[^1]

* Auto disable Autosync

* Quick-doze mod
   * Quickly enter doze mode during screen-off that can not be interrupted by motion to improve standby power consumption[premium][^1]
   * Tasker plugin support

* Auto SENSORS OFF (experimental non-root workaround)
   * Device sensors will automatically turn off while screen is off until the device is unlocked to help minimize battery-draining motion-triggered wakelocks while device is not being used [premium]
   * Tasker plug-in support
   * Note: Supports up to OneUI4 only


#### Extras

* Battery protection mod
   * Option to set maximum charge to 86%-95%(for OneUI4+)[premium]

* Quick resolution switcher[^1]
   * Easily switch to any supported resolutions using the included quick setting tile
   * Tasker plugin support


* Customizable refresh rate monitor
   * Use statusbar or overlay which you can place anywhere on screen.
   * Tasker plugin support

* Statusbar net speed indicator





[^1]: These marked features of Galaxy Max Hz need [**WRITE_SECURE_SETTINGS**](https://github.com/tribalfs/GalaxyMaxHzPub/wiki/How-to-grant-WRITE_SECURE_SETTINGS) permission in order to work. 


[^2]: [Downloads](https://github.com/tribalfs/GalaxyMaxHzPub/releases)

[^3]: Extra steps required for some devices.  After selecting Adaptive or High mode while on power saving mode, either:
       - Do a dummy (fake) video call to any number using the [native video call app](https://user-images.githubusercontent.com/65062033/216779623-7e7d78f1-e6cc-421a-8ab3-02f1d2712dec.png) (not google duo; availability depends on SIM/mobile plan support);
       
       - Game booster method. First, open Game Booster settings and ensure "Save power during touch protection" is turned on AND "Shortcut bar" is also turned on OR "Floating shortcut" is set to Touch Protection.
       Here are the steps:
        1. Select Adaptive Mode while on power saving mode
        2. Open any game (preferably from game launcher)
        3. Press the [touch protection button](https://forum.xda-developers.com/attachments/1676681590219-png.5839707/)(lock icon) in the floating shortcut bar and wait for the screen to dim ("Drag lock icon to unlock" text will fade)
        4. Touch the screen and unlock;

       - Connect and disconnect to a wifi display receiver (e.g. smart tv, chromecast, windows laptops) using the Smart View function; OR
       
       - Connect and disconect to Samsung Dex on TV using an HDMI cable or Samsung Dex on PC using USB data cable. Connect the phone and confirm "Start now" prompt and disconnect once Samsung Dex has started. 

 


Note for modified ROM users: The app may or may not work depending on app's dependencies modified. Tweaks that modify the device model number in the build prop (Build.MODEL) will cause bugs on the app including the license verfication. Also, do not restore app from backup, always fresh install.

##### Only Samsung devices are officially supported. Features may or may not work on other devices.
#### Notes for OneUI6.0 (Android14) : 
* **Starting OneUI6.0, installing the app on OneUi6.0 requires doing  it via ADB using this command:**
  * `adb install --bypass-low-target-sdk-block galaxy_max_hz_v8.1.apk`

* **You also need to "Allow restricted settings" to the app:**
  * Open Galaxy MaxHz > Go to About app in top right menu > Click the info (i) icon > Click top right menu in the window that will open > Click Allow restricted settings


[Contact developer](mailto:tribalfs@gmail.com?subject=[GitHub]%20Galaxy%20MaxHz)
