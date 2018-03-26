---
title: Simplified integration
sidebar: mydoc_sidebar
permalink: simplified_integration.html
folder: mydoc
---

## Overview
{% include_relative partials/integration_overview.md %}

{% include callout.html content="The semplified integration is discouraged for publishers since it reduces the profiling quality, and thus the lead generation performance." %}

## Put the loader tag in all the pages
The loader tag goes in the `<head>` of your base template.
{% include_relative snippets/loader.md %}

## Put the `viewPage` tag in all the pages
This tag should be inserted preferably before the closing `</body>`, or in any case after the loader inside the `<head>` tag.
{% include_relative snippets/viewpage.md %}

You can also invoke the `viewPage` along with the loader creation:
```html
<script>
    window._trx = window._trx || [];
    window._trx.push(
        { event: 'setAccount', account: '**API-KEY**', country: 'IT' },
        { event: 'viewPage' }
    );
</script>
<script src="https://static.transactionale.com/trx/v2/trx.js" async="true"></script>
```

## Put the `trackTransaction` in the order confirmation page
This tag should be inserted preferably before the closing `</body>`, or in any case after the loader inside the `<head>` tag.
You must fill as many fields as you can with the actual values relative to the order just submitted.

{% include_relative snippets/tracktransaction.md %}

## Web touchpoint
If you are using a web touchpoint, you should define where you want the offers to appear in your page.
To do this, insert a `<div id="tr_touchpoint_container"></div>` in the desired place.




