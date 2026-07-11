67<img src="https://github.com/user-attachments/assets/f7e60aa4-573e-464f-8840-702f114a56f7" width=235 height=490>
<img src="https://github.com/user-attachments/assets/af7382fe-7d3f-4010-b2c9-d00d94ff825d" width=235 height=490>
<img src="https://github.com/user-attachments/assets/1724c78d-7623-45a2-9fa8-c6bac01da131" width=235 height=490>
<img src="https://github.com/user-attachments/assets/15b842eb-4c4d-4256-9fc3-b382583ee0ca" width=235 height=490> 
<img src="https://github.com/user-attachments/assets/ba5364c5-7b3b-4948-b210-f0394707567d" width=235 height=490>
<img src="https://github.com/user-attachments/assets/dfe8a619-b46c-41f7-91a5-dfe9615c9b1c" width=235 height=490> 
<img src="https://github.com/user-attachments/assets/63cd4f87-50b7-474a-9229-729aa4d38a46" width=235 height=490>


Galaxy MaxHz[^2]
======

#### Refresh Rate Mods

* Change default refresh rates of devices supporting multiple refresh rates.
    * Set supported mid refresh rates as the maximum refresh rate limit for battery savings.
    * Configure separately for Power Saving Mode and Low Battery State, as well as for the main and outer screens on supported foldables [premium]

* Refresh rate mode switcher(Normal, Adaptive or High)[^1]
    * Set you device motion smoothness mode to stationary refresh rates (high mode) for better smoothness if so desired.
    * Adaptive refresh rate mod on devices that don't natively support adaptive refresh rate  mode [premium][^1]

* Per-app refresh rate settings[premium]:
    * Assign adaptive or static refresh rates per app.
    * Configure individually for main screen and outer screens on supported foldables.
      
* Refresh rate monitor

* Prevent switching to Standard mode on power saving mode [premium]
    * Prevent system from switching to Standard mode when power saving mode is enabled
    * Enforce CPU speed limit on Power Saving Mode even with Adaptive/High mode (OneUI7+)
    * GMH will automatically apply a workaround to bypass 60Hz limitation on Power Saving Mode (PSM) on supported devices.

      _Devices with OneUI5/OneUI6 and those few with OneUI4.* require extra steps, except when rooted and using the Xposed/LSPosed module._

* Screen off/AOD refresh rate
    * Force the lowest supported refresh rate on screen-off or Always-On Display(AOD) to improve standby power consumption a bit.
 
      
#### Screen-off Mods:

* Auto power saving mode on screen-off[^1]
    *  Auto enable power saving mode when the screen is off, and disable it when the screen turns back on.
  
* Auto disable Autosync
  *  Auto disable Autosync when the screen is off, and disable it when the screen turns back on

* Quick-doze mod[^1]
    * Quickly enter doze mode to improve standby drain with customizable maintenance interval [premium]
    * Remove apps from Doze system whitelist to allow system to restrict or optimize their background/standby usage.
 
* Auto SENSORS OFF (Supports up to OneUI4 only)

#### Extras

* Battery protection mod[premium][^1] (for OneUI4+)
    * Option to suspend charging by thermal thresholds
    * Option to customize charge limit and recharge level
    * Pass-through mode (battery by-pass) with customizable threshold on supported models.
    * Set schedules for charge limits and/or pass-through.


* Animation mod[^1]
    * Easily adjust animation duration and scale

* Keep force resizable activites[^1]

* Quick resolution switcher[^1]
    * Easily switch to any supported resolutions using the included quick setting tile

* Statusbar net speed indicator
    * Quick settings toggle [premium][^1]

#### Integrations

* Tasker
* App shortcuts

[^1]: These marked features of Galaxy Max Hz need [**WRITE_SECURE_SETTINGS
**](https://github.com/tribalfs/GalaxyMaxHzPub/wiki/How-to-grant-WRITE_SECURE_SETTINGS) permission in order to work on non-rooted device. This can be granted automatically on rooted device.


[^2]: [Downloads](https://github.com/tribalfs/GalaxyMaxHzPub/releases)



Note for modified ROM users: The app may or may not work depending on app's dependencies modified.
Tweaks that modify the device model number in the build prop (ro.product.vendor.model) will cause
bugs on the app including the license verification. Also, do not restore app from backup, always fresh install.

Info:
This app targets older android sdk in order to control refresh rates without ADB setup or root. Just
tap OK the dialog that says "This app was built for an older version of Android...." when opened for
the first time. If OK button is not visible, just tap the blank space on the lowest portion of the
dialog.

##### Only Samsung devices are officially supported. Features may or may not work on other devices.

### Installation instructions for [OneUI6.0 (Android14) and above](https://github.com/tribalfs/GalaxyMaxHzPub/wiki/How-to-install-on-OneUI6(Android-14)-and-above)

[Contact developer](mailto:tribalfs@gmail.com?subject=[GitHub]%20Galaxy%20MaxHz)
