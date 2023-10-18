---
title: Archived Information for PixelExperience 13 for Xiaomi Mi Pad 4 / 4 Plus(clover)
date: 2023-10-18 12:00:53
tags:
---
Hello, this is Alcatraz

As you can see this post, our PixelExperience (Plus) 13 project for Xiaomi Mi Pad 4 / 4 Plus comes to it's EOL. Here I want to show you history update information and provide you history version download.

***History Updates (non-plus):***

*2023.2.10 - First release*
>Device:
Introduce PE 13 for Mi Pad 4 (Plus)

*2023.2.12*
>Device:
kernel: switched to 4.19
device: add mi settings

*2023.2.18*
>Device:
kernel: fixed wake brightness burst
kernel: backported fuse passthrough from kernel 5.4 for better android storage performance
device: fixed camera stuck in 3rd app
device: moved xiaomi settings back in Settings -> System
device: added auto removal for wifi only/no fingerprint models
device: switched to erofs, f2fs, fbeV2+emmc_optimization(MUST use new recovcery and FORMAT DATA)
device: fixed weird power off charging ui
device: fixed SD card format in two modes
device: fixed microphone
device: enabled ZRAM writeback

*2023.2.20*
>Device:
device: fixed backlight adjustment on Plus variant
device: fixed usb mode detect on Windows(Mtp or so)

*2023.2.24 - First OFFICIAL build*
>device: fixed real MAC reading
device: fixed charging led won't work on high battery percent
device: fully translated xiaomi settings for CN

*2023.2.27*
>Device:
device: fixed brightness driver burst for 8inch. (Plus has no burst issue)
device: fixed device setting can't display by side as tablet mode
kernel: update to 4.19.273
kernel: power optimized

*2023.3.3*
>Device:
device: fixed "UNKNOWN SOC TYPE" in some system info type apps (SDA660)
device: fixed cpu freq scheduler always locks max freq by uclamp
device: enabled 60fps recording in camera
device: enabled cgroup freezer
Upstream:
February security patch
Google Apps updated
Fixed battery drain and lag spike caused by Pixel Launcher (Need to uninstall previous updates of Android System Intelligence or do a clean flash if the issue persists)
Fixed SafetyNet not passing

*2023.3.24/5*
>Device:
kernel: update to 4.19.278
kernel: backport 5.10 fuse filesystem
kernel: reduce power consumption for 8 inch screen
device: reduce continuous ui rendering jitter/lag

*2023.4.1*
>Device:
device: add "Usb fast charge on usb3.0 port"(500mA - 900mA) in Xiaomi Settings
device: switch to aosp task/cpu management for some critical tasks(util clampimg)
device: audio quality HUGE fix
device: "Mi Pad 4 Plus" will be differred in System info as well as the default dpi
device: lower memory pressure caused by bad Qualcomm legacy io scripting
device: optimize round corner
device: won't show a fingerprint page on first boot setup for 8inch now
device: complete software codec2 support (aosp_sw)
device: use qti-usb@1.3 HAL(full USB config panel like reverse charging/role change)
device: set baseband as "Wi-Fi Only" instead of "Unknown" for wifi variant
device: further improve ui/animation lagging
device: optimize RAM consumption
device: optimize background app caching
device: deprecated sdcardfs and use native Android 11 new filesystem base, which supports better scope storage
device: more balanced irq control
device: other minor fix
kernel: minor optimize
Upstream:
Fixed something bad in QPR2(0324/5, below is copied from last)
Android 13 Quarterly Platform Release 2 (QPR2 - lots of new ui/behavior changes)
Enabled multi user switcher on lock screen for large screen device(>600dp)
Source rebased with March security patch
Updated GApps
Updated translations
Minor fixes

*2023.4.19*
>Device:
kernel: update to 4.19.279
kernel: switch default io scheduler to bfq(reduce cpu consumption/power/lag, also +1500 AnTuTu storage score)
kernel: fixed step-chg/sw-jeita(thermal) for pm660_charger/fg
kernel: fixed otg passive mode issue, need one REBOOT after OTA/sideloading
device: fixed system partition not in erofs(increase boot up speed, system app speed)
device: make setup wizard landscape available
device: enable auto rotate by default
device: separate notification and ringtone volumes
device: fixed charge speed issue for LTE/Plus after hang off a call
device: force recovery update with system
device: irq balance now using 4 big cores (previously only 2 big cores)
device: CloverParts: add volume panel trigger in QS
device: CloverParts: add my battery manage system (Settings -> Battery -> Battery Management System) - Step charger / thermal charger switch
-Mode: limit battery around 40-60%
-Mode: limit battery around 80%
Upstream:
April security patch
Updated translations
Optimizations on battery usage of Pixel Launcher
Minor issues fixed

*2023.5.3*
>Device:
kernel: update to 4.19.282
kernel: sdm660 kernel driver update from qcom(wifi/kernel/audio)
kernel: minor fix & optimize
device: expand wifi signal tolerance(reduce disconnect on bad wifi)
device: update display driver for sdm660(gralloc - HAL/display)

*2023.5.7*
>Device:
device: allow 5G hotspot(called "Extend compatibility" in settings, reuquires a factory reset if you need it)
Upstream:
May security patch
Updated translations
Updated Google Apps
Minor issues fixed

*2023.5.19*
>Device:
kernel: qcom sdm660 kernel update LA.UM.11.2.1.r1-03900-sdm660.0(kernel main/kgsl/wifi-fw-api)
device: qcom sdm660 driver/HAL update LA.UM.11.2.1.r1-03900-sdm660.0(camera/audio)
device: add fastbootd option in advanced reboot(pe plus only, normal pe has no advanced reboot function)
device: add a switch in battery management system to turn off charging ripple animation
Upstream:
Minor platform framework fix

*2023.7.14*
>Device:
kernel: fix low power mode wrong booting behavior
kernel: fix rmnet_ipa wrong loading behavior
kernel: hotspot: fix hotspot sleep to death
kernel: update Qualcomm snapdragon driver LA.UM.11.2.1.r1-04100-sdm660.0 - wifi/kernel
kernel: tune for optimization
kernel: update 4.19.288
device: add hub mode resources from Pixel Tablet
device: add Pixel Tablet stock wallpapers
device: add translation(RU, IT, ES, JA, EL) for cloverparts
device: correctly updated video/audio codec profile
device: differed 8 inch/10.1inch power profile(battery report value, doesn't matter but let's make it load diffrent for 8/10.1)
device: enable "Hub mode" entry
device: enable user switcher chip
device: fix adoptable storage(format sdcard as internal storage, no data loss after reboot now, but be careful for "PREWARNING" before doing OTA)
device: fix audio feature extension lib loading error(not user sensible)
device: fix IFAA(Mlipay) service, you may use Alipay with fingerprint(maybe, I can't test it), clover doesn't have soter firmware from MIUI modem(non-HLOS).img, so no soter for clover and no Wechat fingerprint payment
device: fix power profile for counting screen, audio, video battery usage
device: fix sim card background service fail and retry, fix ims service error, may fixed some lag, power drop and other sim card related issue
device: fix some unexpected SELinux denial(like qemu.hw.keys prop)
device: fix zram (write back) related kernel/selinux issue
device: hotspot: enable WPA3-Personal, WPA2/WPA3 option on hotspot(need the client not too old, normally just use WPA2 please)
device: hotspot: fix 2.4ghz hotspot doesn't have network on some old devices
device: hotspot: fix 5ghz wifi hotspot without clean flash
device: hotspot: increase wifi hotspot ap client limit to 32
device: implement QCOM WifiDisplay(improve performance, support mouse/keyboard input from remote, support passing audio to remote)
device: improve UI lagging
device: kill keyguard user switcher, enable Bouncer User Switcher
device: make Google Home built in following Pixel Tablet
device: project clean up, remove not needed system libs
device: reset lmk(Low Memory Killer) profile to apply AOSP default new strategy
device: solve 170M HDR type video decoding
device: tune status bar height, match status bar height for keyguard
device: universal wifi config optimization/upgrade
device: update GPU driver(OpenGL 3.2 @a61af92a49 - 2022/5/31, Vulkan 512.502.0 from Android 12 implementation)
device: update gpu firmware to lavender Android Q MIUI 12.5.7
device: update HUGE amount of qualcomm driver/service to Android 12 version(from Honeywell Hon660) and Android 13 version(LA.QSSI13), Can't write it down here, contains too much
device: update Qualcomm snapdragon driver LA.UM.11.2.1.r1-04100-sdm660.0 - audio
device: other minor fix and improvement
Upstream:
July security patch(Already an update of QPR3 June)
Fixed Google Assistant in landscape
Fixed app drawer icon color on launcher for "light theme"
Added Emoji wallpaper workshop(Update gapps from Play store and wait for a while then you will see)
Some preview UI for Android 14, eg. floating taskbar, new back gesture ui, new charging battery chip in status bar...
Source rebased
Updated gapps and translations
Performance and under the hood improvements

*2023.7.19*
>Device:
kernel: fix the HEVC 10bit
kernel: update Qualcomm driver(kernel, audio-kernel) to LA.UM.11.2.1.r1-04200-sdm660.0
kernel: add USB UAS support(you can mount movable harddisk now)
kernel: add bunch of HID device support
kernel: tuning UClamp scheduler values, better performance, power saving
device: update Qualcomm driver(display-commonsys) to LA.UM.11.2.1.r1-04200-sdm660.0
device: add spatial audio support(it's for wired headphone get better effect when playing supported media)
device: optimize the audio system performance
device: dexpreopt optimization(improve apps speed, get smoother), may need clean flash to take effect, clean flash and let it sleep for a while to complete the optimize process
Upstream:
Minor problem fixed

*2023.8.12/3*
>Device:
kernel: update to 4.19.289
device: add spatial audio for speaker
Upstream:
August Security Patch
Pixel Launcher/ASI drain fixes
Gapps Updated
Minor fixes and improvement

*2023.9.14*
>Device:
kernel: upstream 4.19.294
kernel: qualcomm driver update LA.UM.11.2.1.r1-04500-sdm660.0 (audio/kernel/wifi)
kernel: backport and enable Multigen-LRU
kernel: f2fs optimization from MIUI
kernel: arch arm64 optimization
device: qualcomm driver update LA.UM.11.2.1.r1-04500-sdm660.0 (display)
device: optimize uclamp app launch boost
device: optimize uclamp background process restriction
device: add French translation for cloverparts(thanks to pix106)
device: remove redundant zram setup procedure
Upstream:
Still August patch
Fix SystemUI HAL exception
Updated translations
Minor fix & minor upstream update

*2023.9.26*
>Device:
kernel: some lmk tuning
Upstream:
September security patch

*2023.10.18*
>Device:
kernel: update to 4.19.296
Upstream:
-N/A

==============================================

***History Plus Updates:***

*2023.2.10 - First release*
>-N/A

*2023.2.12*
>-N/A

*2023.2.18*
>-N/A

*2023.2.20*
>-N/A

*2023.2.24 - First OFFICIAL build*
>-N/A

*2023.2.27*
>-N/A

*2023.3.3*
>-N/A

*2023.3.24/5*
>-N/A

*2023.4.1*
>-N/A

*2023.4.19*
>-N/A

*2023.5.3*
>-N/A

*2023.5.7*
>emergency fix: 0503(PE Plus): headphone jack
emergency fix: 0503(PE Plus): camera video recording

*2023.5.19*
>-N/A

*2023.7.14*
>-N/A

*2023.7.19*
>-N/A

*2023.8.12/3*
>-N/A

*2023.9.14*
>-N/A

*2023.9.26*
>-N/A

*2023.10.18*
>-N/A

==============================================

***Archive Download:***
[[Archive]](https://www.androidfilehost.com/?w=files&flid=337493)