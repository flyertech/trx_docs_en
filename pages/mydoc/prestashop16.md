---
title:  "How to install and configure the Prestashop module <= 1.6"
permalink: prestashop16.html
sidebar: mydoc_sidebar
folder: mydoc
---


### Obtaining the latest Prestashop module
You can download the latest version from your dashboard by going to **My Account -> Integration -> Select Prestashop <= 1.6**, click **Download the plugin**

{% include image.html file="prestashop16/downloadplugin.png" url="/images/prestashop16/downloadplugin.png" %}

### Installing the module

Go to the your Prestashop **Modules and Services** click on the **Add new module**. A form will appear where you can upload the module's zip file, click **Choose a file** and **Upload this module**.

{% include image.html file="prestashop16/1.png" url="/images/prestashop16/1.png" %}

The list of modules will appear, in particular you will see the Transactionale module just uploaded. You will have to click on **Install**

{% include image.html file="prestashop16/2.png" url="/images/prestashop16/2.png" %}

A popup will appear, click on **Proceed with installation**

{% include image.html file="prestashop16/3.png" url="/images/prestashop16/3.png" %}

### Settings details

You will be redirected to the module configuration page

{% include image.html file="prestashop16/4.png" url="/images/prestashop16/4.png" %}

The details of the fields displayed are shown below:

*Auth Key*|this is used to identify your account. **Follow the instructions below to fill it**.
*Country*|the two-letter ISO code for the country in which your shop operates. I.E. IT.
*Touchpoint Type*|how to deliver offers to your customers. Make sure you configure your touchpoints in your Transactionale account. It can be Web, Mail, Web+Mail.
*Web Touchpoint Id*|if using the web touchpoint described above, you can specify an id, otherwise it will take a default id.
*Web Touchpoint Text*|if using the web touchpoint described above, you can specify the text to display above the offers.
*Import leads automatically*|Enable leads automatic import. When enabled, copy and paste the displayed URL into your Transactionale account at My Account -> Integration -> Webhook URL.

{% include image.html file="prestashop16/5.png" url="/images/prestashop16/5.png" %}

### Enabling/Disabing Optin

The **opt-in** must be activated from the **Preferences -> Customers** section.

{% include image.html file="prestashop16/optin.png" url="/images/prestashop16/optin.png" %}

### Last steps

Copy your Auth Key from your Transactionale account under  **My Account-> Integration**  and paste into the Auth Key of the Prestashop module configuration.

{% include image.html file="prestashop16/apikey.png" url="/images/prestashop16/apikey.png" %}

Remember to Save the changes.

### Enabling automatic import of leads - Webhook

For the automatic import of leads via webhook you have to select **YES** in the field **Import leads automatically**.

{% include image.html file="prestashop16/webhook.png" url="/images/prestashop16/webhook.png" %}

Paste the link you see in the **My Account-> Integration** section of your Transactional account in the **Webhook Url** field.

{% include image.html file="prestashop16/webhookurl.png" url="/images/prestashop16/webhookurl.png" %}

To check the correct functioning click on **Test** .
