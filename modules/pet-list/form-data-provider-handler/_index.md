# FormDataProvider and FormDataHandler

In order to be able to do CRUD for our entity (--- insert link to CRUD definition ---), we need four main elements, as explained here : 1.7/development/architecture/migration-guide/forms/crud-forms/

- Form Builder (creates a form)
- Form Handler (handle this form's submission)
- Form Data Provider (provides data to prefill the form)
- Form Data Handler (saves data to database)

For our use-case, we only need to create a FormDataProvider and a FormDataHandler. The default Form Builder and Form Handler implemented by Prestashop are enough. 

## FormDataProvider

In `src`, create a subdirectory named `Form`, and create a `CustomerPetListFormDataProvider.php` file :

```php
<?php

namespace Preston\CustomerPetList\Form;

use PrestaShop\PrestaShop\Core\Form\IdentifiableObject\DataProvider\FormDataProviderInterface;
use Preston\CustomerPetList\Entity\Pet;
use PrestaShopObjectNotFoundException;

/**
 * Class CustomerPetListFormDataProvider.
 */
class CustomerPetListFormDataProvider implements FormDataProviderInterface
{
    /**
     * Get form data for given object with given id.
     *
     * @param int $id
     *
     * @return mixed
     */
    public function getData($petId)
    {
        $petObjectModel = new Pet($petId);
        
        // check that the element exists in db
        if (empty($petObjectModel->id)) {
            throw new PrestaShopObjectNotFoundException('Object not found');
        }

        return [
            'name' => $petObjectModel->name,
            'breed' => $petObjectModel->breed
        ];
    }

    /**
     * Get default form data.
     *
     * @return mixed
     */
    public function getDefaultData()
    {
        return [
            'name' => '',
            'breed' => ''
        ];
    }
}
```

## FormDataHandler

In `src/Form`, create a `CustomerPetListFormDataHandler.php` file :

```php
<?php

namespace Preston\CustomerPetList\Form;

use PrestaShop\PrestaShop\Core\Form\IdentifiableObject\DataHandler\FormDataHandlerInterface;
use Preston\CustomerPetList\Entity\Pet;

final class PetFormDataHandler implements FormDataHandlerInterface
{
    /**
     * Create object from form data.
     *
     * @param array $data
     *
     * @return mixed
     */
    public function create(array $data)
    {
        $petObjectModel = new Pet();
    
        $petObjectModel->save();

        return $petObjectModel->id;
    }

    /**
     * Update object with form data.
     *
     * @param int $id
     * @param array $data
     */
    public function update($id, array $data)
    {
        $petObjectModel = new Pet($id);
    
        $petObjectModel->update();
    }
}
```

