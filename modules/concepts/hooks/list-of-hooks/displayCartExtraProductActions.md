---
menuTitle: displayCartExtraProductActions
Title: displayCartExtraProductActions
hidden: true
hookTitle: Extra buttons in shopping cart
files:
  - themes/classic/templates/checkout/_partials/cart-detailed-product-line.tpl
location:
  - front office
type: action
hookAliases:
---

# Hook displayCartExtraProductActions

## Information

{{% notice tip %}}
**Extra buttons in shopping cart:** 

This hook adds extra buttons to the product lines, in the shopping cart
{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/themes/classic/templates/checkout/_partials/cart-detailed-product-line.tpl](themes/classic/templates/checkout/_partials/cart-detailed-product-line.tpl)

## Call of the Hook in the origin file

```php
{hook h='displayCartExtraProductActions' product=$product}
```