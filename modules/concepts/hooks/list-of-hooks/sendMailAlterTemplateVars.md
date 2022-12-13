---
menuTitle: sendMailAlterTemplateVars
Title: sendMailAlterTemplateVars
hidden: true
hookTitle: Alter template vars on the fly
files:
  - classes/Mail.php
location:
  - front office
type: 
hookAliases:
---

# Hook sendMailAlterTemplateVars

## Information

{{% notice tip %}}
**Alter template vars on the fly:** 

This hook is called when Mail::send() is called
{{% /notice %}}

Hook location:
  - front office

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/Mail.php](classes/Mail.php)

## Call of the Hook in the origin file

```php
Hook::exec(
            'sendMailAlterTemplateVars',
            [
                'template' => $template,
                'template_vars' => &$templateVars,
            ]
        )
```