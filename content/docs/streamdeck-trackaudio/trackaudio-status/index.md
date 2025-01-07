---
title: TrackAudio status
description: Displays connection status to TrackAudio on Stream Deck keys
og_image: ogimage/streamdeck-trackaudio.png
prev: /docs/streamdeck-trackaudio/station-volume
next: /docs/streamdeck-trackaudio/examples
weight: 70
---

{{< get-button url="https://marketplace.elgato.com/product/trackaudio-e913a0ca-4c12-411d-a5a6-acf5f6c4bdea" title="Get from marketplace" >}}

The TrackAudio status action shows the status of the connection between Stream Deck and TrackAudio. You can use it to:

- Verify your Stream Deck is connected to TrackAudio
- Verify you are connected to the VATSIM audio network
- Force all TrackAudio actions to refresh their state

## Basic configuration

This action does not require any configuration to use.

## States

{{<action-figures>}}

{{<action-figure src="trackaudio/trackaudio-status/template.svg.html" state="connected" caption="Connected">}}

{{<action-figure src="trackaudio/trackaudio-status/template.svg.html" state="notConnected" caption="Not connected">}}

{{<action-figure src="trackaudio/trackaudio-status/template.svg.html" state="voiceConnected" caption="Voice connected">}}

{{</action-figures>}}

## Interactions

| Interaction | Description                       |
| ----------- | --------------------------------- |
| Long press  | Refreshes all TrackAudio actions. |

### Settings reference

| Setting         | Description                                                          | Required? |
| --------------- | -------------------------------------------------------------------- | :-------: |
| Connected       | The image to display when connected to TrackAudio.                   |    No     |
| Not connected   | The image to display when not connected to TrackAudio.               |    No     |
| Voice connected | The image to display when the TrackAudio voice connection is active. |    Yes    |
| Show title      | Show the title on the action. Default `off`.                         |    Yes    |

## SVG template variables

All state images support [SVG templates](../svg-templates/). The following variables are provided:

| Variable | Description                              |
| -------- | ---------------------------------------- |
| state    | The name for the action's current state. |
| title    | The title specified by the user.         |

The state names are:

- connected
- notConnected
- voiceConnected
