<img src="https://github.com/user-attachments/assets/99a71252-8697-47b5-a1e5-1dd1884e1f3f" width=235 height=480> <img src="https://github.com/user-attachments/assets/d157a94b-2899-4f01-9f21-4c145ebc5ba4" width=235 height=480> <img src="https://github.com/user-attachments/assets/8b2a09dc-1a62-4950-81bb-b5ca8255a002" width=235 height=480> 

<img src="https://github.com/user-attachments/assets/a1503018-e6df-4868-8916-afb7c9a3bd08" width=235 height=480> <img src="https://github.com/user-attachments/assets/447365df-8493-4de9-8a00-d997c5f8b715" width=235 height=480> 
<img src="https://github.com/user-attachments/assets/66519a55-7720-419b-ae4b-5fc7953c2885" width=235 height=480> 


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
    * Option to set different maximum charge limit other than stock limit
    * Pass-through mode (battery by-pass) with customizable threshold on supported models.
    * Option to scheduled maximum charge limits and/or pass-through.

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
