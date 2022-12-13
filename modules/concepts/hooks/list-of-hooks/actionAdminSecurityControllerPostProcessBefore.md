---
menuTitle: actionAdminSecurityControllerPostProcessBefore
Title: actionAdminSecurityControllerPostProcessBefore
hidden: true
hookTitle: On post-process in Admin Security Controller
files:
  - src/PrestaShopBundle/Controller/Admin/Configure/AdvancedParameters/SecurityController.php
location:
  - back office
type: action
hookAliases:
---

# Hook actionAdminSecurityControllerPostProcessBefore

## Information

{{% notice tip %}}
**On post-process in Admin Security Controller:** 

This hook is called on Admin Security Controller post-process before processing any form
{{% /notice %}}

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Controller/Admin/Configure/AdvancedParameters/SecurityController.php](src/PrestaShopBundle/Controller/Admin/Configure/AdvancedParameters/SecurityController.php)

## Call of the Hook in the origin file

```php
dispatchHook('actionAdminSecurityControllerPostProcessBefore', ['controller' => $this])
```