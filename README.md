![Minimal Slackware logo](/mix/slackware_minimal.png "Minimal Slackware logo")

## Minimal Slackware 

**Tagfiles and list of packages for minimal installation of Slackware Linux 14.2**

### Why?
I like the idea of a minimal system with only the software I need, something like FreeBSD's *base* with some programs form ports. In default istallation of a **Slackware Linux** there are 8 (eight) console text editors (some of them have no release for almost 10 years), 4 console mail clients, etc. If I don't use them why install them?

Note that this is not a hardcore minimal set of packages. My goal is to provide a minimal **usable** installation. Having no network is not usable for most cases. 

### Contnet
+ **Base**: this tagfiles provide a minimal usable installation of Slackware Linux including UEFI boot, kernel-huge, wired and wireless networking, *but no Xorg*. 
+ **Base Xorg**: same as **Base**, but with Xorg.
+ **Slackware tags**: set of tagfiles form Slackware 14.2 iso image.

*Important: There is no support for RAID, LVM, Luks and filesystems other then Ext4 by default. To use generic kernel with initrd.gz a/mkinitrd has to be installed first.*

### FAQ
Q: How to install `slackpkg`?
A: `installpkg which wget ncurses gnupg dialog slackpkg`

#### Disclaimer

"Minimal Slackware" is not affiliated with or officially endorsed by either Patrick Volkerding or Slackware Linux, Inc.

Slackware® is a registered trademark of Slackware Linux, Inc.
