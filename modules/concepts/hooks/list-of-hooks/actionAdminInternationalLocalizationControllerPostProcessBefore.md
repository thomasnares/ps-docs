---
menuTitle: actionAdminInternationalLocalizationControllerPostProcessBefore
Title: actionAdminInternationalLocalizationControllerPostProcessBefore
hidden: true
hookTitle: On post-process in Admin Improve International Localization Controller
files:
  - src/PrestaShopBundle/Controller/Admin/Improve/International/LocalizationController.php
location:
  - back office
type: action
hookAliases:
---

# Hook actionAdminInternationalLocalizationControllerPostProcessBefore

## Information

{{% notice tip %}}
**On post-process in Admin Improve International Localization Controller:** 

This hook is called on Admin Improve International Localization post-process before processing any form
{{% /notice %}}

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Controller/Admin/Improve/International/LocalizationController.php](src/PrestaShopBundle/Controller/Admin/Improve/International/LocalizationController.php)

## Call of the Hook in the origin file

```php
dispatchHook('actionAdminInternationalLocalizationControllerPostProcessBefore', ['controller' => $this])
```