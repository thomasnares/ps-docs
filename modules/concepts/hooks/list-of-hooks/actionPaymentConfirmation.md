---
menuTitle: actionPaymentConfirmation
Title: actionPaymentConfirmation
hidden: true
hookTitle: Payment confirmation
files:
  - classes/order/OrderHistory.php
location:
  - front office
type: action
hookAliases:
 - paymentConfirm
---

# Hook actionPaymentConfirmation

Aliases: 
 - paymentConfirm



## Information

{{% notice tip %}}
**Payment confirmation:** 

This hook displays new elements after the payment is validated
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/order/OrderHistory.php](classes/order/OrderHistory.php)

## Parameters details

```php
    <?php
    array(
      'id_order' => (int) Order ID
    );
```

## Call of the Hook in the origin file

```php
Hook::exec('actionPaymentConfirmation', ['id_order' => (int) $order->id], null, false, true, false, $order->id_shop)
```