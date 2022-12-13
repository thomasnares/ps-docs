---
menuTitle: actionPresentCart
Title: actionPresentCart
hidden: true
hookTitle: Cart Presenter
files:
  - src/Adapter/Presenter/Cart/CartPresenter.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionPresentCart

## Information

{{% notice tip %}}
**Cart Presenter:** 

This hook is called before a cart is presented
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/Adapter/Presenter/Cart/CartPresenter.php](src/Adapter/Presenter/Cart/CartPresenter.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionPresentCart',
            ['presentedCart' => &$result]
        )
```