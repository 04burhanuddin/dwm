# DWM - Dynamic Window Manager
>
> version 6.4

DWM is an extremely fast, small, and Dynamic Window Manager for X. from [suckless.org](https://dwm.suckless.org/)

## Installation

    git clone https://github.com/04burhanuddin/dwm.git
    cd dwm
    sudo make install

## Running dwm

In order to display status info in the bar, you can do something
like this in your .xinitrc:

    while xsetroot -name "`date` `uptime | sed 's/.*,//'`"
    do
     sleep 1
    done &
    exec dwm

## Patches and Features

- You can modify key bindings in the ``config.h``
- [Full Gaps](https://dwm.suckless.org/patches/fullgaps/) - This patch adds gaps between client windows
- [Status2d](https://dwm.suckless.org/patches/status2d/) - Status2d allows colors and rectangle drawing in your DWM status bar
- [xrdb](https://dwm.suckless.org/patches/xrdb/) - Allows dwm to read colors from xrdb (.Xresources) at run time.
- You can add patches as needed. [How To Patch ?](https://suckless.org/hacking/)
