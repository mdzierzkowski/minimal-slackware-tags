**Minimal base**: this tagfiles provide a minimal usable installation of Slackware Linux including UEFI boot, kernel-huge, wired and wireless networking, but no Xorg. However there are some broken dependencies:

```
/usr/bin/floppyd from floppy
	missing libXau
	missing libX11
	missing libxcb
	missing libXdmcp
/usr/bin/gxditview and /usr/bin/xtotroff from groff
	missing libSM
	missing libICE
	missing libXaw
	missing libXmu
	missing libXt
	missing libXext
	missing libXpm
	missing libX11
/usr/bin/dbus-launch from dbus
	missing libSM
	missing libICE
	missing libX11
/usr/bin/wpa_gui from wpa_supplicant
	missing qt
	missing libXrender
	missing fontconfig
	missing freetype
	missing harfbuzz
qt pulled by wpa_supplicant
	missing libxslt
	missing libxml2
	missing glib2
	missing gstreamer
	missing gst-plugins-base
	missing sqlite
	missing mesa
	missing icu4c
	missing orc
	missing libxshmfence
	missing libXdamage
	missing libXfixes
	missing libXxf86vm
	missing libdrm
/usr/bin/gears and /usr/bin/glx* from mesa pulled by qt pulled by wpa_supplicant (:P)
	missing glew
	missing glu
	missing freeglut
	missing libXi
	missing libXrandr
xsltproc pulled by qt pulled by wpa_supplicant
	missing libgcrypt
	missing libgpg-error
harfbuzz pulled by wpa_supplicant
	missing cairo
cairo pulled by harfbuzz pulled by wpa_supplicant
	missing pixman
	missing lzo
```

floppy, groff, dbus, wpa_supplicant could be recompiled without Xorg/Qt support.

***Important:
There is no support for RAID, LVM, Luks and filesystems other then Ext4 by default.
To use generic kernel with initrd.gz a/mkinitrd has to be installed first.***

