---
menuTitle: actionAttributeSave
Title: actionAttributeSave
hidden: true
hookTitle: Saving an attributes features value
files:
  - classes/ProductAttribute.php
location:
  - front office
type: action
hookAliases:
 - afterSaveAttribute
---

# Hook actionAttributeSave

Aliases: 
 - afterSaveAttribute



## Information

{{% notice tip %}}
**Saving an attributes features value:** 

This hook is called while saving an attributes features value
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/ProductAttribute.php](classes/ProductAttribute.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionAttributeSave', ['id_attribute' => $this->id])
```