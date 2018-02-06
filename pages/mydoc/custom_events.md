---
title: Custom events
sidebar: mydoc_sidebar
permalink: custom_events.html
folder: mydoc
---

Custom events allow you to create custom lead-generation funnels.
For instance, you can use the [viewPage](#viewPage) event to generate a lead only when a customer navigates to a specified page after clicking on your offer.
The [customEvent](#customEvent) allows generating a lead only when a specific event is triggered, i.e. the user fills-in a form, or wins a competition. It's useful in case of Single Page Applications, where the full page is never reloaded.

## viewPage
Allows tracking a generic page you define. For example, when you want to generate a lead only when the user sees the www.yoursite.com/success page.

```html
<!-- www.yoursite.com/success -->
...
<body>
    <h1>Success!</h1>
</body>
<script>
window._trx.push(
    { event: 'viewPage'}
);
</script>
```
You will have to select *URL* as *Lead funnel type* in the campaign settings, and insert www.yoursite.com/success as the URL.

## customEvent
Allows tracking a generic event you define.
It can be used for custom funnels in Single Page Applications or anywhere you want to track an event after page load.

```js
window._trx.push(
    { event: 'customEvent', name: 'my-custom-event-name'}
);
```
To capture the event, you need to configure the campaign by setting the event name in the dedicated field after selecting *Event* as *Lead funnel type*.