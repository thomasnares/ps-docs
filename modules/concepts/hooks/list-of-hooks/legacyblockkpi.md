---
menuTitle: legacyblockkpi
Title: legacyblockkpi
hidden: true
hookTitle: 
files:
  - src/PrestaShopBundle/Resources/views/Admin/Product/CatalogPage/catalog.html.twig
location:
  - back office
type: 
hookAliases:
---

# Hook legacyblockkpi

## Information

Hook location:
  - back office

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Resources/views/Admin/Product/CatalogPage/catalog.html.twig](src/PrestaShopBundle/Resources/views/Admin/Product/CatalogPage/catalog.html.twig)

## Call of the Hook in the origin file

```php
{{ renderhook('legacy_block_kpi', {'kpi_controller': 'AdminProductsController'}) }}
```