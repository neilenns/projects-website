---
title: Station volume
description: Controls station volume in TrackAudio with Stream Deck dials
og_image: ogimage/streamdeck-trackaudio.png
prev: /docs/streamdeck-trackaudio/station-status
next: /docs/streamdeck-trackaudio/trackaudio-status
weight: 60
---

{{< get-button url="https://marketplace.elgato.com/product/trackaudio-e913a0ca-4c12-411d-a5a6-acf5f6c4bdea" title="Get from marketplace" >}}

The station volume action controls the volume for a specific station. You can use it to:

- Increase or decrease the volume of a station.
- Toggle mute on a station.
- See the current volume level of a station.

This action requires a [Stream Deck with dial inputs](https://www.elgato.com/us/en/p/stream-deck-plus-black).

## Basic configuration

The station volume action does not require any configuration to use. Simply add it to your profile, then use the dial to adjust the station volume.

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

| Setting       | Description                                                                            | Required? |
| ------------- | -------------------------------------------------------------------------------------- | :-------: |
| Callsign      | The callsign for the station you want to control the volume of, for example `PDX_TWR`. |    Yes    |
| Change amount | The size of volume change to make on each click of the knob. Default `1`.              |    Yes    |
| Muted         | The image to display when the station is muted in TrackAudio.                          |    No     |
| Not muted     | The image to display when the station is not muted in TrackAudio.                      |    No     |
| Unavailable   | The image to display when the station is not added in TrackAudio.                      |    No     |
