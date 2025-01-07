---
title: SVG templates
description: Information on how to use SVG templates with vATIS actions
og_image: ogimage/streamdeck-trackaudio.png
---

All image properties on all actions support using SVG templates instead of a standard SVG image. The templates use [Handlebars](https://handlebarsjs.com/) for placeholders and enables using the same SVG image across multiple action.

For template examples see the various `template.svg` files in the [project GitHub repo](https://github.com/neilenns/streamdeck-trackaudio/tree/main/com.neil-enns.trackaudio.sdPlugin/images/actions). Here is the template used for the [TrackAudio status action](../trackaudio-status/):

```svg {filename="TrackAudio status action SVG template" hl_lines=[9,10,11,12,13,14,15,16,17,18]}
<svg
  id="Layer_1"
  data-name="Layer 1"
  xmlns="http://www.w3.org/2000/svg"
  version="1.1"
  viewBox="0 0 350 350"
>
  <style>
    .headset {
    	{{#if (eq state "notConnected")}}
    		fill: white;
    	{{else if (eq state "connected")}}
    		fill: #5fcdfa;
    	{{else if (eq state "voiceConnected")}}
    		fill: #006600;
    	{{else}}
    		fill: black;
    	{{/if}}
    }
  </style>
  <path
    class="headset"
    stroke-width="0px"
    d="M261.3,286.1v-12.2h-22.1c-16.4,0-27-10.6-27-26.8v-45.5c0-16.2,10.4-26.5,26.6-26.6h22.6c0-10,.3-19.6,0-29.2-1.6-39.5-30.8-73.2-69.7-80.8-38.1-7.5-76.4,12.3-93.6,47.7-9.5,19.7-10.4,40.3-9.2,62.2,7.7,0,15.3-.4,22.9.1,4.7.3,9.7,1.3,13.8,3.5,8.2,4.3,12.1,11.9,12.3,21,.3,16.5.3,33,0,49.5-.2,14.1-11.3,24.7-25.5,24.8-10.3.1-20.7.7-30.1-5.1-11.6-7.2-18.2-17.5-18.3-31.3-.2-29-.4-58,0-87,.8-50.8,35.5-95.7,84.7-108,50.6-12.6,103.1,11.8,126.4,59.3,7.6,15.5,11.1,32,11,49.3-.1,40.3,0,80.7,0,121s-15.7,38.9-38.9,38.9h-57.5c-8.6,0-14.5-5-14.5-12.4s5.9-12.4,14.6-12.4h71.5,0Z"
  />
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
