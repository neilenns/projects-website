---
title: Discord timestamp generator for PowerToys Run
---

A [PowerToys Run](https://learn.microsoft.com/en-us/windows/powertoys/run) plugin for generating Discord timestamps,
inspired by the amazing [Discord Timestamp](https://discordtimestamp.com/) website.

## Usage

Type `dt` followed by a date and/or time. Dates and times can be specified in [wide range of natural
language forms](https://github.com/mojombo/chronic?tab=readme-ov-file#examples). Select the desired Discord
timestamp format from the resulting list then paste it into Discord.

![Animated GIF of the plugin showing results for "in 5 minutes"](DiscordTimestamp.gif)

The result when pasted into Discord:

![Screenshot of Discord with a sent message containing the text "Let's play some disc golf! Meet outside in 5 minutes?". The "in 5 minutes" text is a live-updating time based on the timestamp pasted in.](discord-example.png)

## Installation

The easiest way to install is with [ptr](https://github.com/8LWXpg/ptr):

```powershell
ptr add DiscordTimestamp neilenns/Community.PowerToys.Run.Plugin.DiscordTimestamp
```

Alternatively download and extract the plugin from the [releases pages](https://github.com/neilenns/Community.PowerToys.Run.Plugin.DiscordTimestamp/releases/latest) then extract the zip into a folder called `DiscordTimestamp` in your `%localappdata%\Microsoft\PowerToys\PowerToys Run\Plugins` folder. If you are installing manually make sure to restart PowerToys after adding the plugin to the folder.
