---
menuTitle: actionCustomerAddGroups
Title: actionCustomerAddGroups
hidden: true
hookTitle: 
files:
  - classes/Customer.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionCustomerAddGroups

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/Customer.php](classes/Customer.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionCustomerAddGroups', ['id_customer' => $this->id, 'groups' => $groups])
```