---
menuTitle: actionValidateStepComplete
Title: actionValidateStepComplete
hidden: true
hookTitle: 
files:
  - classes/checkout/CheckoutDeliveryStep.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionValidateStepComplete

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/checkout/CheckoutDeliveryStep.php](classes/checkout/CheckoutDeliveryStep.php)

## Parameters details

```php
    <?php
    array(
      'step_name' => 'delivery',
      'request_params' => $requestParams,
      'completed' => &$isComplete,
    );
```

## Call of the Hook in the origin file

```php
Hook::exec(
            'actionValidateStepComplete',
            [
                'step_name' => 'delivery',
                'request_params' => $requestParams,
                'completed' => &$isComplete,
            ],
            Module::getModuleIdByName($currentDeliveryOption['external_module_name'])
        )
```