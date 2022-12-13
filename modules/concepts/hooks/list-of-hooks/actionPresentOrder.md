---
menuTitle: actionPresentOrder
Title: actionPresentOrder
hidden: true
hookTitle: Order Presenter
files:
  - src/Adapter/Presenter/Order/OrderPresenter.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionPresentOrder

## Information

{{% notice tip %}}
**Order Presenter:** 

This hook is called before an order is presented
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/Adapter/Presenter/Order/OrderPresenter.php](src/Adapter/Presenter/Order/OrderPresenter.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionPresentOrder',
            ['presentedOrder' => &$orderLazyArray]
        )
```