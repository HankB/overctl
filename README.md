# overctl

Shell script to enable/disable OverlayFS for Raspberry Pi OS

Inspired by (and with permission of) Mattias Wikstrom who posted the starting point at [Raspberry Pi Overlay Root Filesystem](https://yagrebu.net/unix/rpi-overlay.md) Mattias wishes to credit Rawspberry Pi Forum user ejolson for their help as well.

This is intended to duplicate the functionality found in `raspi-config` but scriptable and with some enhancements and to fully automate the process from the source instructions. The eventual purpose is to use it to update Raspberry Pis using Ansible and which employ the overlayfs.

## Research

Since I created this repo I have found a bunch of other references for scripts that do this. Included in that was the helpful information that `raspi-config` is coded as a shell script and that the procedures that perform this operation can be called from other shell scripts. In fact, `raspi-config` has a `nonint` option that should be scriptable. Here is what I've found so far:

1. https://yagrebu.net/unix/rpi-overlay.md
1. https://github.com/JasperE84/root-ro
1. https://www.domoticz.com/wiki/Setting_up_overlayFS_on_Raspberry_Pi
1. https://raspberrypi.stackexchange.com/questions/124628/raspbian-enable-disable-overlayfs-from-terminal
1. https://forums.raspberrypi.com/viewtopic.php?p=1986514&hilit=overlay+file+system#p1986514
1. https://loganmarchione.com/2021/07/raspi-configs-mostly-undocumented-non-interactive-mode/
1. https://forums.raspberrypi.com/viewtopic.php?t=21632

The current focus therefore is to survey the field to see whgat is available and either use that or perhaps fork something or combine the best aspects of any of them.

## Contributing

I really appreciate any and all help I can get with this. That includes things like pointing out typos, spelling and grammar errors, unclear descriptions up to including help with the script(s), walk throughs, coding critique and so on. Nevertheless, I reserve the right to reject any PRs that I don't feel contribute to the direction I want to take this project. I'm conflicted about asking for copyright assignment. I've heard other projects that got into difficulty because they didn't do that and then could not make changes (licensing) without getting the permission of all contributors. OTOH I hope to leverage a lot of other code and I don't think this is going to be that significant a project. Not asking for that right now. And I will be more than happy to credit all who contribute.
