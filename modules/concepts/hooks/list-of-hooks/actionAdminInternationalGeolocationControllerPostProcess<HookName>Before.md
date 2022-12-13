---
menuTitle: actionAdminInternationalGeolocationControllerPostProcess<HookName>Before
Title: actionAdminInternationalGeolocationControllerPostProcess<HookName>Before
hidden: true
hookTitle: 
files:
  - src/PrestaShopBundle/Controller/Admin/Improve/International/GeolocationController.php
location:
  - back office
type: action
hookAliases:
---

# Hook actionAdminInternationalGeolocationControllerPostProcess&lt;HookName>Before

## Information

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Controller/Admin/Improve/International/GeolocationController.php](src/PrestaShopBundle/Controller/Admin/Improve/International/GeolocationController.php)

## Call of the Hook in the origin file

```php
dispatchHook(
            'actionAdminInternationalGeolocationControllerPostProcess' . $hookName . 'Before',
            ['controller' => $this]
        )
```