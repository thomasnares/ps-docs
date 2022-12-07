---
menuTitle: actionObject<ClassName>AddBefore
Title: actionObject<ClassName>AddBefore
hidden: true
hookTitle: 
files:
  - classes/ObjectModel.php
locations:
  - backoffice
  - frontoffice
type:
  - action
hookAliases:
---

# Hook actionObject<ClassName>AddBefore

## Information

Hook locations: 
  - backoffice
  - frontoffice

Hook type: 
  - action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/ObjectModel.php](classes/ObjectModel.php)

## Hook call in codebase

```php
Hook::exec('actionObject' . $this->getFullyQualifiedName() . 'AddBefore', ['object' => $this]);
```