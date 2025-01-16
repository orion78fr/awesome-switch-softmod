# Awesome Switch Softmod

A collection of Nintendo Switch softmod resources.  
❔ = haven't tested it myself.

## Softmod tutorial

The one I personnally used is : https://switch.hacks.guide/
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

### [Rekado](https://github.com/MenosGrante/Rekado)

Same, but for Android with USB c to c cable

### Sigcheck patches

Allows you to launch unsigned software on switch.  
As this allows illegal things, I won't link to it directly, but you can find them on the "Temporary Game Boy Advance" forums.

## Updaters

### Downloading updates from computer

I recommend this website : https://darthsternie.net/switch-firmwares/

### Daybreak

Included in Atmosphere, installs downloaded firmware from the SD.

### [AIO Switch Updater](https://github.com/HamletDuFromage/aio-switch-updater)

Updates Atmosphere, Sigpatches, downloads firmwares...

## Installers

### [Tinfoil](https://tinfoil.io/Download#download) ⚠️ Not open source !

This is an installer which has a nice feature called shops, which downloads games, DLC and updates directly from the switch.  
A shop I recommand (but won't link for obvious reasons) is "carcaschoi ultimate shop" which adds a selection of shops automatically.

### [Goldleaf](https://github.com/XorTroll/Goldleaf)

An NSP installer

### [Awoo](https://github.com/Huntereb/Awoo-Installer)

An NSP, NSZ, XCI, and XCZ Installer (supports more formats than Goldleaf but has anime NSFW on home page).

### [NS-USBLoader](https://github.com/developersu/ns-usbloader)

Use USB or WiFi to transfer files to Awoo.

## Utilities

### [sys-ftpd-light](https://github.com/cathery/sys-ftpd-light)

A background FTP server to do transfers on the SD card.  
Works great, but only one transfer in parallel is possible.  
Home button on joycon glows when a transfer is happening.  
Don't forget to set up user / password in `/config/sys-ftpd/config.ini` to disallow unauthenticated connections.

### [FTPd Pro](https://github.com/mtheall/ftpd)

A FTP server, but not background (.nro is the Switch release).

### [Emuiibo](https://github.com/XorTroll/emuiibo) ❔

An Amiibo emulator.  
You can create Amiibo on your computer, transfer them on the Switch and use them in games using an overlay.

### [Amiigo](https://github.com/CompSciOrBust/Amiigo) ❔

Same as Emuiibo computer part (Amiibo creation) but on the switch. Still requires Emuiibo.

### [MissionControl](https://github.com/ndeadly/MissionControl)

Use non-Switch controllers directly on the switch with Bluetooth without adapters.  
Tested it with an Xbox one X controller.

### [sys-hidplus](https://github.com/PaskaPinishkes/sys-hidplus)

Control the Switch from a computer.  
You can remote control your Switch using [Parsec](https://parsec.app/) with this (enabling remote multiplayer or remote play).  
Works surprisingly well, effortlessly and with low latency.  
I used the [sys-hidplus client](https://github.com/PaskaPinishkes/SwitchSysHidplusClient) on the computer after installing the sysmodule on the Switch.

### [pPlay](https://github.com/Cpasjuste/pplay) ❔

A media player (MPV port).

### [JKSV](https://github.com/J-D-K/JKSV)

A save manager (backup & restore game saves).

### [Edizon](https://github.com/WerWolv/EdiZon)

A save editor and cheat enabler. Has an overlay.  
If you plan on using cheats, remember to set `dmnt_cheats_enabled_by_default = u8!0x0` in `/atmosphere/system_settings.ini` to avoid enabling cheats by default but only via edizon.

## Overlays

Using [nx-ovlloader](https://github.com/WerWolv/nx-ovlloader), you can have overlays for different utilities.  
You need to install [Tesla menu](https://github.com/WerWolv/Tesla-Menu) to switch between overlays.

You can have a list of available overlays there : https://github.com/n00mkrad/tesla-overlays-list

To open them, you use `L + Dpad Down + Right Stick`.

## Emulators

### [RetroArch](https://retroarch.com/?page=platforms)

A multi-system emulator.  
Probably the only one you will need as you can download cores for most consoles (NES / SNES / GB / GBA / DS / MS / Dreamcast / Arcade...).
