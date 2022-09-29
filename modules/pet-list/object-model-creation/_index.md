# The Object Model

Object Model is ---- 1.7/development/components/database/objectmodel/

For our use-case, we need an entity representing a Pet (an animal), which belongs to a Customer.

For this, we will create a class, extending ObjectModel, and we will declare all its attributes. 

To do so, create a file named `Pet.php` in the directory of your module, with the following content :

```php
<?php

if (!defined('_PS_VERSION_')) {
    exit;
}

class Pet extends ObjectModel
{

}
```

Then, we need to define the model, add this to the body of the class :

```php
public static $definition = [
    'table' => 'customerpetlist_pet',
    'primary' => 'id_pet',
    'multilang' => false,
    'fields' => array(
        'id_customer'  => ['type' => self::TYPE_INT, 'validate' => 'isUnsignedInt'],
        'name'     => [
            'type' => self::TYPE_STRING,
            'validate' => 'isString',
            'required' => true,
            'size' => 128
        ],
        'breed'          => [
            'type' => self::TYPE_STRING,
            'validate' => 'isString',
            'size' => 64
        ],
    )
];
```

This definition is the exact reflection of the database table previously created.

