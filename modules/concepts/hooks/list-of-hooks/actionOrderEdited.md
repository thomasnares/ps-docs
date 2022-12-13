---
menuTitle: actionOrderEdited
Title: actionOrderEdited
hidden: true
hookTitle: Order edited
files:
  - src/Adapter/Order/CommandHandler/UpdateProductInOrderHandler.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionOrderEdited

## Information

{{% notice tip %}}
**Order edited:** 

This hook is called when an order is edited
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/Adapter/Order/CommandHandler/UpdateProductInOrderHandler.php](src/Adapter/Order/CommandHandler/UpdateProductInOrderHandler.php)

## Parameters details

```php
      <?php
        array( 'order' => (object) Order
      );
```

## Call of the Hook in the origin file

```php
Hook::exec('actionOrderEdited', ['order' => $order])
```