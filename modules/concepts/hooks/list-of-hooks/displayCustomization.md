---
menuTitle: displayCustomization
Title: displayCustomization
hidden: true
hookTitle: 
files:
  - classes/Product.php
location:
  - front office
type: display
hookAliases:
---

# Hook displayCustomization

## Information

Hook location:
  - front office

Hook type: display

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/Product.php](classes/Product.php)

## Call of the Hook in the origin file

```php
Hook::exec('displayCustomization', ['customization' => $row], (int) $row['id_module'])
```