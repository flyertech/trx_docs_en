---
title:  "How to install and configure the Prestashop module <= 1.6"
permalink: prestashop16.html
sidebar: mydoc_sidebar
folder: mydoc
---


### Download the latest version of the Prestashop module
You can download the latest version of the Prestashop module by going to **My Account -> Integration -> Select Prestashop <= 1.6**, click **Download the plugin**

{% include image.html file="prestashop16/downloadplugin.png" url="images/prestashop16/downloadplugin.png" %}

### Installing the module

To install Transactionale on your Prestashop website, you need to log in to the backend and access the **“Modules → Module manager”** section, on the right sidebar.

{% include image.html file="prestashop16/01.png" url="images/prestashop16/01.png" %}

After accessing the section, there will be an **“Upload a module”** button at the top right corner to be clicked on

{% include image.html file="prestashop16/02.png" url="images/prestashop16/02.png" %}

The following window will appear: 

{% include image.html file="prestashop16/03.png" url="images/prestashop16/03.png" %}

You will then need to upload the module’s zip file:

{% include image.html file="prestashop16/04.png" url="images/prestashop16/04.png" %}

Click **“Configure”** to proceed with the configuration.


### Configuration details
The following page will appear in Transactionale’s configuration process:

{% include image.html file="prestashop16/05.png" url="images/prestashop16/05.png" %}

Let’s take a look at <ins>each field</ins> to choose the desired settings:

---

**Transactionale’s Activation/Deactivation**
To activate or deactivate Transactionale, you can enable/disable the module directly on Prestashop.

---

**Auth Key**
Authorization code provided by Transactionale to identify your account (follow the instructions below to fill it in)

---

**Country Code**
Two-letter ISO code for the country in which your shop operates (e.g. it, en, etc…)

---

**Touchpoint Type**
From the drop-down menu, you can choose one of the following touchpoints to deliver offers to your customers:
- **Email** → Only an email related to the special offers will be sent;

- **Web** → Only a banner related to the special offers will be displayed on the website;

- **Auto (Web + Mail)** →  This field depends on what users choose in the “Receive offers from our partners” checkbox, enabled by default in Prestashop.
{% include image.html file="prestashop16/06.png" url="images/prestashop16/06.png" %}

Only by selecting **Web and Mail + Web**, two additional fields appear which are exclusively related to the banner:

- **Web Touchpoint Id** → You need to enter the ID of the div which has been set to be populated with the banner’s data in the template (if you are using the web touchpoint, you need to specify an ID, otherwise it will take a default ID);

- **Web Touchpoint Text** → Banner title to be displayed – “There are special offers for you”, in this case.
{% include image.html file="prestashop16/07.png" url="images/prestashop16/07.png" %}


### Summary

{% include image.html file="prestashop16/08.png" url="images/prestashop16/08.png" %}

### Last steps
Copy your Auth Key from your Transactionale account under **My Account-> Integration** and 

{% include image.html file="prestashop16/apikey.png" url="images/prestashop16/apikey.png" %}

paste into the Auth Key field in the configuration page of the Prestashop module.

### Verify integration 

You can verify the correct functioning of the technological integration and the webhook url by following these simple instructions:

{% include_relative partials/link_verify_integration.md %}