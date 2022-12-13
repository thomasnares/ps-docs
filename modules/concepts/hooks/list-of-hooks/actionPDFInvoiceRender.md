---
menuTitle: actionPDFInvoiceRender
Title: actionPDFInvoiceRender
hidden: true
hookTitle: 
files:
  - src/Adapter/PDF/OrderInvoicePdfGenerator.php
location:
  - front office
type: action
hookAliases:
---

# Hook actionPDFInvoiceRender

## Information

Hook location:
  - front office

Hook type: action

Located in: 
  - [https://github.com/PrestaShop/PrestaShop/blob/8.0.x/src/Adapter/PDF/OrderInvoicePdfGenerator.php](src/Adapter/PDF/OrderInvoicePdfGenerator.php)

## Call of the Hook in the origin file

```php
Hook::exec('actionPDFInvoiceRender', ['order_invoice_list' => $order_invoice_list])
```