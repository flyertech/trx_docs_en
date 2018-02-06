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