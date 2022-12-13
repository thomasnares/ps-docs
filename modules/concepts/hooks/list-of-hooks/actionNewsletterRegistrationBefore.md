---
menuTitle: actionNewsletterRegistrationBefore
Title: actionNewsletterRegistrationBefore
hidden: true
hookTitle: 
files:
  - modules/ps_emailsubscription/ps_emailsubscription.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionNewsletterRegistrationBefore

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/modules/ps_emailsubscription/ps_emailsubscription.php](modules/ps_emailsubscription/ps_emailsubscription.php)

## Call of the Hook in the origin file

```php
Hook::exec(
            'actionNewsletterRegistrationBefore',
            [
                'hookName' => $hookName,
                'email' => $_POST['email'],
                'action' => $_POST['action'],
                'hookError' => &$hookError,
            ]
        )
```