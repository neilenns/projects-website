---
title: ATIS letter
description: Displays the current ATIS letter for a station from VATSIM on Stream Deck keys
next: /docs/streamdeck-trackaudio/hotline
weight: 10
---

> [!IMPORTANT]
> If you are actively controlling with [vATIS](https://vatis.app/) use the [vATIS actions for Stream Deck plugin](https://github.com/neilenns/streamdeck-vatis) instead to get
> real-time ATIS updates on your Stream Deck.
>
> For this action to work TrackAudio must be running and you must be connected for the ATIS letter to update.
> It can take five minutes or longer for the VATSIM data source to refresh and reflect the latest ATIS letter.

The ATIS letter action shows the current ATIS letter for a station, refreshed automatically every minute.
When the ATIS letter updates the action will show an orange background until the action is pressed to reset the
state. A long press of the action will force a refresh of the ATIS information.

See the [SVG template documentation](https://github.com/neilenns/streamdeck-trackaudio/wiki/SVG-templates) for an example
template that shows the title small and station letter big.

### ATIS letter action settings <!-- omit from toc -->

| Setting                     | Description                                                                                                               | Default                                |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------- | -------------------------------------- |
| Title                       | The title to show on the action. The current ATIS letter will be appended to this title separated by a newline. Optional. | Blank                                  |
| Callsign                    | The callsign to get the current AITS letter for, for example `KSEA_ATIS`. Required.                                       |                                        |
| Current                     | The image to display when the ATIS letter shown is current. Optional.                                                     | ![Black background](atis-current.png)  |
| Unavailable                 | The image to display when no ATIS letter is available. Optional.                                                          | ![Warning icon](atis-unavailable.png)  |
| Updated                     | The image to display when the ATIS letter updated to a new one. Optional.                                                 | ![Orange background](atis-updated.png) |
| Automatically clear updates | Clears the updated state automatically after two minutes. Pressing the action will always clear the update state.         | true                                   |
| Show letter                 | Show the letter on thea ction.                                                                                            | true                                   |
| Show title                  | Show the title on the action.                                                                                             | true                                   |
