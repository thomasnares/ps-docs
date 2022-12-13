---
menuTitle: actionOverrideEmployeeImage
Title: actionOverrideEmployeeImage
hidden: true
hookTitle: Get Employee Image
files:
  - classes/Employee.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionOverrideEmployeeImage

## Information

{{% notice tip %}}
**Get Employee Image:** 

This hook is used to get the employee image
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/Employee.php](classes/Employee.php)

## Call of the Hook in the origin file

```php
Hook::exec(
            'actionOverrideEmployeeImage',
            [
                'employee' => $this,
                'imageUrl' => &$imageUrl,
            ]
        )
```