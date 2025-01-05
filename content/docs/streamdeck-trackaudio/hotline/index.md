---
title: Hotline
prev: /docs/streamdeck-trackaudio/atis-letter
next: /docs/streamdeck-trackaudio/push-to-talk
weight: 20
---

The hotline action provides a quick way to toggle between two stations for voice transmissions. This is typically
used by center controllers who have a hotline frequency established with neighbouring sectors.
It also automatically adds the primary and hotline stations to TrackAudio after a voice connection is established.

To use the hotline action start by adding the appropriate stations to TrackAudio. Your primary station should
be added with `XCA` enabled and the hotline station should be added with `RX` enabled. Then configure the
hotline action with the primary and hotline station callsigns.

Once configured, pressing the action will toggle `TX` active between your primary and hotline frequencies.
A long press of the action will refresh the action's state.

### Hotline action settings <!-- omit from toc -->

| Setting               | Description                                                                                                                                                                                                  | Default                                                 |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------- |
| Primary callsign      | The callsign you are actively controlling, for example `SEA_CTR`. Required.                                                                                                                                  |                                                         |
| Hotline callsign      | The callsign for the hotline, for example `ZOA-ZSE`. Required.                                                                                                                                               |                                                         |
| Both active           | The image to display when both the primary and hotline and frequencies are the active frequency. This should never happen, as it means your voice transmissions will get sent to both frequencies. Optional. | ![Handset with red background](hotline-both.png)        |
| Hotline active        | The image to display when transmitting on the hotline frequency. Optional.                                                                                                                                   | ![Handset with orange background](hotline-active.png)   |
| Listening             | The image to display when listening to the hotline frequency. Optional.                                                                                                                                      | ![Handset with blue background](hotline-listening.png)  |
| Neither active        | The iamge to display when neither the primary nor the hotline frequencies have TX enabled. Optional.                                                                                                         | ![Handset with black background](hotline-neither.png)   |
| Receiving             | The image to display when receiving a transmission on the hotline frequency. Optional.                                                                                                                       | ![Handset with green background](hotline-receiving.png) |
| Unavailable           | The image to display when the primary and hotline stations are not added in TrackAudio. Optional.                                                                                                            | ![Warning icon](hotline-unavailable.png)                |
| Show hotline callsign | Show the hotline callsign on the action.                                                                                                                                                                     | false                                                   |
| Show primary callsign | Show the primary callsign on the action.                                                                                                                                                                     | false                                                   |
| Show title            | Show the title on the action.                                                                                                                                                                                | true                                                    |
