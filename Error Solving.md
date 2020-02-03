**In this file I describe the error reported by log files and how I solved them**

**/var/log/kernel.log**

* [drm:mipi_exec_pmic [i915]] *ERROR* Your hardware requires CONFIG_PMIC_OPREGION and it is not set
* Audio Port: ASoC: no backend DAIs enabled for Audio Port
* silead_ts i2c-MSSL1680:00: Direct firmware load for silead/mssl1680.fw failed with error -2
silead_ts i2c-MSSL1680:00: Firmware request error -2
silead_ts: probe of i2c-MSSL1680:00 failed with error -2
* silead_ts i2c-MSSL1680:00: i2c-MSSL1680:00 supply vddio not found, using dummy regulator
* [    8.896056] usb 1-4.4.2: Warning! Unlikely big volume range (=511), cval->res is probably wrong.
[    8.896063] usb 1-4.4.2: [15] FU [Targus Audio Playback Volume] ch = 2, val = -8176/0/16
[    8.896880] usb 1-4.4.2: Warning! Unlikely big volume range (=767), cval->res is probably wrong.
[    8.896885] usb 1-4.4.2: [12] FU [Mic Capture Volume] ch = 2, val = -4592/7680/16
* mmc2: error -84 whilst initialising SD card
mmc2: error -110 whilst initialising SD card
