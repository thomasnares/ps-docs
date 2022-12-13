---
menuTitle: actionFeatureValueSave
Title: actionFeatureValueSave
hidden: true
hookTitle: Saving an attributes features value
files:
  - classes/FeatureValue.php
location:
  - front office
type: action
hookAliases:
 - afterSaveFeatureValue
---

# Hook actionFeatureValueSave

Aliases: 
 - afterSaveFeatureValue



## Information

{{% notice tip %}}
**Saving an attributes features value:** 

This hook is called while saving an attributes features value
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/FeatureValue.php](classes/FeatureValue.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionFeatureValueSave', ['id_feature_value' => $this->id])
```