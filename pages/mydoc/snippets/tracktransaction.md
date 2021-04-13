```html
<script>
window._trx.push(
    {
        event: 'trackTransaction',
        transaction: {
            id: 'xxxxx', // Order ID
            total: xxx.xx, // Required
            currency: 'EUR' // EUR by default
        },
        // The customer object can be removed if the website does not support a dedicated opt-in for data sharing with third parties
        customer: {
            firstName: 'name', // Optional
            lastName: 'surname', // Optional
            email: 'indirizzo@email.com', // Optional
            optin: false // Optional - if false all the provided data will be discarded
        },
        // touchpointId: 123, // Always show the provided touchpoint
        touchpointType: 'auto' // auto, web, mail
    }
);
</script>
```
```html
<!-- Only for publishers - Defines the spot where the banner or the offers will be displayed -->
<div id="tr_touchpoint_container"></div>
```