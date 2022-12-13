---
menuTitle: actionAdminShippingPreferencesControllerPostProcessHandlingBefore
Title: actionAdminShippingPreferencesControllerPostProcessHandlingBefore
hidden: true
hookTitle: On post-process in Admin Improve Shipping Preferences Controller
files:
  - src/PrestaShopBundle/Controller/Admin/Improve/Shipping/PreferencesController.php
location:
  - back office
type: action
hookAliases:
---

# Hook actionAdminShippingPreferencesControllerPostProcessHandlingBefore

## Information

{{% notice tip %}}
**On post-process in Admin Improve Shipping Preferences Controller:** 

This hook is called on Admin Improve Shipping Preferences post-process before processing the Handling form
{{% /notice %}}

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Controller/Admin/Improve/Shipping/PreferencesController.php](src/PrestaShopBundle/Controller/Admin/Improve/Shipping/PreferencesController.php)

## Call of the Hook in the origin file

```php
dispatchHook(
            'actionAdminShippingPreferencesControllerPostProcessHandlingBefore',
            ['controller' => $this]
        )
```