---
menuTitle: actionCustomerLogoutBefore
Title: actionCustomerLogoutBefore
hidden: true
hookTitle: Before customer logout
files:
  - classes/Customer.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionCustomerLogoutBefore

## Information

{{% notice tip %}}
**Before customer logout:** 

This hook allows you to execute code before customer logout
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/Customer.php](classes/Customer.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionCustomerLogoutBefore', ['customer' => $this])
```