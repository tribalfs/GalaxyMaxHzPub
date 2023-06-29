---
name: Bug report
about: Create a report to help us improve
title: ''
labels: ''
assignees: ''

---

**Important: Before submitting a bug, ensure to check [FAQs](https://github.com/tribalfs/GalaxyMaxHzPub/wiki/FREQUENTLY-ASK-QUESTIONS-(FAQs))  and in the app description in the appropriate XDA forum thread for your device to ensure that the behavior is not expected or not part of the limitation of the app.**

**Describe the bug**
A clear and concise description of what the bug is.

**To Reproduce**

A. GMH version and the exact settings in GMH

B. Steps to reproduce the behavior:
1. Go to '...'
2. Click on '....'
3. Scroll down to '....'
4. See error

**Expected behavior**
A clear and concise description of what you expected to happen.

**Screenshots**
If applicable, please include screenshots and/or [screen recording](https://play.google.com/store/apps/details?id=us.rec.screen) to help explain your problem. 

**Smartphone (please complete the following information):**
 - Model Number: [e.g. SM-S908B]
 - OS/OneUI version:  [e.g. android12 OneUI4.1]
 - Date of latest security update, if applicable: [e.g. June 2022]
 - Stock or modded ROM?

**Additional context**
Add any other context about the problem here.

**Crashlog**
If GMH crashes on your device, please include the crashlog of your device.  Just execute the following adb command. 
`adb logcat -c`.  
Then reproduce the crash.   Then execute this right after the crash (device must not be rebooted yet):
`adb logcat -b crash > crashlog.txt`
_Ctrl+C_ after 10seconds.
Then locate _crashlog.txt_ file in your adb installation folder then send it to tribalfs@gmail.com.
