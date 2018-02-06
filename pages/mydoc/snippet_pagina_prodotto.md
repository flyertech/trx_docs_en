---
title: Product details snippet
sidebar: mydoc_sidebar
permalink: snippet_pagina_prodotto.html
folder: mydoc
---

## Description
The **product page** contains the details of a single product.

{% include_relative partials/loader_warning.md %}

## The viewItem event
Keeps track of a visit to a single item (product, property, etc.)
Items can be provided in two ways:
 - by id only: if you have previous imported your products data feed into Transactionale
 - a full object with all the required details

If you provide the products by ID only, make sure you use the same ID as contained in the datafeed you provided.

```js
    _trx.push({
      event: 'viewItem',
      itemID: 'ABC123'
    });
    
    // Example of full product specification
    _trx.push({
      event: 'viewItem',
      item: {
        id: 'ABC123', 
        price: '12.34', 
        name: 'Product name', 
        categoryId: 123, // Google merchant center category ID 
        categoryName: 'My Category', // Custom or Google category name
        barcode: '0000123456789'
      }
    });
```

[Google merchant categories (ENG)](https://www.google.com/basepages/producttype/taxonomy-with-ids.en-US.txt)
[Google merchant categories (ITA)](https://www.google.com/basepages/producttype/taxonomy-with-ids.it-IT.txt)
[Google merchant categories (ESP)](https://www.google.com/basepages/producttype/taxonomy-with-ids.es-ES.txt)