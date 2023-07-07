# Burhan Build of DWM

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

- [Full Gaps](https://dwm.suckless.org/patches/fullgaps/) - This patch adds gaps between client windows
- [Status2d](https://dwm.suckless.org/patches/status2d/) - Status2d allows colors and rectangle drawing in your DWM status bar
- [xrdb](https://dwm.suckless.org/patches/xrdb/) - Allows dwm to read colors from xrdb (.Xresources) at run time.
- [Fakefullscreen](https://dwm.suckless.org/patches/fakefullscreen/) - Only allow clients to "fullscreen" into space currently given to them
- [Bottomstack](https://dwm.suckless.org/patches/bottomstack/) - Bstack and bstackhoriz are two stack layouts for dwm.
- [Cyclelayouts](https://dwm.suckless.org/patches/cyclelayouts/) - This adds a "NULL, NULL" layout at the end of the list, which should always be the last layout in your list.
- [Movestack](https://dwm.suckless.org/patches/movestack/) - This plugin allows you to move clients around in the stack and swap them with the master
- [Pertag](https://dwm.suckless.org/patches/pertag/) - This patch keeps layout, mwfact, barpos and nmaster per tag.
