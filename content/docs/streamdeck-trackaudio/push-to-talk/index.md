---
title: Push to talk
description: Triggers push to talk in TrackAudio with Stream Deck keys
og_image: ogimage/streamdeck-trackaudio.png
prev: /docs/streamdeck-trackaudio/main-volume
next: /docs/streamdeck-trackaudio/station-status
weight: 40
---

{{< get-button url="https://marketplace.elgato.com/product/trackaudio-e913a0ca-4c12-411d-a5a6-acf5f6c4bdea" title="Get from marketplace" >}}

The push to talk action triggers the transmit function in TrackAudio. You can use it to:

- Start transmission using a Stream Deck key
- See when you are transmitting

## Basic configuration

The push to talk action does not require any configuration to use. Simply add it to your profile, then press the key to start transmitting.

## States

{{<action-figures>}}

<!-- not transmitting -->

{{<action-figure src="trackaudio/push-to-talk/template.svg.html" state="notTransmitting" caption="Not transmitting">}}

<!-- transmitting -->

{{<action-figure src="trackaudio/push-to-talk/template.svg.html" state="transmitting" title="KPDX" caption="Transmitting">}}

{{</action-figures>}}

## Interactions

| Interaction    | Description                          |
| -------------- | ------------------------------------ |
| Press and hold | Transmits as long as the key is held |

## Settings reference

| Setting          | Description                                 | Required |
| ---------------- | ------------------------------------------- | -------- |
| Title            | The title to show on the action. No         |          |
| Not transmitting | Shown when idle. Optional.                  | No       |
| Transmitting     | Shown when actively transmitting. Optional. | No       |
| Show title       | Show the title on the action.               | No       |
