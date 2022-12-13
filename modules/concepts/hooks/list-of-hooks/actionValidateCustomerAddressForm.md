---
menuTitle: actionValidateCustomerAddressForm
Title: actionValidateCustomerAddressForm
hidden: true
hookTitle: Customer address form validation
files:
  - classes/form/CustomerAddressForm.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionValidateCustomerAddressForm

## Information

{{% notice tip %}}
**Customer address form validation:** 

This hook is called when a customer submit its address form
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/form/CustomerAddressForm.php](classes/form/CustomerAddressForm.php)

## Parameters details

```php
    <?php
    array(
      'form' => (object) CustomerAddressForm
    );
```

## Call of the Hook in the origin file

```php
Hook::exec('actionValidateCustomerAddressForm', ['form' => $this])
```