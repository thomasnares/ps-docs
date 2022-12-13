---
menuTitle: actionPresentOrderReturn
Title: actionPresentOrderReturn
hidden: true
hookTitle: Order Return Presenter
files:
  - src/Adapter/Presenter/Order/OrderReturnPresenter.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionPresentOrderReturn

## Information

{{% notice tip %}}
**Order Return Presenter:** 

This hook is called before an order return is presented
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/Adapter/Presenter/Order/OrderReturnPresenter.php](src/Adapter/Presenter/Order/OrderReturnPresenter.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionPresentOrderReturn',
            ['presentedOrderReturn' => &$orderReturnLazyArray]
        )
```