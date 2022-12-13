---
menuTitle: actionShopDataDuplication
Title: actionShopDataDuplication
hidden: true
hookTitle: 
files:
  - classes/shop/Shop.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionShopDataDuplication

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/shop/Shop.php](classes/shop/Shop.php)

## Parameters details

```php
    <?php
    array(
      'old_id_shop' => (int) Old shop ID,
      'new_id_shop' => (int) New shop ID
    );
```

## Call of the Hook in the origin file

```php
Hook::exec('actionShopDataDuplication', [
                        'old_id_shop' => (int) $old_id,
                        'new_id_shop' => (int) $this->id,
                    ], $m['id_module'])
```