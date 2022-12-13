---
menuTitle: actionCartUpdateQuantityBefore
Title: actionCartUpdateQuantityBefore
hidden: true
hookTitle: 
files:
  - classes/Cart.php
location:
  - front office
type: action
hookAliases:
 - actionBeforeCartUpdateQty
---

# Hook actionCartUpdateQuantityBefore

Aliases: 
 - actionBeforeCartUpdateQty



## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/Cart.php](classes/Cart.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionCartUpdateQuantityBefore', $data)
```