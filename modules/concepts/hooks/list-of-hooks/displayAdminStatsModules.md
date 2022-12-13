---
menuTitle: displayAdminStatsModules
Title: displayAdminStatsModules
hidden: true
hookTitle: Stats - Modules
files:
  - controllers/admin/AdminStatsTabController.php
location:
  - back office
type: display
hookAliases:
 - AdminStatsModules
---

# Hook displayAdminStatsModules

Aliases: 
 - AdminStatsModules



## Information

{{% notice tip %}}
**Stats - Modules:** 


{{% /notice %}}

Hook location:
  - back office

Hook type: display

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/controllers/admin/AdminStatsTabController.php](controllers/admin/AdminStatsTabController.php)

## Call of the Hook in the origin file

```php
Hook::exec('displayAdminStatsModules', [], $module_instance->id)
```