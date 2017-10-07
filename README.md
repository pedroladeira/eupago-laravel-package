# eupago-laravel-package
This package helps to generate references to service "eupago.pt"

```php
$eupago = Eupago::getInstance();
//required fields
$eupago->setApiKey('demo-5b72-04a6-7847-5f6');
$eupago->setTransactionId('orderid');

// generate reference passing value
$result = $eupago->generateReferenceMB(123.43);

// get information about reference
$result = $eupago->referenceInformation($result->referencia);
```
