---
menuTitle: actionFeatureValueDelete
Title: actionFeatureValueDelete
hidden: true
hookTitle: Deleting attributes' features' values
files:
  - classes/FeatureValue.php
location:
  - front office
type: action
hookAliases:
 - afterDeleteFeatureValue
---

# Hook actionFeatureValueDelete

Aliases: 
 - afterDeleteFeatureValue



## Information

{{% notice tip %}}
**Deleting attributes' features' values:** 

This hook is called while deleting an attributes features value
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/FeatureValue.php](classes/FeatureValue.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionFeatureValueDelete', ['id_feature_value' => $this->id])
```