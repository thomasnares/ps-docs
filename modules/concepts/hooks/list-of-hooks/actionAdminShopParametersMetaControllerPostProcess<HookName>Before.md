---
menuTitle: actionAdminShopParametersMetaControllerPostProcess<HookName>Before
Title: actionAdminShopParametersMetaControllerPostProcess<HookName>Before
hidden: true
hookTitle: 
files:
  - src/PrestaShopBundle/Controller/Admin/Configure/ShopParameters/MetaController.php
location:
  - back office
type: action
hookAliases:
---

# Hook actionAdminShopParametersMetaControllerPostProcess<HookName>Before

## Information

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Controller/Admin/Configure/ShopParameters/MetaController.php](src/PrestaShopBundle/Controller/Admin/Configure/ShopParameters/MetaController.php)

## Call of the Hook in the origin file

```php
dispatchHook(
            'actionAdminShopParametersMetaControllerPostProcess' . $hookName . 'Before',
            ['controller' => $this]
        )
```