---
menuTitle: displayback officeEmployeeMenu
Title: displayback officeEmployeeMenu
hidden: true
hookTitle: Administration Employee menu
files:
  - src/PrestaShopBundle/Bridge/Smarty/HeaderConfigurator.php
location:
  - front office
type: display
hookAliases:
---

# Hook displayback officeEmployeeMenu

## Information

{{% notice tip %}}
**Administration Employee menu:** 

This hook is displayed in the employee menu
{{% /notice %}}

Hook location:
  - front office

Hook type: display

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Bridge/Smarty/HeaderConfigurator.php](src/PrestaShopBundle/Bridge/Smarty/HeaderConfigurator.php)

## Parameters details

```php
    <?php
    [
        'links' => (ActionsBarButtonsCollection) $menuLinksCollections,
    ]
```

## Call of the Hook in the origin file

```php
dispatchWithParameters(
            'displayback officeEmployeeMenu',
            [
                'links' => $menuLinksCollections,
            ]
        )
```