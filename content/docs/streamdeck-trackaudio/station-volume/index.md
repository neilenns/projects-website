---
title: Station volume
description: Controls station volume in TrackAudio with Stream Deck dials
og_image: ogimage/streamdeck-trackaudio.png
prev: /docs/streamdeck-trackaudio/station-status
next: /docs/streamdeck-trackaudio/trackaudio-status
weight: 60
---

{{< get-button url="https://marketplace.elgato.com/product/trackaudio-e913a0ca-4c12-411d-a5a6-acf5f6c4bdea" title="Get from marketplace" >}}

> [!NOTE]
> This action is coming soon!

The station volume action controls the volume for a specific station. You can use it to:

- Increase or decrease the volume of a station.
- Toggle mute on a station.
- See the current volume level of a station.

This action requires a [Stream Deck with dial inputs](https://www.elgato.com/us/en/p/stream-deck-plus-black).

## Basic configuration

To configure the action to control the volume for a specific station configure the following settings:

| Setting  | Value                                                           | Example     |
| -------- | --------------------------------------------------------------- | ----------- |
| Callsign | The callsign for the station you want to control the volume of. | `PDX_O_TWR` |

## Configuring a station volume action

The station volume action displays the current volume of a specific station and enables changing the volume, as well as muting
the station. This action requires a dial control, available on the [Stream Deck +](https://www.elgato.com/us/en/p/stream-deck-plus-black).

## States

{{<action-figures>}}

{{<action-figure src="trackaudio/station-volume/template.svg.html" state="muted" title="GND" volume=30 caption="Muted">}}

{{<action-figure src="trackaudio/station-volume/template.svg.html" state="notMuted" title="GND" volume=30 caption="Not muted">}}

{{<action-figure src="trackaudio/station-volume/template.svg.html" state="unavailable" title="GND" volume=30 caption="Unavailable">}}

{{</action-figures>}}

## Interactions

| Interaction  | Description           |
| ------------ | --------------------- |
| Rotate left  | Decreases the volume. |
| Rotate right | Increases the volume. |
| Short press  | Toggles mute.         |
| Tap          | Toggles mute.         |

### Settings reference

| Setting       | Description                                                                              | Required? |
| ------------- | ---------------------------------------------------------------------------------------- | :-------: |
| Callsign      | The callsign for the station you want to control the volume of, for example `PDX_O_TWR`. |    Yes    |
| Change amount | The size of volume change to make on each click of the knob. Default `1`.                |    Yes    |
| Muted         | The image to display when the station is muted in TrackAudio.                            |    No     |
| Not muted     | The image to display when the station is not muted in TrackAudio.                        |    No     |
| Unavailable   | The image to display when the station is not added in TrackAudio.                        |    No     |

## SVG template variables

All state images support [SVG templates](../svg-templates/). The following variables are provided:

| Variable | Description                              |
| -------- | ---------------------------------------- |
| volume   | The current station volume, from 0-100.  |
| state    | The name for the action's current state. |

The state names are:

- unavailable
- muted
- notMuted
