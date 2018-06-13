---
title: Simplified integration
sidebar: mydoc_sidebar
permalink: simplified_integration.html
folder: mydoc
---

### Overview
{% include_relative partials/integration_overview.md %}

{% include callout.html content="The semplified integration is discouraged for publishers since it reduces the profiling quality, and thus the lead generation performance." %}

### Put the loader tag in all the pages
The loader tag goes in the `<head>` of your base template.
{% include_relative snippets/loader.md %}

### Put the `viewPage` tag in all the pages
This tag should be inserted preferably before the closing `</body>`, or in any case after the loader inside the `<head>` tag.
{% include_relative snippets/viewpage.md %}

You can also invoke the `viewPage` along with the loader creation:
{% include_relative snippets/loader_viewPage.md %}

### Put the `trackTransaction` in the order confirmation page
This tag should be inserted preferably before the closing `</body>`, or in any case after the loader inside the `<head>` tag.
You must fill as many fields as you can with the actual values relative to the order just submitted.

{% include callout.html content="WARNING: The sample values ('xxxx') must be replaced with the corresponding variables, you can delete the fields whose value isn't retain." %}

{% include_relative snippets/tracktransaction.md %}

### Automatic touchpoint selection
By setting `auto` as `touchpointType`, the best touchpoint will be activated automatically according to the values provided. In case the web touchpoint is activated and no `touchpointId` is provided, the default one will be used.

### Web and auto touchpoints
If you are using a web (or auto) touchpoint, you should define where you want the offers to appear in your page.
To do this, insert a `<div id="tr_touchpoint_container"></div>` in the desired place.

### Offers banner
If you want to use the banner version of the web touchpoint, you have two available layouts to choose from: horizontal (default) or vertical.

{% include image.html file="banner_horizontal.png" url="images/banner_horizontal.png" %}

You can enable a vertical layout by adding the `tr-touchpoint-layout-vertical` class to the `<div>` like this:<br>
 `<div id="tr_touchpoint_container" class="tr-touchpoint-layout-vertical"></div>` <br>
The banner will appear similar to the following:

{% include image.html file="banner_vertical.png" url="images/banner_vertical.png" %}

### Verify integration and webhook

You can check the correct functioning of the technological integration and the webhook url through these simple instructions:

{% include_relative partials/link_verify.md %}