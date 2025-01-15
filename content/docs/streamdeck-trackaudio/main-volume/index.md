---
title: Main volume
description: Controls app volume in TrackAudio with Stream Deck dials
og_image: ogimage/streamdeck-trackaudio.png
prev: /docs/streamdeck-trackaudio/hotline
next: /docs/streamdeck-trackaudio/push-to-talk
weight: 30
---

{{< get-button url="https://marketplace.elgato.com/product/trackaudio-e913a0ca-4c12-411d-a5a6-acf5f6c4bdea" title="Get from marketplace" >}}

The main volume action controls the volume for TrackAudio. You can use it to:

- Increase or decrease TrackAudio volume.
- See the current TrackAudio volume level.

This action requires a [Stream Deck with dial inputs](https://www.elgato.com/us/en/p/stream-deck-plus-black).

## Basic configuration

The main volume action does not require any configuration to use. Simply add it to your profile.

## States

{{<action-figures>}}
{{<action-figure src="trackaudio/main-volume/template.svg.html" state="connected" volume=90 title="Main volume" caption="Connected">}}
{{<action-figure src="trackaudio/main-volume/template.svg.html" state="notConnected" volume=90 title="Main volume" caption="Not connected">}}
{{</action-figures>}}

## Interactions

| Interaction  | Description           |
| ------------ | --------------------- |
| Rotate left  | Decreases the volume. |
| Rotate right | Increases the volume. |

### Settings reference

| Setting       | Description                                                               | Required? |
| ------------- | ------------------------------------------------------------------------- | :-------: |
| Title         | The title to show on the action.                                          |    No     |
| Change amount | The size of volume change to make on each click of the knob. Default `2`. |    Yes    |
| Connected     | The image to display when connected to TrackAudio.                        |    No     |
| Not connected | The image to display when not connected to TrackAudio.                    |    No     |

## SVG template variables

All state images support [SVG templates](../svg-templates/). The following variables are provided:

| Variable | Description                              |
| -------- | ---------------------------------------- |
| volume   | The current station volume, from 0-100.  |
| state    | The name for the action's current state. |

The state names are:

- connected
- notConnected
