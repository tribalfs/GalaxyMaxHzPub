
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
   * GMH will automatically apply a workaround to bypass 60Hz limitation on Power Saving Mode (PSM) on supported Samsung smartphones.
      (not working on all devices with OneUI4.**+, test first). [^1] Devices with OneUI5.* and those few with OneUI4.* require extra steps[^3]


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
       - Do a dummy (fake) video call to any number using the [native video call app](https://user-images.githubusercontent.com/65062033/216779623-7e7d78f1-e6cc-421a-8ab3-02f1d2712dec.png) (not google duo; availability depends on SIM/mobile plan support) OR
       - Connect and disconnect to a wifi display receiver (e.g. smart tv, chromecast, windows laptops) using the Smart View function OR
       - Connect and disconect to Samsung Dex on TV using an HDMI cable or Samsung Dex on PC using USB data cable. Connect the phone and confirm "Start now" prompt and disconnect once Samsung Dex has started. 
 

Note for modified ROM users: The app may or may not work depending on app's dependencies modified. Tweaks that modify the device model number in the build prop (Build.MODEL) will cause bugs on the app including the license verfication.
