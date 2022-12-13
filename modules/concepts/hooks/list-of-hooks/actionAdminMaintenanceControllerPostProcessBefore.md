---
menuTitle: actionAdminMaintenanceControllerPostProcessBefore
Title: actionAdminMaintenanceControllerPostProcessBefore
hidden: true
hookTitle: 
files:
  - src/PrestaShopBundle/Controller/Admin/Configure/ShopParameters/MaintenanceController.php
location:
  - back office
type: action
hookAliases:
---

# Hook actionAdminMaintenanceControllerPostProcessBefore

## Information

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Controller/Admin/Configure/ShopParameters/MaintenanceController.php](src/PrestaShopBundle/Controller/Admin/Configure/ShopParameters/MaintenanceController.php)

## Call of the Hook in the origin file

```php
dispatchHook('actionAdminMaintenanceControllerPostProcessBefore', ['controller' => $this])
```