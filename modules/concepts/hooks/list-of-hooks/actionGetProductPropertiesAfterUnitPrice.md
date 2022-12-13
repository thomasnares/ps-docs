---
menuTitle: actionGetProductPropertiesAfterUnitPrice
Title: actionGetProductPropertiesAfterUnitPrice
hidden: true
hookTitle: Product Properties
files:
  - classes/Product.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionGetProductPropertiesAfterUnitPrice

## Information

{{% notice tip %}}
**Product Properties:** 

This hook is called after defining the properties of a product
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/Product.php](classes/Product.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionGetProductPropertiesAfterUnitPrice', [
            'id_lang' => $id_lang,
            'product' => &$row,
            'context' => $context,
        ])
```