---
menuTitle: actionAdmin<Action>After
Title: actionAdmin<Action>After
hidden: true
hookTitle: 
files:
  - classes/controller/AdminController.php
location:
  - back office
type: action
hookAliases:
---

# Hook actionAdmin<Action>After

## Information

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/controller/AdminController.php](classes/controller/AdminController.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionAdmin' . ucfirst($this->action) . 'After', ['controller' => $this, 'return' => $return]);
```