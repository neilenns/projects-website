---
title: SVG templates
description: Information on how to use SVG templates with TrackAudio actions
og_image: ogimage/streamdeck-vatis.png
---

All image properties on all actions support using SVG templates instead of a standard SVG image. The templates use [Handlebars](https://handlebarsjs.com/) for placeholders and enables using the same SVG image across multiple action.

For template examples see the various `template.svg` files in the [project GitHub repo](https://github.com/neilenns/streamdeck-vatis/tree/main/com.neil-enns.vatis.sdPlugin/images/actions). Here is the template used for the [ATIS letter action](../atis-letter/):

```svg {filename="ATIS letter action SVG template" hl_lines=[4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20]}
<svg xmlns="http://www.w3.org/2000/svg" version="1.2" width="144" height="144">
	<defs>
		<style>
			.displayText {
				fill: {{#if isConnected}}white{{else}}grey{{/if}};
			}
			.altimeterText {
				{{#if (eq pressure.unit "MercuryInch")}}
					{{#if (lte pressure.value 2991 )}}
						fill: {{#if isConnected}}red{{else}}grey{{/if}};
					{{else}}
						fill: {{#if isConnected}}white{{else}}grey{{/if}};
					{{/if}}
				{{else}}
					fill: {{#if isConnected}}white{{else}}grey{{/if}};
				{{/if}}
			}
			.background {
				fill: {{#if isNewAtis}}#e96518{{else}}black{{/if}};
			}
		</style>
	</defs>

	<rect class="background" width="144" height="144"/>
	<text class="displayText" x="72" y="36" font-family="Verdana" font-weight="bold" font-size="22"
		text-anchor="middle">{{title}}</text>
	<text class="displayText" x="72" y="92" font-family="Verdana" font-weight="bold" font-size="50"
		text-anchor="middle">{{#if letter}}{{letter}}{{else}}ATIS{{/if}}</text>
	<text class="altimeterText" x="72" y="130" font-family="Verdana" font-weight="bold" font-size="22"
		text-anchor="middle">{{pressure.formattedValue}}</text>
</svg>
```

In addition to the default helpers the following logical operators are supported:

| Operator | Description           |
| -------- | --------------------- |
| eq       | Equals                |
| ne       | Not equals            |
| gt       | Greater than          |
| gte      | Greater than or equal |
| lt       | Less than             |
| lte      | Less than or equal    |

Example:

```xml
{{#if (eq state "connected")}} {{else}} {{/if}}
```

For a list of the variables provided to the template see the `SVG template variables` section of the action's documentation page.
