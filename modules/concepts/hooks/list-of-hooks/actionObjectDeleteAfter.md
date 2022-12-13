---
menuTitle: actionObjectDeleteAfter
Title: actionObjectDeleteAfter
hidden: true
hookTitle: 
files:
  - classes/ObjectModel.php
location:
  - back office
  - front office
type: action
hookAliases:
---

# Hook actionObjectDeleteAfter

## Information

Hook location:
  - back office
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/ObjectModel.php](classes/ObjectModel.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionObjectDeleteAfter', ['object' => $this])
```