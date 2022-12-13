---
menuTitle: displayAdminOrderSideBottom
Title: displayAdminOrderSideBottom
hidden: true
hookTitle: 
files:
  - src/PrestaShopBundle/Resources/views/Admin/Sell/Order/Order/view.html.twig
location:
  - back office
type: display
hookAliases:
---

# Hook displayAdminOrderSideBottom

## Information

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
{{ renderhook('displayAdminOrderSideBottom', {'id_order': orderForViewing.id}) }}
```