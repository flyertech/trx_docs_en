---
title: Shopify
sidebar: mydoc_sidebar
permalink: shopify.html
folder: mydoc
---


### Overview
{% include_relative partials/integration_overview.md %}

### Where should you implement the trackTransaction code? 

From your Shopify **Admin** page, select **Settings**

{% include image.html file="shopify/settings.png" url="images/shopify/settings.png" %}

Click on  **Checkout**

{% include image.html file="shopify/checkout.png" url="images/shopify/checkout.png" %}

{% include image.html file="shopify/apikey.png" url="images/shopify/apikey.png" %}

Paste the following snippet in **Additional scripts**

{% include image.html file="shopify/add_script.png" url="images/shopify/add_script.png" %}

{% include callout.html content="In the following snippet you will need to replace the \"ApiKey\" with your API Key that you will find in your Transactionale account under  **My Account -> Integration**. Copy it" %}

{% highlight html %}{% include_relative snippets/shopify.md %}{% endhighlight %}

Click on **Save** 

{% include image.html file="shopify/save_settings.png" url="images/shopify/save_settings.png" %}

<hr />

###  Where should you implement the loader and the viewPage event? 


From your Shopify **Admin** page, select **Online Store**

{% include image.html file="shopify/online_store.png" url="images/shopify/online_store.png" %}

From **Themes->current theme** click on **Actions->Edit Code**

{% include image.html file="shopify/edit_code.png" url="images/shopify/edit_code.png" %}

{% include callout.html content="In the following snippet you will need to replace the \"ApiKey\" with your API Key that you will find in your Transactionale account under  **My Account -> Integration**. Copy it " %}

Click on **theme.liquid** and paste the code  inside the **<head>** tag of the page 

{% include image.html file="shopify/snippet.png" url="images/shopify/snippet.png" %}

{% include_relative snippets/loader_viewPage.md %}

Click on **Save** 

{% include image.html file="shopify/save_edit_code.png" url="images/shopify/save_edit_code.png" %}

### Verify integration and webhook

You can check the correct functioning of the technological integration and the webhook url through these simple instructions:

{% include_relative partials/link_verify.md %}

