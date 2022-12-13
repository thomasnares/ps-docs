---
menuTitle: actionSubmitAccountBefore
Title: actionSubmitAccountBefore
hidden: true
hookTitle: 
files:
  - controllers/front/RegistrationController.php
location:
  - front office
type: action
hookAliases:
 - actionBeforeSubmitAccount
---

# Hook actionSubmitAccountBefore

Aliases: 
 - actionBeforeSubmitAccount



## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/controllers/front/RegistrationController.php](controllers/front/RegistrationController.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionSubmitAccountBefore', [], null, true)
```