**Base Xorg**: this tagfiles provide a minimal usable installation of Slackware Linux including UEFI boot, kernel-huge, wired and wireless networking, with Xorg. However there are some broken dependencies:

```
/usr/lib64/qt/bin/assistant from qt
missing l/libxslt
missing l/glib2
missing l/gstreamer
missing l/gst-plugins-base
missing ap/sqlite
```

***Important:
There is no support for RAID, LVM, Luks and filesystems other then Ext4 by default.
To use generic kernel with initrd.gz a/mkinitrd has to be installed first.***

