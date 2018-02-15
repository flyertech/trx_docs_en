---
title: "Overview"
sidebar: mydoc_sidebar
permalink: index.html
folder: mydoc
summary: V2 Integration Details

---

This is the **Transactionale tech knowledge base**, where you can find all the details to integrate your e-Shop with Transactionale.

{% comment %}
{% include callout.html content="If your shop is based on **WooCommerce** or **Prestashop**, we can provide you ready-made plugins that you can install and configure autonomously, without any tech involved." %}
{% endcomment %}

# How to? Technical instructions

You can integrate with us in two ways:

  - [Full integration](full_integration.html), **recommended** for best performance
  - [Simplified integration](simplified_integration.html)

You can enable the [development mode](debugging.html) to ensure the correctness of the integration.

# How the network works

## Advertiser {#advertiser}
With **Transactionale** you can engage new potential customers into your e-Shop and track their conversions.

### How do I engage new customers?
In just a few steps, you will be able to create an **advertising campaign** and we will **distribute it over our network**. Customers from other shops will receive your offer and will claim it on your website. This will allow you to acquire **qualified leads** of real customers who do online shopping.

If you also choose to be a [publisher](#publisher), you can also **monetize** and, if you want so, reinvest your earnings into new acquisition campaigns, lowering their cost.

### How to manage generated leads
We keep track of all the generated leads, allowing you to monitor on our platform how your campaigns are performing.

But we can also deliver every generated leads **to your systems in real time** to allow you collect the data of the generated leads directly on your platform. This allows integrations with **newsletters**, **email automation** systems, **remarketing** or more. Check out the [webhook](webhook.html) section for implementation details. Using the webhook is required to enable the **deduplication** system.

## Publisher {#publisher}
With **Transactionale** you will be able to monetize your customers while making them happy by delivering them targeted special offers.

### How do I earn through the network?
When Lisa, one of your customers, **finalizes an order on your e-Shop**, Transactionale will send her some offers from other shops in our network - complementary and non-competing. Every time an offer generates a lead (that is, when Lisa clicks on an offer and lands on the advertised website), your **earn** something.

In addition, if you also are an [advertiser](#advertiser), you will be able to reinvest your earnings for lead-generation campaigns, lowering acquisition costs.

### How does it work?
1. Lisa makes an order on your shop
2. Every time an order is submitted, your shop **notifies** us about it through a **tracking snippet**, usually on the thank-you page
3. As soon as we receive the notification, Transactionale will send Lisa a **transactional email** with targeted offers
4. If Lisa clicks on an offer, a **lead** will be generated
