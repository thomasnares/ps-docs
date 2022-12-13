---
menuTitle: actionMailAlterMessageBeforeSend
Title: actionMailAlterMessageBeforeSend
hidden: true
hookTitle: 
files:
  - classes/Mail.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionMailAlterMessageBeforeSend

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/Mail.php](classes/Mail.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionMailAlterMessageBeforeSend', [
                'message' => &$message,
            ])
```