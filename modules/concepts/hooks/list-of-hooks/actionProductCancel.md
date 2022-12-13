---
menuTitle: actionProductCancel
Title: actionProductCancel
hidden: true
hookTitle: Product cancelled
files:
  - src/Adapter/Order/CommandHandler/IssueStandardRefundHandler.php
location:
  - front office
type: action
hookAliases:
 - cancelProduct
---

# Hook actionProductCancel

Aliases: 
 - cancelProduct



## Information

{{% notice tip %}}
**Product cancelled:** 

This hook is called when you cancel a product in an order
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/Adapter/Order/CommandHandler/IssueStandardRefundHandler.php](src/Adapter/Order/CommandHandler/IssueStandardRefundHandler.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionProductCancel', ['order' => $order, 'id_order_detail' => (int) $orderDetailId, 'cancel_quantity' => $productRefund['quantity'], 'action' => CancellationActionType::STANDARD_REFUND], null, false, true, false, $order->id_shop)
```