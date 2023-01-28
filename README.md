
 <img src="https://forum.xda-developers.com/attachments/screenshot_20220819-102810_galaxy-maxhz-jpg.5689917" width=235 height=480><img src="https://forum.xda-developers.com/attachments/screenshot_20220819-102819_galaxy-maxhz-jpg.5689919" width=235 height=480><img src="https://forum.xda-developers.com/attachments/screenshot_20220819-102912_galaxy-maxhz-jpg.5689921" width=235 height=480>

Galaxy MaxHz[^2]
======
#### Refresh Rate Mods

* Change default refresh rates
   * Easily change the overall refresh rate settings of devices supporting multiple refresh rates.
   * Set supported mid refresh rates as the maximum refresh rate limit for battery savings (e.g. 96hz instead of 120Hz).
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
      (not working on all devices with OneUI4.**+, test first). [^1]


#### Screen-off Mods:

* Screen off/AOD refresh rate (Force to Lowest Hz)
   * Force the lowest refresh rate on screen-off or Always-On Display(AOD) to improve standby power consumption a bit.
   * Select refresh rate to set for AOD/screen-off[premium]
   * Tasker plugin support.

* Auto power saving mode on screen-off[^1]

* Auto disable Autosync[^1]

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

[Note for modified ROM users](https://github.com/tribalfs/GalaxyMaxHzPub/wiki/Frequently-Asked-Questions-(FAQs)#4-i-have-a-modified-rom-will-this-app-work)
