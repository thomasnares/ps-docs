---
menuTitle: actionSubmitCustomerAddressForm
Title: actionSubmitCustomerAddressForm
hidden: true
hookTitle: 
files:
  - classes/form/CustomerAddressForm.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionSubmitCustomerAddressForm

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/form/CustomerAddressForm.php](classes/form/CustomerAddressForm.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionSubmitCustomerAddressForm', ['address' => &$address])
```