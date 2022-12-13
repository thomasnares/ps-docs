---
menuTitle: displayAdminCustomers
Title: displayAdminCustomers
hidden: true
hookTitle: Display new elements in the Back Office, tab AdminCustomers
files:
  - src/PrestaShopBundle/Resources/views/Admin/Sell/Customer/view.html.twig
location:
  - back office
type: display
hookAliases:
 - adminCustomers
---

# Hook displayAdminCustomers

Aliases: 
 - adminCustomers



## Information

{{% notice tip %}}
**Display new elements in the Back Office, tab AdminCustomers:** 

This hook launches modules when the AdminCustomers tab is displayed in the Back Office
{{% /notice %}}

Hook location:
  - back office

Hook type: display

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Resources/views/Admin/Sell/Customer/view.html.twig](src/PrestaShopBundle/Resources/views/Admin/Sell/Customer/view.html.twig)

## Parameters details

```php
    <?php
    array(
      'id_customer' = (int) Customer ID
    );
```

## Call of the Hook in the origin file

```php
{{ renderhook('displayAdminCustomers', {'id_customer': customerInformation.customerId.value}) }}
```