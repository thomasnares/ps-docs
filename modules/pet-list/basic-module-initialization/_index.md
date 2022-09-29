# Basic module initialization

## The Module class

In the modules directory, create a folder named : `customerpetlist`

Create a file named like the directory, `customerpetlist.php`

Set the file with this content, as explained here : /1.7/modules/creation/tutorial/

```php
<?php

if (!defined('_PS_VERSION_')) {
    exit;
}

class CustomerPetList extends Module
{

    public function __construct()
    {
        $this->name = 'customerpetlist';
        $this->tab = 'front_office_features';
        $this->version = '1.0.0';
        $this->author = 'John DOE';
        $this->need_instance = 0;
        $this->ps_versions_compliancy = [
            'min' => '1.6.0',
            'max' => '8.1.0',
        ];
        $this->bootstrap = true;

        parent::__construct();

        $this->displayName = $this->l('Customer Pet List');
        $this->description = $this->l('This module allows you to store the Pet list of a Customer');

        $this->confirmUninstall = $this->l('Are you sure you want to uninstall and delete all pets from database ?');
    }

    public function install()
    {
        if (Shop::isFeatureActive()) {
            Shop::setContext(Shop::CONTEXT_ALL);
        }

        return (
            parent::install()
        ); 
    }
    
    public function uninstall()
    {
        return (
            parent::uninstall()
        );
    }

}
```

## The database tables

Create a `install.sql` with the sql query to create the table :

```sql
CREATE TABLE IF NOT EXISTS `custom_pet` (
  `id_pet` int(10) unsigned NOT NULL auto_increment,
  `id_customer` int(10) unsigned NOT NULL,
  `name` varchar(128) NULL,
  `breed` varchar(64) NULL,
  PRIMARY KEY (`id_pet`),
  KEY `id_customer` (`id_customer`),
) ENGINE=ENGINE_TYPE  DEFAULT CHARSET=utf8;
```

Please add a `IF NOT EXISTS` statement when creating a table to avoid any installation issue

Create the `uninstall.sql` file with the query to delete the table :

```sql
DROP TABLE IF EXISTS `custom_pet`;
```

Then, execute the queries of those files in the `install` and `uninstall`  methods of your module :

```php
public function install()
{
    if (Shop::isFeatureActive()) {
        Shop::setContext(Shop::CONTEXT_ALL);
    }

    if (!file_exists(dirname(__FILE__) . '/' . self::INSTALL_SQL_FILE)) {
        return false;
    } elseif (!$sql = file_get_contents(dirname(__FILE__) . '/' . self::INSTALL_SQL_FILE)) {
        return false;
    }
    
    $sql = preg_split("/;\s*[\r\n]+/", trim($sql));
    foreach ($sql as $query) {
        if (!Db::getInstance()->execute(trim($query))) {
            return false;
        }
    }
    
    return (
        parent::install() 
    ); 
}

public function uninstall()
{
    if (!file_exists(dirname(__FILE__) . '/' . self::UNINSTALL_SQL_FILE)) {
        return false;
    } elseif (!$sql = file_get_contents(dirname(__FILE__) . '/' . self::UNINSTALL_SQL_FILE)) {
        return false;
    }
    
    $sql = preg_split("/;\s*[\r\n]+/", trim($sql));
    foreach ($sql as $query) {
        if (!Db::getInstance()->execute(trim($query))) {
            return false;
        }
    }

    return (
        parent::uninstall()
    );
}
```

## Install the module

At this point, you can install / uninstall your module, with the method of your choice : backoffice or symfony's console. 

To install the module with symfony's console : 

```php
php bin/console prestashop:module install customerpetlist
```

Confirm that the module is successfully installed by checking if the database table is created using your favorite GUI (phpMyAdmin, adminer, ...) or your Mysql CLI.

## Setup Composer and define your namespace

Create a `composer.json` file in your module directory, and define a namespace :

```json
{
    "name": "preston/customerpetlist",
    "description": "Manage pet list for your customers",
    "authors": [
        {
            "name": "Preston",
            "email": "preston@domain.com"
        }
    ],
    "require": {
        "php": ">=7.3.0"
    },
    "autoload": {
        "psr-4": {
            "Preston\\CustomerPetList\\": "src/"
        },
        "classmap": [
            "<file>.php",
            "classes/"
        ],
        "exclude-from-classmap": []
    },
    "config": {
        "preferred-install": "dist",
        "prepend-autoloader": false
    },
    "type": "prestashop-module",
    "author": "Preston",
    "license": ""
}
```

Then run : `composer dump-autoload` in your module root. (1.7/modules/concepts/composer/#generate-the-autoloader)

