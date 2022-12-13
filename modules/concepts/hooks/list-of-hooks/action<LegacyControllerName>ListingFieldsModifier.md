---
menuTitle: action<LegacyControllerName>ListingFieldsModifier
Title: action<LegacyControllerName>ListingFieldsModifier
hidden: true
hookTitle: 
files:
  - src/PrestaShopBundle/Bridge/Helper/Listing/HelperBridge/HelperListBridge.php
location:
  - front office
type: action
hookAliases:
---

# Hook action<LegacyControllerName>ListingFieldsModifier

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/PrestaShopBundle/Bridge/Helper/Listing/HelperBridge/HelperListBridge.php](src/PrestaShopBundle/Bridge/Helper/Listing/HelperBridge/HelperListBridge.php)

## Call of the Hook in the origin file

```php
dispatchWithParameters('action' . $helperListConfiguration->legacyControllerName . 'ListingFieldsModifier', [
            'select' => &$helperListConfiguration->select,
            'join' => &$helperListConfiguration->join,
            'where' => &$helperListConfiguration->where,
            'group_by' => &$helperListConfiguration->group,
            'order_by' => &$helperListConfiguration->orderBy,
            'order_way' => &$helperListConfiguration->orderWay,
            'fields' => &$helperListConfiguration->fieldsList,
        ])
```