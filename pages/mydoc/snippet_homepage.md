---
title: Home page snippet
sidebar: mydoc_sidebar
permalink: snippet_homepage.html
folder: mydoc
---

## Description
The Home page integration allows tracking *bounces* and tracking users who have clicks on a Transcationale offer.

{% include_relative partials/loader_warning.md %}

```js
<script>
    window._trx.push({
        event: 'viewHome'
    });
</script>
```