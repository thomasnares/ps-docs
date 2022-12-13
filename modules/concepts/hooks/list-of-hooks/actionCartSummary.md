---
menuTitle: actionCartSummary
Title: actionCartSummary
hidden: true
hookTitle: 
files:
  - classes/Cart.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionCartSummary

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/Cart.php](classes/Cart.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionCartSummary', $summary, null, true)
```