---
menuTitle: actionPresentModule
Title: actionPresentModule
hidden: true
hookTitle: 
files:
  - src/Adapter/Presenter/Module/ModulePresenter.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionPresentModule

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/Adapter/Presenter/Module/ModulePresenter.php](src/Adapter/Presenter/Module/ModulePresenter.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionPresentModule',
            ['presentedModule' => &$result]
        )
```