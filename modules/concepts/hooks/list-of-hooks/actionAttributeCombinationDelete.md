---
menuTitle: actionAttributeCombinationDelete
Title: actionAttributeCombinationDelete
hidden: true
hookTitle: 
files:
  - classes/Combination.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionAttributeCombinationDelete

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/Combination.php](classes/Combination.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionAttributeCombinationDelete', ['id_product_attribute' => (int) $this->id])
```