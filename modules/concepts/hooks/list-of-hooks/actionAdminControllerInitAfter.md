---
menuTitle: actionAdminControllerInitAfter
Title: actionAdminControllerInitAfter
hidden: true
hookTitle: Perform actions after admin controller initialization
files:
  - classes/controller/AdminController.php
location:
  - back office
type: action
hookAliases:
---

# Hook actionAdminControllerInitAfter

## Information

{{% notice tip %}}
**Perform actions after admin controller initialization:** 

This hook is launched after the initialization of all admin controllers
{{% /notice %}}

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/controller/AdminController.php](classes/controller/AdminController.php)

## Call of the Hook in the origin file

```php
Hook::exec(
            'actionAdminControllerInitAfter',
            [
                'controller' => $this,
            ]
        )
```