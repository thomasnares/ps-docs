---
menuTitle: displayback officeHeader
Title: displayback officeHeader
hidden: true
hookTitle: Administration panel header
files:
  - classes/controller/AdminController.php
location:
  - back office
type: display
hookAliases:
 - back officeHeader
---

# Hook displayback officeHeader

Aliases: 
 - back officeHeader



## Information

{{% notice tip %}}
**Administration panel header:** 

This hook is displayed in the header of the admin panel
{{% /notice %}}

Hook location:
  - back office

Hook type: display

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/controller/AdminController.php](classes/controller/AdminController.php)

## Call of the Hook in the origin file

```php
Hook::exec('displayback officeHeader')
```