---
title: Products listing page
sidebar: mydoc_sidebar
permalink: snippet_pagina_ricerca.html
folder: mydoc
---

## Description
A **products listing page** shows a list items. For example, it can be a category page, or a search results page.

{% include_relative partials/loader_warning.md %}

## The viewList event
Items can be provided in two ways:
 - by id only: if you have previous imported your products data feed into Transactionale
 - a full object with all the required details

 If you provide the products by ID only, make sure you use the same ID as contained in the datafeed you provided.
 
```js
_trx.push({
  event: 'viewList',
  itemIDs: ['ABC123', 'ABC124']
});

// Example of full product specification
_trx.push({
  event: 'viewList',
  items: [{
        id: 'ABC123', 
        price: '12.34', 
        name: 'Product name', 
        categoryId: 123, // Google merchant center category ID 
        categoryName: 'My Category', // Custom or Google category name
        barcode: '0000123456789'
      }]
});
```

{% include_relative partials/google_categories.md %}