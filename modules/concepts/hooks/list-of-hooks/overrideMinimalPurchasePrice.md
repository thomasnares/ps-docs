---
menuTitle: overrideMinimalPurchasePrice
Title: overrideMinimalPurchasePrice
hidden: true
hookTitle: 
files:
  - src/Adapter/Presenter/Cart/CartPresenter.php
location:
  - front office
type: 
hookAliases:
---

# Hook overrideMinimalPurchasePrice

## Information

Hook location:
  - front office

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/Adapter/Presenter/Cart/CartPresenter.php](src/Adapter/Presenter/Cart/CartPresenter.php)

## Call of the Hook in the origin file

```php
Hook::exec('overrideMinimalPurchasePrice', [
            'minimalPurchase' => &$minimalPurchase,
        ])
```