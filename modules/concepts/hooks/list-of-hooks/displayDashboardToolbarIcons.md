---
menuTitle: displayDashboardToolbarIcons
Title: displayDashboardToolbarIcons
hidden: true
hookTitle: Display new elements in back office page with dashboard, on icons list
files:
  - src/PrestaShopBundle/Resources/views/Admin/Product/CatalogPage/Blocks/tools.html.twig
location:
  - back office
type: display
hookAliases:
---

# Hook displayDashboardToolbarIcons

## Information

{{% notice tip %}}
**Display new elements in back office page with dashboard, on icons list:** 

This hook launches modules when the back office with dashboard is displayed
{{% /notice %}}

Hook location:
  - back office

Hook type: display

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Resources/views/Admin/Product/CatalogPage/Blocks/tools.html.twig](src/PrestaShopBundle/Resources/views/Admin/Product/CatalogPage/Blocks/tools.html.twig)

## Call of the Hook in the origin file

```php
{{ renderhook('displayDashboardToolbarIcons', {}) }}
```