---
menuTitle: actionWatermark
Title: actionWatermark
hidden: true
hookTitle: Watermark
files:
  - src/Adapter/Product/Image/Uploader/ProductImageUploader.php
location:
  - front office
type: action
hookAliases:
 - watermark
---

# Hook actionWatermark

Aliases: 
 - watermark



## Information

{{% notice tip %}}
**Watermark:** 


{{% /notice %}}

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/Adapter/Product/Image/Uploader/ProductImageUploader.php](src/Adapter/Product/Image/Uploader/ProductImageUploader.php)

## Parameters details

```php
    <?php
    array(
      'id_image' => (int) Image ID,
      'id_product' => (int) Product ID
    );
```

## Call of the Hook in the origin file

```php
dispatchWithParameters(
            'actionWatermark',
            ['id_image' => $imageId->getValue(), 'id_product' => $productId]
        )
```