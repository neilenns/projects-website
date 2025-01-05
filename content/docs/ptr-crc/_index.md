---
title: CRC profile launcher for PowerToys Run
---

A [PowerToys Run](https://learn.microsoft.com/en-us/windows/powertoys/run) plugin for launching CRC profiles, useful
for VATSIM controllers.

## Usage

Type `crc` then select the profile you want to launch. To filter the list type a portion of the profile name.

![Animated GIF showing PowerToys Run launched, with "CRC" typed in, then a list of installed CRC profiles showing.](CrcLauncher.gif)

## Installation

The easiest way to install is with [ptr](https://github.com/8LWXpg/ptr):

```powershell
ptr add CrcLauncher neilenns/Community.PowerToys.Run.Plugin.CrcLauncher
```

Alternatively download the plugin from the [releases pages](https://github.com/neilenns/Community.PowerToys.Run.Plugin.CrcLauncher/releases/latest) then extract the zip into your `%localappdata%\Microsoft\PowerToys\PowerToys Run\Plugins` folder. If you are installing manually make sure to restart PowerToys after adding the plugin to the folder.
