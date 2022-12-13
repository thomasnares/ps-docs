---
menuTitle: actionGetProductPropertiesAfter
Title: actionGetProductPropertiesAfter
hidden: true
hookTitle: 
files:
  - classes/Product.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionGetProductPropertiesAfter

## Information

{{% notice warning %}}
**Deprecated:** Since 1.7.8.0
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/Product.php](classes/Product.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionGetProductPropertiesAfter', [
            'id_lang' => $id_lang,
            'product' => &$row,
            'context' => $context,
        ])
```