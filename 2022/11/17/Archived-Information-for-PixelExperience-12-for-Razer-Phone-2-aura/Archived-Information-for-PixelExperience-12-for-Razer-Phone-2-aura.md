---
title: Archived Information for PixelExperience 12 for Razer Phone 2(aura)
date: 2022-11-17 22:21:30
tags:
---
Hello, this is Alcatraz

As you can see this post, our PixelExperience (Plus) 12 project for Razer Phone 2 comes to it's EOL. Here I want to show you history update information and provide you history version download.

***History Updates (non-plus):***

*2021.12.12 (first release)*
>Introduce Android 12
fix flashlight and multi camera
fix refreshrate control
add chroma, dolby

*2021.12.13*
>IMS, Mobile data fixed
Color profile now selectable not system crashing

*2021.12.15*
>fix 1213's boot loop issue
fix ANR on android.hardware.secure_element

*2021.12.21*
>fix sdcard issue, now it is fully functional on PE, also can format and using exFAT which has no 4G file size limit
fix fingerprint now shown on mine or los, but available on stock rom or arter kernel(dtbo disabled)

*2021.12.24 (\*Recommend clean flash for update)*
>sync PE stable
SeLinux enforcing
SafetyNet Passing

*2022.1.14*
>fix system animation stuck
fix volume distortion under 50%
Sync PE upstream

*2022.1.15*
>fix nfc issue

*2022.1.18*
>fix fingerprint sleep to death
fix color mode issue(inverse color, color space simulation or color profile change cause bootloop)

*2022.1.20*
>add system updater (OTA)

*2022.2.23 (\*OTA available)*
>kernel: merge upstream 4.9.302
kernel: merge Tag LA.UM.10.3.r1-00900-sdm845.0
device: fix refresh rate setting mismatch value and summary
February Security patch
Face Unlock added

*2022.3.1 (\*OTA available, but clean flash recommended for Dolby to keep alive)*
>device: totally fixed some game volume distortion or too low under 50%
device: fixed Dolby function and Dolby Tile service in systemui
device: fixed Ok Google function
device: fixed video cause screen freezing
device: add Aptx, Aptx HD codec
device: moved RazerParts App to Settings and add icon


*2022.3.7 (\*OTA available from 3.1 and after, but if FROM BEFORE 3.1, MUST CLEAN FLASH)*
>device: Fix Discord gif freezing
device: Fix mic too low
device: Add Dolby Atmos for a2dp
device: Add Built in Google Camera
device: RazerParts: chroma brightness fix
device: RazerParts: chroma on booting fix
device: RazerParts: function: kill chroma after screen lock
device: RazerParts: add 40hz refresh rate
device: RazerParts: fix Dolby Atmos jump
device: RazerParts: fix chroma switch override
device: Update WifiDisplay blobs

*2022.3.31 (\*OTA available from 3.1 and after, but if FROM BEFORE 3.1, MUST CLEAN FLASH)*
>Upstream:
 Android 12L
 March update
Device:
kernel: Merge tag LA.UM.10.3.r1-01000-sdm845.0
 kernel: Merge 4.9.309
 device: fix hardware decoder for video low fps
 device: fix 4k video recording
 device: update IMS related blobs
 device: fix fingerprint animation location
 device: add QuickTap function

*2022.4.1 (\*OTA available from 3.1 and after, but if FROM BEFORE 3.1, MUST CLEAN FLASH)*
>Tiny update from 3.31
 device: fix 3.31's refresh rate can't switch
 device: update MGC Gcam to 8.4.500_A10_V5

*2022.4.16 (\*OTA available from 3.1 and after, but if FROM BEFORE 3.1, MUST CLEAN FLASH)*
>Device:
 device: fix aac for tws or normal headset
 device: fix aac for truck bluetooth stereo
 device: fix mic too low for any type video recording
 device: fix mic crash for in game tws(like pubg)
 device: fix Dolby conflict with ok google/adaptive sound
 device: tune speaker least volume
 device: add back Aptx, Aptx HD codec
 device: universal audio fix
 device: bring back active wake(pick up and wake/Doze)
Upstream:
 April security patch
 Fixed charging animation not appearing
 Fixed unlock sound playing repeatedly
 Updated translations
 Others fixes

*2022.5.27*
>Device:
 kernel: merge LA.UM.10.3.r1-01700-sdm845.0 from Qualcomm
 kernel: merge 4.9.316 from aosp
 device: fix gpu error for "masterduel" and some other games
 device: fix charge interrupt frequently under 50%
 device: offline charging animation change(fixed bzzz lines)
 device: Gcam update(telescope back)
Upstream:
 May security patch
 Updated translations and gapps
 Fixed battery widget not working properly
 Fixed rotation button not showing in 2-button navbar mode
 Others fixes

*2022.6.21*
>Device:
 device: correct 2k screen display density & use 2k icons
Upstream:
 June security patch
 Updated translations
 Fixed video playback issues on some devices
 Fixed styling issues on DocumentsUI
 Fixed ringtone selection for devices with e-SIM
 Fixed location indicator showing when no apps running
 Fixed app font on Pixel Launcher
 Other minor issues have been fixed

*2022.7.8*
>Device:
 device: enable wifi display mouse input
 kernel: merge 4.9.321
 kernel: merge wireguard driver 1.0.20220627
Upstream:
 July security patch
 Updated translations
 Fixed storage usage issue on OTA app
 Other minor issues have been fixed

*2022.8.15*
>Device:
 device: speaker tuning for better audio quality
 device: fully fixed lowest volume
 device: add stock RazerCamera 2.8.613 from SMR7
 device: add Telephony Rx for voip_tx input source
 kernel: merge 4.9.325
Upstream:
 August security patch
 Monet bootanimation added
 Updated translations
 Other minor issues have been fixed

*2022.9.15*
>Device:
 kernel: merge 4.9.327
 device: audio improvement
 device: mic gain for voice increase
 device: removed aosp camera
Upstream:
 GApps power drain issue fix
 September security patch
 Updated translations
 Other minor issues have been fixed

*2022.10.16*
>Device:
 device: audio improvement (Ver 2022.oct)
 device: further increase mic volume
Upstream:
 October security patch
 Updated translations
 Other minor issues have been fixed

*2022.11.12 (FINAL)*
>Device:
 device: merge 4.9.332
 device: BSG GCam update to 8.6.263_A11_V10
Upstream:
 November security patch
 Updated translations
 Other minor issues have been fixed

==============================================

***History Plus Updates:***

*2022.4.21*
>LiveDisplay (color profile, display mode, reading mode, color calibration)
Hide Notch support.
StatusBar shortcuts
Rotation settings
Lock screen display (media cover, music visualizer, power menu)
Per-app volume settings
Increasing ring volume
Different gestures
Power and Volume button customisations
Network traffic monitor
Brightness (brightness slider, auto brightness, brightness control)
Quick settings (quick pulldown, title visibility, vibrate on touch, rows, columns)
more other functions

*2022.5.27*
>Improved statusbar brightness control
Introduced more granular settings for hotspot(5G, always on, blacklist)
Reverted QS background on white theme to old style

*2022.6.21*
>Fixed network traffic behavior when toggling clock position to center

*2022.7.8*
>-N/A

*2022.8.15*
>-N/A

*2022.9.15*
>-N/A

*2022.10.16*
>-N/A

==============================================

***Archive Download:***
[[Archive]](https://www.androidfilehost.com/?w=files&flid=328764)