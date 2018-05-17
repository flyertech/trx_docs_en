```js
window._trx.push(
    {
        event: 'trackTransaction',
        transaction: {
            id: 'xxxxx', // Order number
            subtotal: xxx.xx,
            shipping: xxx.xx,
            discount: xxx.xx,
            total: xxx.xx, // Required
            coupon: 'xxx', 
            currency: 'EUR', // EUR by default
        },
        items: [
            {id: x, price: xx.xx, quantity: x}, 
            {id: x, price: xx.xx, quantity: x},
        ],
        address: {
            address: 'xxxxxx',
            address2: 'xxxxxx',
            city: 'xxxxx',
            postalCode: 'xxxxx',
            country: 'IT',
            phone: 'xxxxxxxx',
            phoneMobile: 'xxxxxxxxx',
        },
        customer: {
            firstName: 'Xxxxx',
            lastName: 'Xxxxxxx',
            company: 'xxxxxxxx',
            email: 'xxxxx@xxxx.xx',
            birthdate: 'yyyy-mm-dd', // YYYY-MM-DD
            gender: 'x', 
            optin: xxxx // if the users opted in to receiving commercial offers
        },
        // Example of integration of ads directly in the page
        touchpointType: 'auto',
    }
```
```html
<div id="tr_touchpoint_container"></div>
```