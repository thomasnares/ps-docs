---
menuTitle: displayMaintenance
Title: displayMaintenance
hidden: true
hookTitle: Maintenance Page
files:
  - classes/controller/FrontController.php
location:
  - front office
type: display
hookAliases:
---

# Hook displayMaintenance

## Information

{{% notice tip %}}
**Maintenance Page:** 

This hook displays new elements on the maintenance page
{{% /notice %}}

Hook location:
  - front office

Hook type: display

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/controller/FrontController.php](classes/controller/FrontController.php)

## Call of the Hook in the origin file

```php
Hook::exec('displayMaintenance', [])
```