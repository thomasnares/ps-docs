---
menuTitle: overrideLayoutTemplate
Title: overrideLayoutTemplate
hidden: true
hookTitle: 
files:
  - classes/controller/FrontController.php
location:
  - front office
type: 
hookAliases:
---

# Hook overrideLayoutTemplate

## Information

Hook location:
  - front office

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/controller/FrontController.php](classes/controller/FrontController.php)

## Call of the Hook in the origin file

```php
Hook::exec(
            'overrideLayoutTemplate',
            [
                'default_layout' => $layout,
                'entity' => $entity,
                'locale' => $this->context->language->locale,
                'controller' => $this,
                'content_only' => $content_only,
            ]
        )
```