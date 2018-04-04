---
title: Order confirmation page snippet
sidebar: mydoc_sidebar
permalink: snippet_pagina_conferma.html
folder: mydoc
---

## Description
The **order confirmation page** is displayed after the users completes a purchase on your website. 

{% include_relative partials/loader_warning.md %}

## The trackTransaction event
Tracks a **completed transaction** (order, booking etc.). This allows tracking conversion besides allowing the delivery of offers to the customers via one of the available **touchpoints**: `web` or `mail`.
For `web` touchpoints you should set **touchpointType**: "web" e chiamerà implicitamente [triggerWebTouchpoint](#triggerWebTouchpoint) and also provide a `touchpointId` that you can find on the *Monetize* section of your Transactionale account.

{% include_relative snippets/tracktransaction.md %}

{% include_relative partials/google_categories.md %}


## Automatic touchpoint selection
By setting `auto` as `touchpointType`, the best touchpoint will be activated automatically according to the values provided. In case the web touchpoint is activated and no `touchpointId` is provided, the default one will be used.

## Web and auto touchpoints
If you are using a web (or auto) touchpoint, you should define where you want the offers to appear in your page.
To do this, insert a `<div id="tr_touchpoint_container"></div>` in the desired place.

## Offers banner
If you want to use the banner version of the web touchpoint, you have two available layouts to choose from: horizontal (default) or vertical.

![Horizontal banner](images/banner_horizontal.png){:class="img-responsive"}

You can enable a vertical layout by adding the `tr-touchpoint-layout-vertical` class to the `<div>` like this:<br>
 `<div id="tr_touchpoint_container" class="tr-touchpoint-layout-vertical"></div>` <br>
The banner will appear similar to the following:
![Banner verticale](images/banner_vertical.png){:class="img-responsive"}