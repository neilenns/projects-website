---
title: vATIS status
description: Displays connection status to vATIS on Stream Deck keys
prev: /docs/streamdeck-vatis/atis-letter
og_image: ogimage/streamdeck-vatis.png
---

{{< get-button url="https://marketplace.elgato.com/product/vatis-878fcd1a-7e0a-4d6e-bd36-c70b075573ea" title="Get from marketplace" >}}

The vATIS status action shows the state of the connection to the vATIS application. You can use it to:

- Verify your Stream Deck is connected to vATIS
- Force all vATIS actions to refresh their state

## Basic configuration

This action does not require any configuration to use.

## States

{{<action-figures>}}

<!-- Not connected -->

{{< action-figure src="vatis/vatis-status/template.svg.html" isConnected="false" caption="Not connected to vATIS" >}}

{{< action-figure src="vatis/vatis-status/template.svg.html" isConnected="true" caption="Connected to vATIS" >}}

{{</action-figures>}}

## Interactions

| Interaction | Description                        |
| ----------- | ---------------------------------- |
| Long press  | Refreshes all ATIS letter actions. |

## Settings reference

| Setting       | Description                                       | Required? |
| ------------- | ------------------------------------------------- | :-------: |
| Title         | The title to show on the action.                  |    No     |
| Connected     | The image to display when connected to vATIS.     |    No     |
| Not connected | The image to display when not connected to vATIS. |    No     |

## SVG template variables

All state images support [SVG templates](../svg-templates/). The following variables are provided:

| Variable    | Description                                 |
| ----------- | ------------------------------------------- |
| isConnected | True if the actions are connected to vATIS. |
| title       | The title specified by the user.            |
