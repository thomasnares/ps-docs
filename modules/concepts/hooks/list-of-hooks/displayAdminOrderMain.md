---
menuTitle: displayAdminOrderMain
Title: displayAdminOrderMain
hidden: true
hookTitle: Admin Order Main Column
files:
  - src/PrestaShopBundle/Resources/views/Admin/Sell/Order/Order/view.html.twig
location:
  - back office
type: display
hookAliases:
---

# Hook displayAdminOrderMain

## Information

{{% notice tip %}}
**Admin Order Main Column:** 

This hook displays content in the order view page in the main column under the details view
{{% /notice %}}

Hook location:
  - back office

Hook type: display

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Resources/views/Admin/Sell/Order/Order/view.html.twig](src/PrestaShopBundle/Resources/views/Admin/Sell/Order/Order/view.html.twig)

## Parameters details

```php
    <?php
    array(
      'id_order' => (int) Order ID
    );
```

## Call of the Hook in the origin file

```php
{{ renderhook('displayAdminOrderMain', {'id_order': orderForViewing.id}) }}
```