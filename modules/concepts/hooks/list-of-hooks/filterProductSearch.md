---
menuTitle: filterProductSearch
Title: filterProductSearch
hidden: true
hookTitle: Filter search products result
files:
  - modules/blockwishlist/controllers/front/view.php
location:
  - front office
type: 
hookAliases:
---

# Hook filterProductSearch

## Information

{{% notice tip %}}
**Filter search products result:** 

This hook is called in order to allow to modify search product result
{{% /notice %}}

Hook location:
  - front office

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/modules/blockwishlist/controllers/front/view.php](modules/blockwishlist/controllers/front/view.php)

## Call of the Hook in the origin file

```php
Hook::exec('filterProductSearch', ['searchVariables' => &$searchVariables])
```