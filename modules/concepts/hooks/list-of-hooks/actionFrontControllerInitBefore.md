---
menuTitle: actionFrontControllerInitBefore
Title: actionFrontControllerInitBefore
hidden: true
hookTitle: Perform actions before front office controller initialization
files:
  - classes/controller/FrontController.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionFrontControllerInitBefore

## Information

{{% notice tip %}}
**Perform actions before front office controller initialization:** 

This hook is launched before the initialization of all front office controllers
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/controller/FrontController.php](classes/controller/FrontController.php)

## Call of the Hook in the origin file

```php
Hook::exec(
            'actionFrontControllerInitBefore',
            [
                'controller' => $this,
            ]
        )
```