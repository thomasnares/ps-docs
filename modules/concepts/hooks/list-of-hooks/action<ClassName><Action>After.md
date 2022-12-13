---
menuTitle: action<ClassName><Action>After
Title: action<ClassName><Action>After
hidden: true
hookTitle: 
files:
  - classes/controller/AdminController.php
location:
  - back office
type: action
hookAliases:
---

# Hook action&lt;ClassName>&lt;Action>After

## Information

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/controller/AdminController.php](classes/controller/AdminController.php)

## Call of the Hook in the origin file

```php
Hook::exec('action' . get_class($this) . ucfirst($this->action) . 'After', ['controller' => $this, 'return' => $return]);
```