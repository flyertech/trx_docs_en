---
title:  "How to install and configure the Prestashop module >= 1.7"
permalink: prestashop17.html
sidebar: mydoc_sidebar
folder: mydoc
---


Obtaining the latest Prestashop module
You can download the latest version from your dashboard by going to **My Account -> Integration -> Select Prestashop <= 1.7**, click **Download the plugin**

{% include image.html file="prestashop17/downloadplugin.png" url="/images/prestashop17/downloadplugin.png" %}

### Installing the module

Go to the your Prestashop **Modules and Services** and you install the plugin you just downloaded. At the end of the installation click on **Configure**.

{% include image.html file="prestashop17/uploadplugin.png" url="/images/prestashop17/uploadplugin.png" %}


### Settings details
You will be redirected to the module configuration page

{% include image.html file="prestashop17/4.png" url="/images/prestashop17/4.png" %}

The details of the fields displayed are shown below:

*Auth Key*|this is used to identify your account. **Follow the instructions below to fill it**.
*Country*|the two-letter ISO code for the country in which your shop operates. I.E. IT.
*Touchpoint Type*|how to deliver offers to your customers. Make sure you configure your touchpoints in your Transactionale account. It can be Web, Mail, Web+Mail.
*Web Touchpoint Id*|if using the web touchpoint described above, you can specify an id, otherwise it will take a default id.
*Web Touchpoint Text*|if using the web touchpoint described above, you can specify the text to display above the offers.
*Import leads automatically*|Enable leads automatic import. When enabled, copy and paste the displayed URL into your Transactionale account at My Account -> Integration -> Webhook URL.

{% include image.html file="prestashop17/5.png" url="/images/prestashop17/5.png" %}

### Enabling/Disabing Optin

The **opt-in** must be activated from the **Preferences -> Customers** section.
{% include image.html file="prestashop17/optin.png" url="/images/prestashop17/optin.png" %}

### Last steps

Copy your Auth Key from your Transactionale account under  **My Account-> Integration**  and paste into the Auth Key of the Prestashop module configuration.

{% include image.html file="prestashop17/apikey.png" url="/images/prestashop17/apikey.png" %}

Remember to Save the changes.

### Enabling automatic import of leads - Webhook

For the automatic import of leads via webhook you have to select **YES** in the field **Import leads automatically**

{% include image.html file="prestashop17/webhook.png" url="/images/prestashop17/webhook.png" %}

Paste the link you see in the **My Account-> Integration** section of your Transactional account in the **Webhook Url** field.

{% include image.html file="prestashop17/webhookurl.png" url="/images/prestashop17/webhookurl.png" %}

To check the correct functioning click on **Test** .