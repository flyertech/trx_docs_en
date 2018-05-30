---
title:  "How to install and configure the Woocommerce plugin"
permalink: woocommerce330.html
sidebar: mydoc_sidebar
folder: mydoc
---

### Obtaining the latest Prestashop module
You can download the latest version from your dashboard by going to **My Account -> Integration -> Select Woocommerce >= 3.3.0**, click **Download the plugin**.

{% include image.html file="woocommerce/downloadplugin.png" url="images/woocommerce/downloadplugin.png" %}

### Installing the module

From the Plugin section of your WooCommerce click on **Add plugin** and you install the plugin you just downloaded.
{% include image.html file="woocommerce/1.png" url="images/woocommerce/1.png" %}

You will be redirected to the Plugin section and you will find Trasactionale.

If you haven't specified any Terms and Conditions page for your shop you will see the **Woocommerce Checkout Settings** link

{% include image.html file="woocommerce/checkoutsettings.png" url="images/woocommerce/checkoutsettings.png" %}

On this page you will need to insert the page where **Terms and Conditions** of your shop are specified.

{% include image.html file="woocommerce/termsconditions.png" url="images/woocommerce/termsconditions.png" %}

Remember to Save the changes.

Return to the **Plugin** section

Click on **Settings** related to the Transactionale plugin.

{% include image.html file="woocommerce/settings.png" url="images/woocommerce/settings.png" %}

### Settings details

You will be redirected to the module configuration page

The details of the fields displayed are shown below:

*Transactionale status*|select Enabled to enable the plugin.
*Auth Key*|this is used to identify your account. **Follow the instructions below to fill it**.
*Country code*|the two-letter ISO code for the country in which your shop operates. I.E. IT.
*Product Format*|indicates the format of the product that the teeth send (Full or Id only).
*Touchpoint Type*|how to deliver offers to your customers. Make sure you configure your touchpoints in your Transactionale account. It can be Web, Mail, Web+Mail.
*Web Touchpoint Text*|if using the web touchpoint described above, you can specify the text to display above the offers.
*Import leads automatically*|Enable leads automatic import. When enabled, copy and paste the displayed URL into your Transactionale account at My Account -> Integration -> Webhook URL.

{% include image.html file="woocommerce/configuration.png" url="images/woocommerce/configuration.png" %}


### Last steps

Copy your Auth Key from your Transactionale account under  **My Account-> Integration**  and paste into the Auth Key of the Woocommerce plugin configuration.

{% include image.html file="woocommerce/apikey.png" url="images/woocommerce/apikey.png" %}

After completing all the required fields click on Save.

{% include image.html file="woocommerce/configurationsave.png" url="images/woocommerce/configurationsave.png" %}