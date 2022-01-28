# Awesome Switch Softmod

A collection of Nintendo Switch softmod resources.  
❔ = haven't tested it myself.

## Softmod tutorial

The one I personnally used is : https://nh-server.github.io/switch-guide/  
I know this one too : https://switch.homebrew.guide/  
Don't use video guides, they tend to not age well and be full of approximations. You can brick your switch with these. Prefer a well written guide that can be maintained up to date !

## Payloads & injectors

### [Atmosphere](https://github.com/Atmosphere-NX/Atmosphere)

The main software for the Switch softmod.  
Replace some part of the OS and allows patching others.  
Enables EmuMMC (a safe copy of the system on the SD card to leave no trace on the system itself).

### [Hekate](https://github.com/CTCaer/hekate)

A GUI Bootloader for the Switch.  
You can do a lot of things with this, like enabling AutoRCM, connect the Switch SD or internal storage as mass storage, create EmuMMC partition...

### [TegraRcmGUI](https://github.com/eliboa/TegraRcmGUI)

A Windows GUI for payload injection (for Atmosphere & Hekate).  
Allows auto-inject payload on Switch connection.

### Sigcheck patches

Allows you to launch unsigned software on switch.  
As this allows illegal things, I won't link to it directly, but you can find them on the "Temporary Game Boy Advance" forums.

## Updaters

### Daybreak

Included in Atmosphere, installs downloaded firmware from the SD.

### [AIO Switch Updater](https://github.com/HamletDuFromage/aio-switch-updater)

Updates Atmosphere, Sigpatches, downloads firmwares...

### [NightFall](https://github.com/D3fau4/NightFall) ⚠️ Crashed for me after download

Online updater for Atmosphere EmuMMC.  
As it crashed for me after the download, I recommend downloading with AIO Updater then installing it with Daybreak.

## Installers

### [Tinfoil](https://tinfoil.io/Download#download) ⚠️ Not open source !

This is an installer which has a nice feature called shops, which downloads games, DLC and updates directly from the switch.  
A shop I recommand (but won't link for obvious reasons) is "carcaschoi ultimate shop" which adds a selection of shops automatically.

### [TinWoo](https://github.com/mrdude2478/TinWoo)

A .nsp / .nsz / .xci / .xcz installer. An alternative to Awoo without anime NSFW.

### [AtmoXL-Titel-Installer](https://github.com/dezem/AtmoXL-Titel-Installer) ❔

Another fork of Awoo.

### [NS-USBLoader](https://github.com/developersu/ns-usbloader)

Use USB or WiFi to transfer files to TinWoo.

## Utilities

### [sys-ftpd-light](https://github.com/cathery/sys-ftpd-light) ❔

A background FTP server to do transfers on the SD card.

### [FTPd Pro](https://github.com/mtheall/ftpd)

A FTP server, but not background (.nro is the Switch release).

### [Emuiibo](https://github.com/XorTroll/emuiibo) ❔

An Amiibo emulator.  
You can create Amiibo on your computer, transfer them on the Switch and use them in games using an overlay.

### [Amiigo](https://github.com/CompSciOrBust/Amiigo) ❔

Same as Emuiibo computer part (Amiibo creation) but on the switch. Still requires Emuiibo.

### [MissionControl](https://github.com/ndeadly/MissionControl) ❔

Use non-Switch controllers directly on the switch with Bluetooth without adapters.

### [sys-hidplus](https://github.com/PaskaPinishkes/sys-hidplus)

Control the Switch from a computer.  
You can remote control your Switch using [Parsec](https://parsec.app/) with this (enabling remote multiplayer or remote play).  
Works surprisingly well, effortlessly and with low latency.  
I used the [sys-hidplus client](https://github.com/PaskaPinishkes/SwitchSysHidplusClient) on the computer after installing the sysmodule on the Switch.

### [pPlay](https://github.com/Cpasjuste/pplay) ❔

A media player (MPV port).

### [JKSV](https://github.com/J-D-K/JKSV)

A save manager (backup & restore game saves).

## Overlays


Using [nx-ovlloader](https://github.com/WerWolv/nx-ovlloader), you can have overlays for different utilities.  
You need to install [Tesla menu](https://github.com/WerWolv/Tesla-Menu) to switch between overlays.

You can have a list of available overlays there : https://github.com/n00mkrad/tesla-overlays-list

## Emulators

### [RetroArch](https://retroarch.com/?page=platforms)

A multi-system emulator.  
Probably the only one you will need as you can download cores for most consoles (NES / SNES / GB / GBA / DS / MS / Dreamcast / Arcade...).
