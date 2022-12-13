---
menuTitle: action<DefinitionId>GridPresenterModifier
Title: action<DefinitionId>GridPresenterModifier
hidden: true
hookTitle: 
files:
  - src/Core/Grid/Presenter/GridPresenter.php
location:
  - front office
type: action
hookAliases:
---

# Hook action<DefinitionId>GridPresenterModifier

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/Core/Grid/Presenter/GridPresenter.php](src/Core/Grid/Presenter/GridPresenter.php)

## Call of the Hook in the origin file

```php
dispatchWithParameters('action' . Container::camelize($definition->getId()) . 'GridPresenterModifier', [
            'presented_grid' => &$presentedGrid,
        ])
```