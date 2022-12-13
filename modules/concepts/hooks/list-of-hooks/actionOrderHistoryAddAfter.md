---
menuTitle: actionOrderHistoryAddAfter
Title: actionOrderHistoryAddAfter
hidden: true
hookTitle: 
files:
  - classes/order/OrderHistory.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionOrderHistoryAddAfter

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/order/OrderHistory.php](classes/order/OrderHistory.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionOrderHistoryAddAfter', ['order_history' => $this], null, false, true, false, $order->id_shop)
```