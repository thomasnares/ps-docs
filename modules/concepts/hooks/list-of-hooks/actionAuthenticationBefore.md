---
menuTitle: actionAuthenticationBefore
Title: actionAuthenticationBefore
hidden: true
hookTitle: 
files:
  - classes/form/CustomerLoginForm.php
location:
  - front office
type: action
hookAliases:
 - actionBeforeAuthentication
---

# Hook actionAuthenticationBefore

Aliases: 
 - actionBeforeAuthentication



## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/form/CustomerLoginForm.php](classes/form/CustomerLoginForm.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionAuthenticationBefore')
```