---
menuTitle: actionGetIDZoneByAddressID
Title: actionGetIDZoneByAddressID
hidden: true
hookTitle: 
files:
  - classes/Address.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionGetIDZoneByAddressID

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/Address.php](classes/Address.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionGetIDZoneByAddressID', ['id_address' => $id_address])
```