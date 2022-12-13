---
menuTitle: productSearchProvider
Title: productSearchProvider
hidden: true
hookTitle: 
files:
  - classes/controller/ProductListingFrontController.php
location:
  - front office
type: 
hookAliases:
---

# Hook productSearchProvider

## Information

Hook location:
  - front office

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/controller/ProductListingFrontController.php](classes/controller/ProductListingFrontController.php)

This hook has an `$array_return` parameter set to `true` (module output will be set by name in an array, [see explaination here]({{< relref "/8/development/components/hook/dispatching-hook">}})).

## Call of the Hook in the origin file

```php
Hook::exec(
            'productSearchProvider',
            ['query' => $query],
            null,
            true
        )
```