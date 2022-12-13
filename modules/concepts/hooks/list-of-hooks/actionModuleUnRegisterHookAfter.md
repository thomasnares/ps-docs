---
menuTitle: actionModuleUnRegisterHookAfter
Title: actionModuleUnRegisterHookAfter
hidden: true
hookTitle: 
files:
  - classes/Hook.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionModuleUnRegisterHookAfter

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/Hook.php](classes/Hook.php)

## Call of the Hook in the origin file

```php
Hook::exec(
            'actionModuleUnRegisterHookAfter',
            [
                'object' => $module_instance,
                'hook_name' => $hook_name,
            ]
        )
```