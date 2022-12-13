---
menuTitle: actionProductActivation
Title: actionProductActivation
hidden: true
hookTitle: 
files:
  - src/Adapter/Product/AdminProductDataUpdater.php
location:
  - back office
type: action
hookAliases:
---

# Hook actionProductActivation

## Information

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/Adapter/Product/AdminProductDataUpdater.php](src/Adapter/Product/AdminProductDataUpdater.php)

## Call of the Hook in the origin file

```php
dispatchWithParameters('actionProductActivation', ['id_product' => (int) $product->id, 'product' => $product, 'activated' => $activate])
```