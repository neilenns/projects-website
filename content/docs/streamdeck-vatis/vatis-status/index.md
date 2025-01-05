---
title: vATIS status
prev: /docs/streamdeck-vatis/atis-letter
---

The vATIS status action shows the state of the connection to the vATIS application. You can use it to:

- Verify your Stream Deck is connected to vATIS
- Force all vATIS actions to refresh their state

## Basic configuration

This action does not require any configuration to use.

## States

{{<action-figures>}}

<!-- Not connected -->

{{< action-figure src="vatis-status/template.svg.html" isConnected="false" caption="Not connected to vATIS" >}}

{{< action-figure src="vatis-status/template.svg.html" isConnected="true" caption="Connected to vATIS" >}}

{{</action-figures>}}

## Interactions

The action supports long press.

| Interaction | Description                        |
| ----------- | ---------------------------------- |
| Long press  | Refreshes all ATIS letter actions. |

## Settings reference

| Setting       | Description                                             | Required? |
| ------------- | ------------------------------------------------------- | :-------: |
| Title         | The title to show on the action. Optional.              |    No     |
| Connected     | The image to display when connected to vATIS. Optional. |    No     |
| Not connected | The image to display when not connected to vATIS.       |    No     |
