---
title: vATIS profile launcher for PowerToys Run
---

> [!IMPORTANT]
> This plugin requires [vATIS version v4.1.0-beta.3 or later](https://vatis.app/) and
> [Microsoft PowerToys version v0.87.0 or later](https://github.com/microsoft/PowerToys/releases/latest).

A [PowerToys Run](https://learn.microsoft.com/en-us/windows/powertoys/run) plugin for launching vATIS profiles, useful
for VATSIM controllers.

## Usage

Type `va` then select the profile you want to launch. To filter the list type a portion of the profile name.

![Animated GIF showing PowerToys Run launched, with "va" typed in, then a list of installed vATIS profiles showing.](launcher.gif)

## Installation

The easiest way to install is with [ptr](https://github.com/8LWXpg/ptr):

```powershell
ptr add vAtisLauncher neilenns/Community.PowerToys.Run.Plugin.vAtisLauncher
```

Alternatively download the plugin from the [releases pages](https://github.com/neilenns/Community.PowerToys.Run.Plugin.vAtisLauncher/releases/latest) then extract the zip into your `%localappdata%\Microsoft\PowerToys\PowerToys Run\Plugins` folder. If you are installing manually make sure to restart PowerToys after adding the plugin to the folder.
