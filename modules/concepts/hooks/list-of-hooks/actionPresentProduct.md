---
menuTitle: actionPresentProduct
Title: actionPresentProduct
hidden: true
hookTitle: Product Presenter
files:
  - src/Adapter/Presenter/Product/ProductPresenter.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionPresentProduct

## Information

{{% notice tip %}}
**Product Presenter:** 

This hook is called before a product is presented
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/Adapter/Presenter/Product/ProductPresenter.php](src/Adapter/Presenter/Product/ProductPresenter.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionPresentProduct',
            ['presentedProduct' => &$productLazyArray]
        )
```