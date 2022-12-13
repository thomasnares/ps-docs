---
menuTitle: displayFeatureValuePostProcess
Title: displayFeatureValuePostProcess
hidden: true
hookTitle: On post-process in admin feature value
files:
  - controllers/admin/AdminFeaturesController.php
location:
  - back office
type: display
hookAliases:
 - postProcessFeatureValue
---

# Hook displayFeatureValuePostProcess

Aliases: 
 - postProcessFeatureValue



## Information

{{% notice tip %}}
**On post-process in admin feature value:** 

This hook is called on post-process in admin feature value
{{% /notice %}}

Hook location:
  - back office

Hook type: display

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/controllers/admin/AdminFeaturesController.php](controllers/admin/AdminFeaturesController.php)

## Call of the Hook in the origin file

```php
Hook::exec(
                'displayFeatureValuePostProcess',
                ['errors' => &$this->errors]
            )
```