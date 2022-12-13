---
menuTitle: displayAdminProductsQuantitiesStepBottom
Title: displayAdminProductsQuantitiesStepBottom
hidden: true
hookTitle: Display new elements in back office product page, Quantities/Combinations tab
files:
  - src/PrestaShopBundle/Resources/views/Admin/Product/ProductPage/Panels/combinations.html.twig
location:
  - back office
type: display
hookAliases:
---

# Hook displayAdminProductsQuantitiesStepBottom

## Information

{{% notice tip %}}
**Display new elements in back office product page, Quantities/Combinations tab:** 

This hook launches modules when the back office product page is displayed
{{% /notice %}}

Hook location:
  - back office

Hook type: display

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Resources/views/Admin/Product/ProductPage/Panels/combinations.html.twig](src/PrestaShopBundle/Resources/views/Admin/Product/ProductPage/Panels/combinations.html.twig)

## Call of the Hook in the origin file

```php
{{ renderhook('displayAdminProductsQuantitiesStepBottom', { 'id_product': productId }) }}
```