
Debian
====================
This directory contains files used to package cobaltcashd/cobaltcash-qt
for Debian-based Linux systems. If you compile cobaltcashd/cobaltcash-qt yourself, there are some useful files here.

## cobaltcash: URI support ##


cobaltcash-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install cobaltcash-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your cobaltcashqt binary to `/usr/bin`
and the `../../share/pixmaps/cobaltcash128.png` to `/usr/share/pixmaps`

cobaltcash-qt.protocol (KDE)

