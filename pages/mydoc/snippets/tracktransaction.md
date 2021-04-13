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
        // This will automatically display the appropriate touchpoint according to your settings
        touchpointType: 'auto',
    }
);
</script>
```
```html
<!-- Only for publishers - Defines the spot where the banner or the offers will be displayed -->
<div id="tr_touchpoint_container"></div>
```