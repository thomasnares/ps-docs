---
menuTitle: displayFooterProduct
Title: displayFooterProduct
hidden: true
hookTitle: Product footer
files:
  - themes/classic/templates/catalog/product.tpl
location:
  - front office
type: display
hookAliases:
 - productfooter
---

# Hook displayFooterProduct

Aliases: 
 - productfooter



## Information

{{% notice tip %}}
**Product footer:** 

This hook adds new blocks under the product's description
{{% /notice %}}

Hook location:
  - front office

Hook type: display

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/themes/classic/templates/catalog/product.tpl](themes/classic/templates/catalog/product.tpl)

## Call of the Hook in the origin file

```php
{hook h='displayFooterProduct' product=$product category=$category}
```