---
menuTitle: actionProductCoverage
Title: actionProductCoverage
hidden: true
hookTitle: 
files:
  - classes/stock/StockManager.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionProductCoverage

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/stock/StockManager.php](classes/stock/StockManager.php)

## Call of the Hook in the origin file

```php
Hook::exec(
                'actionProductCoverage',
                    [
                        'id_product' => $id_product,
                        'id_product_attribute' => $id_product_attribute,
                        'warehouse' => $warehouse,
                    ]
            )
```