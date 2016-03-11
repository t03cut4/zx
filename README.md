# zx
i3 scratchpad manager

# About zx
zx creates a taskbar like window on the bottom of the screen to show you windows which have been minimized (sent to scratchpad). You can easily reopen them in any workspace you like.

TODO: Add screenshots

# Status
This is fully working, very little tested.

# Requirements
* i3ipc-glib
* glib
* libxcb

# Installation
Install the requirements then run `make` then `sudo make install`

You can run this from your i3 config to run on startup

# Config
You can configure zx with a config file in ~/.zxconfig

Example config file:
```
[zx]
background=0x2C3E50
border_color=0x7F8C8D
border=1
floating=0
font_color=0xFFFFFF
```

Config explanation
```
background (unsigned long / hex) - background color (ex. 0x000000)
border_color (unsigned long / hex) - border color (border around each window entry) (ex. 0xFFFFFF)
border (int) - enable/disable border
floating (int) - should windows opened from zx float or not
font_color (unsigned long / hex) - font color (ex. 0xFFFFFF)
```
