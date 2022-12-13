---
menuTitle: action<Controller>OptionsModifier
Title: action<Controller>OptionsModifier
hidden: true
hookTitle: 
files:
  - classes/controller/AdminController.php
location:
  - back office
type: action
hookAliases:
---

# Hook action<Controller>OptionsModifier

## Information

Hook location:
  - back office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/controller/AdminController.php](classes/controller/AdminController.php)

## Call of the Hook in the origin file

```php
Hook::exec('action' . $this->controller_name . 'OptionsModifier', [
            'options' => &$this->fields_options,
            'option_vars' => &$this->tpl_option_vars,
        ])
```