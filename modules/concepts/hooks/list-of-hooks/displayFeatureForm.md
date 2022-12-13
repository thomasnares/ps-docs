---
menuTitle: displayFeatureForm
Title: displayFeatureForm
hidden: true
hookTitle: Add fields to the form 'feature'
files:
  - src/PrestaShopBundle/Resources/views/Admin/Sell/Catalog/Features/Blocks/form.html.twig
location:
  - back office
type: display
hookAliases:
 - featureForm
---

# Hook displayFeatureForm

Aliases: 
 - featureForm



## Information

{{% notice tip %}}
**Add fields to the form 'feature':** 

This hook adds fields to the form 'feature'
{{% /notice %}}

Hook location:
  - back office

Hook type: display

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Resources/views/Admin/Sell/Catalog/Features/Blocks/form.html.twig](src/PrestaShopBundle/Resources/views/Admin/Sell/Catalog/Features/Blocks/form.html.twig)

## Call of the Hook in the origin file

```php
{{ renderhook('displayFeatureForm', {'id_feature': featureId}) }}
```