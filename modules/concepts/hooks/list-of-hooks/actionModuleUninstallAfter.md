---
menuTitle: actionModuleUninstallAfter
Title: actionModuleUninstallAfter
hidden: true
hookTitle: actionModuleUninstallAfter
files:
  - classes/module/Module.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionModuleUninstallAfter

## Information

{{% notice tip %}}
**actionModuleUninstallAfter:** 


{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/module/Module.php](classes/module/Module.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionModuleUninstallAfter', ['object' => $this])
```