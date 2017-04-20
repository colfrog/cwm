This is a fork of OpenBSD's cwm[0] to Linux and other Unices by Leah Neukirchen (https://github.com/chneukirchen).
I added some features and I'm trying to keep it updated.

    cwm is a window manager for X11 which contains many features that
    concentrate on the efficiency and transparency of window
    management.  cwm also aims to maintain the simplest and most
    pleasant aesthetic.

This fork changed the config file to ~/.config/cwm/cwmrc and added an autoexec file in the same directory
that is executed at start. It also adds an XSession desktop file and a few features.

## New Features
Among these features are:

    * Grid/Manual tiling support taken from github.com/TaylanTatli/cwm-mod

    * Resizing with the mouse while keeping aspect ratio

    * Resizing with the keyboard while keeping aspect ratio

## BUILDING
This window manager requires the following packages and their development headers to build:

    * pkg-config

    * bison or a compatible yacc implementation

    * (lib)Xft

    * (lib)Xrandr

    * (lib)Xinerama (only required for multi-monitor support, can probably work without

    * BSD Make or GNU Make

It has been built succesfully on OpenBSD, NetBSD, FreeBSD, macOS 10.12 and Linux.
This version is also compatible with musl.

[0]: http://cvsweb.openbsd.org/cgi-bin/cvsweb/xenocara/app/cwm/
