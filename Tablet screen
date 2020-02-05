#Xorg config
* Screen rotation to match orientation with the keyboard connected
`sudo vi /etc/X11/xorg.conf.d/30-display.conf`
Section "Monitor"
  Identifier    "DSI1"
  Option        "Rotate"                 "left"
EndSection

* Touchscreen
`sudo vi /etc/X11/xorg.conf.d/99-touchscreen.conf`
Section "InputClass"
  Identifier    "calibration"
  MatchProduct  "Goodix Capacitive TouchScreen"
  Option        "TransformationMatrix"   "0 1 0 -1 0 1 0 0 1"
EndSection

* Video card option
`sudo vi /etc/X11/xorg.conf.d/20-intel.conf`
Section "Device"
  Identifier    "Intel Graphics"
  Driver        "intel"
  Option        "AccelMethod"            "sna"
  Option        "TearFree"               "true"
  Option        "DRI"                    "3"
EndSection
