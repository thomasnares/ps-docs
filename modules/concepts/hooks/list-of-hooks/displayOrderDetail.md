---
menuTitle: displayOrderDetail
Title: displayOrderDetail
hidden: true
hookTitle: Order detail
files:
  - controllers/front/OrderDetailController.php
location:
  - front office
type: display
hookAliases:
 - orderDetailDisplayed
---

# Hook displayOrderDetail

Aliases: 
 - orderDetailDisplayed



## Information

{{% notice tip %}}
**Order detail:** 

This hook is displayed within the order's details in Front Office
{{% /notice %}}

Hook location:
  - front office

Hook type: display

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/controllers/front/OrderDetailController.php](controllers/front/OrderDetailController.php)

## Parameters details

```php
    <?php
    array(
      'order' => (object) Order object
    );
```

## Call of the Hook in the origin file

```php
Hook::exec('displayOrderDetail', ['order' => $order])
```