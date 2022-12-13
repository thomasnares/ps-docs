---
menuTitle: actionFeatureSave
Title: actionFeatureSave
hidden: true
hookTitle: Saving attributes' features
files:
  - classes/Feature.php
location:
  - front office
type: action
hookAliases:
 - afterSaveFeature
---

# Hook actionFeatureSave

Aliases: 
 - afterSaveFeature



## Information

{{% notice tip %}}
**Saving attributes' features:** 

This hook is called while saving an attributes features
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/Feature.php](classes/Feature.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionFeatureSave', ['id_feature' => $this->id])
```