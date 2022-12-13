---
menuTitle: displayback officeTop
Title: displayback officeTop
hidden: true
hookTitle: Administration panel hover the tabs
files:
  - classes/controller/AdminController.php
location:
  - back office
type: display
hookAliases:
 - back officeTop
---

# Hook displayback officeTop

Aliases: 
 - back officeTop



## Information

{{% notice tip %}}
**Administration panel hover the tabs:** 

This hook is displayed on the roll hover of the tabs within the admin panel
{{% /notice %}}

Hook location:
  - back office

Hook type: display

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/controller/AdminController.php](classes/controller/AdminController.php)

## Call of the Hook in the origin file

```php
Hook::exec('displayback officeTop')
```