---
title: SVG templates
description: Information on how to use SVG templates with TrackAudio actions
og_image: ogimage/streamdeck-vatis.png
---

All image properties on all actions support using SVG templates instead of a standard SVG image. The templates use [Handlebars](https://handlebarsjs.com/) for placeholders and enables using the same SVG image across multiple action.

For template examples see the various `template.svg` files in the [project GitHub repo](https://github.com/neilenns/streamdeck-trackaudio/tree/main/com.neil-enns.trackaudio.sdPlugin/images/actions).

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
