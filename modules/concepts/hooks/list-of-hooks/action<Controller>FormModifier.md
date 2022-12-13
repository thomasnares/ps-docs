---
menuTitle: action<Controller>FormModifier
Title: action<Controller>FormModifier
hidden: true
hookTitle: 
files:
  - classes/controller/AdminController.php
location:
  - back office
type: action
hookAliases:
---

# Hook action&lt;Controller>FormModifier

## Information

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/controller/AdminController.php](classes/controller/AdminController.php)

## Call of the Hook in the origin file

```php
Hook::exec('action' . $this->controller_name . 'FormModifier', [
                'object' => &$this->object,
                'fields' => &$this->fields_form,
                'fields_value' => &$fields_value,
                'form_vars' => &$this->tpl_form_vars,
            ])
```