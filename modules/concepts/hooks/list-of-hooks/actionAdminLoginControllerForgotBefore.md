---
menuTitle: actionAdminLoginControllerForgotBefore
Title: actionAdminLoginControllerForgotBefore
hidden: true
hookTitle: Perform actions before admin login controller forgot action initialization
files:
  - controllers/admin/AdminLoginController.php
location:
  - back office
type: action
hookAliases:
---

# Hook actionAdminLoginControllerForgotBefore

## Information

{{% notice tip %}}
**Perform actions before admin login controller forgot action initialization:** 

This hook is launched before the initialization of the forgot action in login controller
{{% /notice %}}

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/controllers/admin/AdminLoginController.php](controllers/admin/AdminLoginController.php)

## Call of the Hook in the origin file

```php
Hook::exec(
            'actionAdminLoginControllerForgotBefore',
            [
                'controller' => $this,
                'email' => $email,
            ]
        )
```