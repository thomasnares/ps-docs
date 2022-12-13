---
menuTitle: actionAdminPreferencesControllerPostProcessBefore
Title: actionAdminPreferencesControllerPostProcessBefore
hidden: true
hookTitle: 
files:
  - src/PrestaShopBundle/Controller/Admin/Configure/ShopParameters/PreferencesController.php
location:
  - back office
type: action
hookAliases:
---

# Hook actionAdminPreferencesControllerPostProcessBefore

## Information

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Controller/Admin/Configure/ShopParameters/PreferencesController.php](src/PrestaShopBundle/Controller/Admin/Configure/ShopParameters/PreferencesController.php)

## Call of the Hook in the origin file

```php
dispatchHook('actionAdminPreferencesControllerPostProcessBefore', ['controller' => $this])
```