---
menuTitle: filterSupplierContent
Title: filterSupplierContent
hidden: true
hookTitle: Filter the content page supplier
files:
  - controllers/front/listing/SupplierController.php
location:
  - front office
type: 
hookAliases:
---

# Hook filterSupplierContent

## Information

{{% notice tip %}}
**Filter the content page supplier:** 

This hook is called just before fetching content page supplier
{{% /notice %}}

Hook location:
  - front office

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/controllers/front/listing/SupplierController.php](controllers/front/listing/SupplierController.php)

This hook has a `$chain` parameter set to `true` (hook will chain the return of hook module, [see explaination here]({{< relref "/8/development/components/hook/dispatching-hook">}})).

## Call of the Hook in the origin file

```php
Hook::exec(
            'filterSupplierContent',
            ['object' => $supplierVar],
            $id_module = null,
            $array_return = false,
            $check_exceptions = true,
            $use_push = false,
            $id_shop = null,
            $chain = true
        )
```