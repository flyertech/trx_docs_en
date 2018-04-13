---
title: Shopify
sidebar: mydoc_sidebar
permalink: shopify.html
folder: mydoc
---


## Overview
{% include_relative partials/integration_overview.md %}

## Where should you implement the trackTransaction code? 

From your Shopify **Admin** page, select **Settings**

![image-title-here](images/shopify/settings.png){:class="img-responsive"}

Click on  **Checkout**

![image-title-here](images/shopify/checkout.png){:class="img-responsive"}


![image-title-here](images/shopify/apikey.png){:class="img-responsive"}

Paste the following snippet in **Additional scripts**

![image-title-here](images/shopify/add_script.png){:class="img-responsive"}

{% include callout.html content="In the following snippet you will need to replace the \"ApiKey\" with your API Key that you will find in your Transactionale account under  **My Account -> Integration**. Copy it" %}

{% highlight html %}{% include_relative snippets/shopify.md %}{% endhighlight %}

Click on **Save** 

![image-title-here](images/shopify/save_settings.png){:class="img-responsive"}

<hr />

##  Where should you implement the loader and the viewPage event? 


From your Shopify **Admin** page, select **Online Store**

![image-title-here](images/shopify/online_store.png){:class="img-responsive"}

From **Themes->current theme** click on **Actions->Edit Code**

![image-title-here](images/shopify/edit_code.png){:class="img-responsive"}

{% include callout.html content="In the following snippet you will need to replace the \"ApiKey\" with your API Key that you will find in your Transactionale account under  **My Account -> Integration**. Copy it " %}

Click on **theme.liquid** and paste the code  inside the **<head>** tag of the page 

![image-title-here](images/shopify/snippet.png){:class="img-responsive"}

{% include_relative snippets/loader_viewPage.md %}

Click on **Save** 

![image-title-here](images/shopify/save_edit_code.png){:class="img-responsive"}


