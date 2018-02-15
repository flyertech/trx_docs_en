---
title: Shopping basket snippet
sidebar: mydoc_sidebar
permalink: snippet_carrello.html
folder: mydoc
---

## Overview
The snippet must be implemented in the **shopping basket page** to monitor users who abandon the conversion funnel.

## The viewBasket event
Keeps track of the shopping cart with its contents.
In this case items have to be provided as full objects, since you will have to provide at least one attribute: quantity.

```js
_trx.push({
    event: 'viewBasket',
    items: [{
        id: 'ABC123', // REQUIRED
        quantity: 1, // REQUIRED
        price: '123.23', // String is preferred
        name: 'Example',
        categoryId: 123, // Google category ID
        categoryName: 'Custom o Google category name'
    }]
});
```

{% include_relative partials/google_categories.md %}