Backup of [upd72020x-fw](https://aur.archlinux.org/packages/upd72020x-fw) from [AUR](https://aur.archlinux.org).
This is a fork from [upd72020x-fw](https://aur.archlinux.org/packages/upd72020x-fw),
due to as of **May 13 2025** the [upd72020x-fw](https://aur.archlinux.org/packages/upd72020x-fw)
is missing a file [uPD72020x-Firmware-1.0.0.tar.gz](https://github.com/nothingHereReally/upd72020x-fw-bk/blob/master/uPD72020x-Firmware-1.0.0.tar.gz).
Due to it has a dependency to this [repo](https://github.com/denisandroid/uPD72020x-Firmware) which just shows Page Not Found
and seems to be deleted by the owner of that [repo](https://github.com/denisandroid/uPD72020x-Firmware)


This is the xhci_pci firmware, this has mainly been tested( works on Arch GNU/Linux)
on Arch GNU/Linux, I don't know if this works for other GNU/Linux distro.
This package solves the problem of `==> WARNING: Possibly missing firmware for module: 'xhci_pci'`
or `==> WARNING: Possibly missing firmware for module: 'xhci_pci_renesas'`
for more info see the [missing firmware on Arch Wiki](https://wiki.archlinux.org/title/Mkinitcpio#Possibly_missing_firmware_for_module_XXXX).


To install this on Arch GNU/Linux run
```bash
git clone https://github.com/nothingHereReally/upd72020x-fw-bk.git
cd upd72020x-fw-bk
makepkg -si
```


If the [upd72020x-fw](https://aur.archlinux.org/packages/upd72020x-fw) package
from the [AUR](https://aur.archlinux.org) is fixed, please use [that](https://aur.archlinux.org/packages/upd72020x-fw)
instead of [this](https://github.com/nothingHereReally/upd72020x-fw-bk).
Due to when [this](https://github.com/nothingHereReally/upd72020x-fw-bk)
package is installed it will be named as `upd72020x-fw` which would be
in conflict with [upd72020x-fw](https://aur.archlinux.org/packages/upd72020x-fw).
So on pacman, just to check that would be
```bash
pacman -Qs upd72020x-fw
```


The [upd-firmware tar file here](https://github.com/nothingHereReally/upd72020x-fw-bk/blob/master/uPD72020x-Firmware-1.0.0.tar.gz)
passes the SHA512 hash from the [.SRCINFO](https://github.com/nothingHereReally/upd72020x-fw-bk/blob/master/.SRCINFO)
and [PKGBUILD](https://github.com/nothingHereReally/upd72020x-fw-bk/blob/master/PKGBUILD) which is
`9d7e61c99a0f46d0ae96505317e763a468d3e8006f7398d10899ab78532b1ace608662b8a1b410a5577b268dc1f9275d1ebe3d03d209b85b2c4307ceb48dd261`
feel free to check the hash yourself.
To check that would be
```bash
sha512sum uPD72020x-Firmware-1.0.0.tar.gz
```

