---
menuTitle: actionAdminLoginControllerResetAfter
Title: actionAdminLoginControllerResetAfter
hidden: true
hookTitle: Perform actions after admin login controller reset action initialization
files:
  - controllers/admin/AdminLoginController.php
location:
  - back office
type: action
hookAliases:
---

# Hook actionAdminLoginControllerResetAfter

## Information

{{% notice tip %}}
**Perform actions after admin login controller reset action initialization:** 

This hook is launched after the initialization of the reset action in login controller
{{% /notice %}}

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/controllers/admin/AdminLoginController.php](controllers/admin/AdminLoginController.php)

## Call of the Hook in the origin file

```php
Hook::exec(
                        'actionAdminLoginControllerResetAfter',
                        [
                            'controller' => $this,
                            'employee' => $employee,
                        ]
                    )
```