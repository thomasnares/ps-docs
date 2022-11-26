---
title: Context
---

# Context component

The Context is a component first introduced with version 1.5 of PrestaShop. Its two goals are:

- preventing developers from using global variables.
- enabling them to change the context of some methods.

The Context is a registry for PHP variables that were previously accessed as globals. It aims to standardize the way these variables are accessed, and to make the code more robust by getting rid of global vars.

It is a light implementation of the Registry design pattern: it is a class that stores the main PrestaShop information, such as the current cookie, the customer, the employee, the cart, Smarty, etc.

Context is implemented following a [Singleton design pattern](https://refactoring.guru/design-patterns/singleton).

## What is stored by the Context?

These objects are always accessible through the context:

- **Language.** Set with the customer or employee language.
- **Country.** Default country.
- **Currency.** Set with the customer currency or the shop's default currency.
- **Shop.** Current shop.
- **Cookie.** Cookie instance.
- **Link.** Link instance.
- **Smarty.** Smarty instance.

These objects are only accessible for the customer Context:

- **Customer.** Existing customer retrieved from the cookie or default customer.
- **Cart.** Current cart.
- **Controller.** Current controller instance.

These objects are only accessible for the administrator Context:

- **Employee.** Current employee.

## How to access the Context?

From inside a `Controller` subclass or a `Module` subclass, the Context should be called with this shortcut: `$this->context`.

From anywhere else, you can get the Context instance by calling `Context::getContext()`.

## How is the Context initialized?

The context is initialized with data coming from the cookie or from the database. For example, to create the Language object, the context looks for an `id_lang` value in the cookie. If it doesn't find one, it will retrieve the default language id from the database.

The context is initialized at every request, in [config/config.inc.php](https://github.com/PrestaShop/PrestaShop/blob/8.0.x/config/config.inc.php).

First, [an empty context is created](https://github.com/PrestaShop/PrestaShop/blob/8.0.x/config/config.inc.php#L113) using `Context::getContext();`, and then it is sequencially filled with:

- [Shop](https://github.com/PrestaShop/PrestaShop/blob/8.0.x/config/config.inc.php#L117)
- [Country](https://github.com/PrestaShop/PrestaShop/blob/8.0.x/config/config.inc.php#L146-L147)
- [Session](https://github.com/PrestaShop/PrestaShop/blob/8.0.x/config/config.inc.php#L191)
- [Cookie](https://github.com/PrestaShop/PrestaShop/blob/8.0.x/config/config.inc.php#L194)
- [Employee (if in BO)](https://github.com/PrestaShop/PrestaShop/blob/8.0.x/config/config.inc.php#L198-L199)
- [Language](https://github.com/PrestaShop/PrestaShop/blob/8.0.x/config/config.inc.php#L242)
- [Smarty](https://github.com/PrestaShop/PrestaShop/blob/8.0.x/config/config.inc.php#L247)
- [Customer (if in FO)](https://github.com/PrestaShop/PrestaShop/blob/8.0.x/config/config.inc.php#L272)
- [Link](https://github.com/PrestaShop/PrestaShop/blob/8.0.x/config/config.inc.php#L277)

The Cart (and the Currency) are set in the Context when [initializing the FrontController instance in FO](https://github.com/PrestaShop/PrestaShop/blob/8.0.x/classes/controller/FrontController.php#L428-L434)