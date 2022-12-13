---
menuTitle: displayProductActions
Title: displayProductActions
hidden: true
hookTitle: Display additional action button on the product page
files:
  - themes/classic/templates/catalog/_partials/product-add-to-cart.tpl
location:
  - front office
type: action
hookAliases:
---

# Hook displayProductActions

## Information

{{% notice tip %}}
**Display additional action button on the product page:** 

This hook allow additional actions to be triggered, near the add to cart button.
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/themes/classic/templates/catalog/_partials/product-add-to-cart.tpl](themes/classic/templates/catalog/_partials/product-add-to-cart.tpl)

## Call of the Hook in the origin file

```php
{hook h='displayProductActions' product=$product}
```