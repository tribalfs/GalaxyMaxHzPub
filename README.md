<img src="https://github.com/user-attachments/assets/99a71252-8697-47b5-a1e5-1dd1884e1f3f" width=235 height=480> <img src="https://github.com/user-attachments/assets/d157a94b-2899-4f01-9f21-4c145ebc5ba4" width=235 height=480> <img src="https://github.com/user-attachments/assets/8b2a09dc-1a62-4950-81bb-b5ca8255a002" width=235 height=480> 

<img src="https://github.com/user-attachments/assets/a1503018-e6df-4868-8916-afb7c9a3bd08" width=235 height=480> <img src="https://github.com/user-attachments/assets/447365df-8493-4de9-8a00-d997c5f8b715" width=235 height=480> 
<img src="https://github.com/user-attachments/assets/66519a55-7720-419b-ae4b-5fc7953c2885" width=235 height=480> 


Galaxy MaxHz[^2]
======

#### Refresh Rate Mods

* Change default refresh rates
    * Easily change the overall refresh rate settings of devices supporting multiple refresh rates.
    * Set supported mid refresh rates as the maximum refresh rate limit for battery savings (e.g.
      96hz instead of 120Hz).
    * Set refresh rates for low battery state.
    * Quick settings shortcut[^1]
    * Tasker plugin support
    * Configure separate default refresh rates when folded for supported Samsung Galaxy Z Fold
      devices [premium]

* Refresh rate mode switcher(Normal, Adaptive or High)[^1]
    * Set you device motion smoothness mode to stationary refresh rates (high mode) for better
      smoothness if so desired on Samsung devices with native Adaptive motion smoothness with a
      little trade-off to the battery.
    * Adaptive refresh rate mod on devices that don't natively support adaptive refresh rate
      mode [premium][^1]
    * Tasker plugin support

* Per-app refresh rate settings[premium]:
    * Configure different refresh rate settings for different apps, either adaptive or static .
    * Separate settings can be set for inner and outer screen for supported Samsung Galaxy Z Fold
      devices.

* Prevent switching to Standard mode on power saving mode [premium]
    * Prevent system from switching to Standard mode when power saving mode is enabled
    * Enforce CPU speed limit on Power Saving Mode even with Adaptive/High mode (OneUI7+)
    * GMH will automatically apply a workaround to bypass 60Hz limitation on Power Saving Mode (PSM)
      on supported Samsung smartphones[^1].

      _Devices with OneUI5/OneUI6 and those few with OneUI4.* require extra steps, except when using
      the Xposed/LSPosed module._

#### Screen-off Mods:

* Screen off/AOD refresh rate (Force to Lowest Hz)
    * Force the lowest refresh rate on screen-off or Always-On Display(AOD) to improve standby power
      consumption a bit.
    * Select refresh rate to set for AOD/screen-off[premium]
    * Tasker plugin support.

* Auto power saving mode on screen-off[^1]

* Auto disable Autosync

* Quick-doze mod[^1]
    * Quickly enter doze mode during screen-off that can not be interrupted by motion to improve
      standby power consumption[premium]
    * Tasker plugin support

* Auto SENSORS OFF (Supports up to OneUI4 only)
    * Device sensors will automatically turn off while screen is off until the device is unlocked to
      help minimize battery-draining motion-triggered wakelocks while device is not being
      used [premium]
    * Tasker plug-in support

#### Extras

* Battery protection mod[premium][^1] (for OneUI4+)
    * Option to set different maximum charge limit other than stock limit
    * Option to enable pass-through (battery by-pass) on supported models.
    * Option to sscheduled maximum charge limits and/or pass-through mode.

* Animation mod[^1]
    * Easily adjust animation duration and scale

* Keep force resizable activites[^1]

* Re-enable wifi sharing (hotspot source)[^1]

* Animation mod[^1]

* Quick resolution switcher[^1]
    * Easily switch to any supported resolutions using the included quick setting tile
    * Tasker plugin support


* Customizable refresh rate monitor
    * Use statusbar or overlay which you can place anywhere on screen.
    * Tasker plugin support

* Statusbar net speed indicator
    * Quick settings toggle [premium][^1]

[^1]: These marked features of Galaxy Max Hz need [**WRITE_SECURE_SETTINGS
**](https://github.com/tribalfs/GalaxyMaxHzPub/wiki/How-to-grant-WRITE_SECURE_SETTINGS) permission
in order to work.


[^2]: [Downloads](https://github.com/tribalfs/GalaxyMaxHzPub/releases)



Note for modified ROM users: The app may or may not work depending on app's dependencies modified.
Tweaks that modify the device model number in the build prop (ro.product.vendor.model) will cause
bugs on the app including the license verification.
Also, do not restore app from backup, always fresh install.

Info:
This app targets older android sdk in order to control refresh rates without ADB setup or root. Just
tap OK the dialog that says "This app was built for an older version of Android...." when opened for
the first time. If OK button is not visible, just tap the blank space on the lowest portion of the
dialog.

##### Only Samsung devices are officially supported. Features may or may not work on other devices.

#### [Important Notes for installing it on OneUI6.0(Android14) and above](https://github.com/tribalfs/GalaxyMaxHzPub/wiki/How-to-install-on-OneUI6(Android-14)-and-above)

[Contact developer](mailto:tribalfs@gmail.com?subject=[GitHub]%20Galaxy%20MaxHz)
