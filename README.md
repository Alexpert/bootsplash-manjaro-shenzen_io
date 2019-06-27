# Manjaro-bootsplash-arch
Kernel Bootsplash theme for manjaro Linux using Shenzen I/O loading screen logo

# Installation:

- `cd manjaro-bootsplash-shenzen_io`
- run `bootsplash-manjaro-shenzen_io.sh` to generate STL model.
- run `makepkg` to create Arch package and install it with `pacman -U $package_name`
- append `bootsplash-manjaro-shenzen_io` hook in the end of HOOKS string of `/etc/mkinitcpio.conf`
- add `bootsplash.bootfile=bootsplash-themes/manjaro-shenzen_io/bootsplash` into `GRUB_CMDLINE_LINUX` string in `/etc/default/grub`
- run `sudo mkinitcpio -P`
- run `sudo update-grub`

# Nota Bene

- This is a modified version of: https://github.com/Blacksuan19/Bootsplash-Themes/tree/master/manjaro-bootsplash-arch
- The logo comes from the game Shenzen I/O developped by Zachtronics: http://www.zachtronics.com/shenzhen-io/
