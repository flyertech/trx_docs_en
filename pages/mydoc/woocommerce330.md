---
title:  "How to install and configure the Woocommerce plugin"
permalink: woocommerce330.html
sidebar: mydoc_sidebar
folder: mydoc
---

### Download the latest version of the Woocommerce module
You can download the latest version of the Woocommerce module by going to **My Account -> Integration -> Select Woocommerce ->** click **Download the plugin.**

{% include image.html file="woocommerce/downloadplugin.png" url="images/woocommerce/downloadplugin.png" %}

### Installing the module

To install the Transactionale plugin, you need to log in to the backend of your website and go to the **Plugin section**:
{% include image.html file="woocommerce/1.png" url="images/woocommerce/1.png" %}

Click **“Add new”**

{% include image.html file="woocommerce/02.png" url="images/woocommerce/02.png" %}

Click **“Upload Plugin”**

{% include image.html file="woocommerce/03.png" url="images/woocommerce/03.png" %}

Upload the plugin’s zip file by clicking on the **“Choose file”** button

{% include image.html file="woocommerce/04.png" url="images/woocommerce/04.png" %}

Then click **“Install Now”**

{% include image.html file="woocommerce/05.png" url="images/woocommerce/05.png" %}

After installing the plugin, the “Transactionale” field will be added to the sidebar

{% include image.html file="woocommerce/06.png" url="images/woocommerce/06.png" %}

After installation, you will move on to the module configuration.

### Wordpress module configuration
The following page will appear in Transactionale’s configuration process:

{% include image.html file="woocommerce/07.png" url="images/woocommerce/07.png" %}

Let’s take a look at each field to choose the desired settings:

---

**Transactionale Status**
- **Enable** → Transactionale will be activated and ready to be used; 
- **Disabled** → Transactionale will be deactivated.

---

**Auth Key**
Authorization code provided by Transactionale to identify your account

---

**Country Code**
Two-letter ISO code for the country in which your shop operates (e.g. it, en, etc…)

---

**Show 3rd Party Opt-In checkbox**
- **Enable** → By enabling this feature, the following checkbox is displayed during checkout: 
{% include image.html file="woocommerce/08.png" url="images/woocommerce/08.png" %}

- <ins>What happens if the acceptance box is checked</ins>: An email is sent while the banner is not displayed;
- <ins>What happens if the acceptance box is NOT checked</ins>: No email is sent and only the banner is displayed

- **Disabled** → The checkbox does not appear during checkout; by default, no email is sent and only the banner is displayed.

* This feature is specific to Wordpress.

---

**Touchpoint Type**
From the drop-down menu, you can choose one of the following touchpoints to deliver offers to your customers:
- **Email** → Only an email related to the special offers will be sent; 
- **Web** → Only a banner related to the special offers will be displayed on the website;
- **Auto (Web + Mail)** → This field depends on what users choose in the 3rd party opt-in checkbox.

Only by selecting Web and Auto, two additional fields appear which are exclusively related to the banner:
- **Web Touchpoint Id** → You need to enter the ID of the div which has been set to be populated with the banner’s data in the template;
- **Web Touchpoint Text** → Banner title to be displayed – “Special offers reserved for you”, in this case.

{% include image.html file="woocommerce/09.png" url="images/woocommerce/09.png" %}

### Summary

{% include image.html file="woocommerce/10.png" url="images/woocommerce/10.png" %}

*Only for Wordpress 

### Last steps

Copy your Auth Key from your Transactionale account under **My Account-> Integration** and paste into the Auth Key field in the configuration page of the WooCommerce plugin.

{% include image.html file="woocommerce/apikey.png" url="images/woocommerce/apikey.png" %}

### Verify integration

You can verify the correct functioning of the technological integration and the webhook url by following these simple instructions:

{% include_relative partials/link_verify_integration.md %}