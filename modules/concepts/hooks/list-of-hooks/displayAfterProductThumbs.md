---
menuTitle: displayAfterProductThumbs
Title: displayAfterProductThumbs
hidden: true
hookTitle: Display extra content below product thumbs
files:
  - themes/classic/templates/catalog/_partials/product-cover-thumbnails.tpl
location:
  - front office
type: display
hookAliases:
---

# Hook displayAfterProductThumbs

## Information

{{% notice tip %}}
**Display extra content below product thumbs:** 

This hook displays new elements below product images ex. additional media
{{% /notice %}}

Hook location:
  - front office

Hook type: display

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/themes/classic/templates/catalog/_partials/product-cover-thumbnails.tpl](themes/classic/templates/catalog/_partials/product-cover-thumbnails.tpl)

## Call of the Hook in the origin file

```php
{hook h='displayAfterProductThumbs' product=$product}
```