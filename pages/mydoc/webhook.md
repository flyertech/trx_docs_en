---
title: Webhook / lead tracking
sidebar: mydoc_sidebar
permalink: webhook.html
folder: mydoc
---

## Overview
**Transactionale** handles all the lead generation process for you. But if you have the resources, it's a great idea to take advantage of the Transactionale **webhook** to improve your performance.

We created this feature to help you **automatically import leads into your platform** so you can implement your own marketing strategies with them.

With the webhook, **leads are notified immediately** when they are generated according to the *Lead generation funnel* you selected for your campaign.
This way you will be able to use the data for statistics, marketing automations or any other use you need.

## How does it work?
The advertiser can set-up an URL to be called with the lead data according to the specifications below.
**IMPORTANT:** if you use the webhook to send reminders, please remember to disable reminders in the campaign settings to avoid overlapping communications to your users.

## Implementation details
You will receive a `POST` request encoded as ```application/x-www-form-urlencoded```, so just like a form submission, with the following parameters:

|Parameter| Description|
|-------|------|
|ad_id| the campaign id|
|email|	email address|
|first_name|	the user's first name|
|last_name|	the users's last name|
|gender|	gender (“M” o “F”)|
|phone|	phone number|
|birth_year|	year of birth|
|coupon_code|	the coupon code recived by the user, optional. Useful for multi-coupon campaigns|
|zip_code|	the user's postal code|

Example:
```
ad_id=72&email=test%40transactionale.com&coupon_code=TRCOUPON&first_name=Marianna&zip_code=12345
```

{% include callout.html content="<strong>NOTE</strong>: the actual data you will receive depends on the data the publisher shares with Transactionale. We guarantee the ad_id and email field. For all the other fields, always consider the case they are not present." %}

## Error handling
The content of the response will not be considered. The **response codes >= 300** will be considered as errors, therefore the system might re-try sending the request.

## Deduplication
The **HTTP 400 response code** indicates that the email address is a duplicate, so it will not be charged as a lead.

