---
menuTitle: actionAdminShopParametersProductPreferencesControllerPostProcess<HookName>Before
Title: actionAdminShopParametersProductPreferencesControllerPostProcess<HookName>Before
hidden: true
hookTitle: 
files:
  - src/PrestaShopBundle/Controller/Admin/Configure/ShopParameters/ProductPreferencesController.php
location:
  - back office
type: action
hookAliases:
---

# Hook actionAdminShopParametersProductPreferencesControllerPostProcess&lt;HookName>Before

## Information

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Controller/Admin/Configure/ShopParameters/ProductPreferencesController.php](src/PrestaShopBundle/Controller/Admin/Configure/ShopParameters/ProductPreferencesController.php)

## Call of the Hook in the origin file

```php
dispatchHook(
            'actionAdminShopParametersProductPreferencesControllerPostProcess' . $hookName . 'Before',
            ['controller' => $this]
        )
```