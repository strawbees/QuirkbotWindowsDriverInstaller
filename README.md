# Quirkbot Windows Drivers Installer

Quirkbot board requires a driver for Windows 7 and 8.1. This repository contains the driver files and source to build an installer/wizard to install those drivers.

## Build instructions (Windows)

- Downdload and install [NSIS](http://nsis.sourceforge.net/Download) (verison `3.0b3`).
- Install [NSIS UAC Plugin](https://nsis.sourceforge.io/UAC_plug-in):
    - [Download zip with source files](https://nsis.sourceforge.io/mediawiki/images/8/8f/UAC.zip) or the `UAC.zip` file contained in this repo.
    - Extract `UAC.zip\Plugins\x86-ansi\UAC.dll` to `C:\Program Files\NSIS\Plugins\x86-ansi\UAC.dll`
    - Extract `UAC.zip\Plugins\x86-unicode\UAC.dll` to `C:\Program Files\NSIS\Plugins\x86-unicode\UAC.dll`
    - Extract `UAC.zip\UAC.nsh` to `C:\Program Files\NSIS\Includes\UAC.sh`
- Right click `build.nsi` and select `Compile Script` or run `makensis build.nsi`.
- Wait for `Quirkbot-Windows-Drivers-Installer.exe` to be generated.
