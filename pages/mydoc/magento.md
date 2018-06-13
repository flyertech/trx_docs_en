---
title:  "How to install and configure the Magento plugin"
permalink: magento.html
sidebar: mydoc_sidebar
folder: mydoc
---

### Obtaining the latest Magento module
You can download the latest version from your dashboard by going to **My Account -> Integration -> Select Magento 1.x**, click **Download the plugin**.

{% include image.html file="magento/downloadplugin.png" url="images/magento/downloadplugin.png" %}

### Installing the module

From **Magento Connect Manager** click on **Choose file** and then **Upload**.

{% include image.html file="magento/connectmanager.png" url="images/magento/connectmanager.png" %}

Click on Transactionale **Settings**.

{% include image.html file="magento/settings.png" url="images/magento/settings.png" %}

### Settings details

You will be redirected to the module configuration page

The details of the fields displayed are shown below:

*Enabled*| select Yes to enable the plugin.
*Debug*| select No.
*Auth Key*|this is is used to identify your account. **Follow the instructions below to fill it**.
*Import leads automatically*|Enable leads automatic import. When enabled, copy and paste the displayed URL into your Transactionale account at My Account -> Integration -> Webhook URL.

{% include image.html file="magento/webhook.png" url="images/magento/webhook.png" %}

You will also need to complete the configuration for the single store.

The details of the fields displayed are shown below:

*Country Code*| the two-letter ISO code for the country in which your shop operates. I.E. IT.
*Touchpoint Type*| select Auto to automatically select the best choice
*Web Touchpoint Id*|if using the web touchpoint described above, you can specify an id, otherwise it will take a default id.
*Web Touchpoint Text*|if using the web touchpoint described above, you can specify the text to display above the offers.
*Import leads automatically*|Enable leads automatic import. When enabled, copy and paste the displayed URL into your Transactionale account at My Account -> Integration -> Webhook URL.
*Opt-in Privacy Link* | your privacy policy link.

{% include image.html file="magento/configuration_store.png" url="images/magento/configuration_store.png" %}


### Last steps

Copy your Auth Key from your Transactionale account under **My Account-> Integration** ed  and paste into the Auth Key of the Magento plugin settings.

{% include image.html file="magento/apikey.png" url="images/magento/apikey.png" %}

After completing all the required fields click on Save.


### Enabling automatic import of leads - Webhook

For the automatic import of leads via webhook you have to select **YES** in the field **Import leads automatically**

{% include image.html file="magento/webhook.png" url="images/magento/webhook.png" %}

Paste the link you see in the **My Account-> Integration** section of your Transactional account in the **Webhook Url** field.

### Verify integration and webhook

You can check the correct functioning of the technological integration and the webhook url through these simple instructions:

{% include_relative partials/link_verify.md %}

