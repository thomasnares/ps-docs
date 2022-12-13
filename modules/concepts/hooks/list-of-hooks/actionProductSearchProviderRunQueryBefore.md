---
menuTitle: actionProductSearchProviderRunQueryBefore
Title: actionProductSearchProviderRunQueryBefore
hidden: true
hookTitle: Runs an action before ProductSearchProviderInterface::RunQuery()
files:
  - classes/controller/ProductListingFrontController.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionProductSearchProviderRunQueryBefore

## Information

{{% notice tip %}}
**Runs an action before ProductSearchProviderInterface::RunQuery():** 

Required to modify an SQL query before executing it
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/controller/ProductListingFrontController.php](classes/controller/ProductListingFrontController.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionProductSearchProviderRunQueryBefore', [
            'query' => $query,
        ])
```