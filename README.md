# SwaggerClient-php
DGI Bénin - Tous droits réservés

This PHP package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 1.0
- Build package: io.swagger.codegen.v3.generators.php.PhpClientCodegen
For more information, please visit [https://www.impots.finances.gouv.bj](https://www.impots.finances.gouv.bj)

## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com/GIT_USER_ID/GIT_REPO_ID.git"
    }
  ],
  "require": {
    "GIT_USER_ID/GIT_REPO_ID": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/SwaggerClient-php/vendor/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\SfeInfoApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->apiInfoInvoiceTypesGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SfeInfoApi->apiInfoInvoiceTypesGet: ', $e->getMessage(), PHP_EOL;
}

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\SfeInfoApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->apiInfoPaymentTypesGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SfeInfoApi->apiInfoPaymentTypesGet: ', $e->getMessage(), PHP_EOL;
}

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\SfeInfoApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->apiInfoStatusGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SfeInfoApi->apiInfoStatusGet: ', $e->getMessage(), PHP_EOL;
}

// Configure API key authorization: Bearer
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\SfeInfoApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->apiInfoTaxGroupsGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SfeInfoApi->apiInfoTaxGroupsGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

## Documentation for API Endpoints

All URIs are relative to *https://developper.impots.bj/sygmef-emcf*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*SfeInfoApi* | [**apiInfoInvoiceTypesGet**](docs/Api/SfeInfoApi.md#apiinfoinvoicetypesget) | **GET** /api/info/invoiceTypes | 
*SfeInfoApi* | [**apiInfoPaymentTypesGet**](docs/Api/SfeInfoApi.md#apiinfopaymenttypesget) | **GET** /api/info/paymentTypes | 
*SfeInfoApi* | [**apiInfoStatusGet**](docs/Api/SfeInfoApi.md#apiinfostatusget) | **GET** /api/info/status | 
*SfeInfoApi* | [**apiInfoTaxGroupsGet**](docs/Api/SfeInfoApi.md#apiinfotaxgroupsget) | **GET** /api/info/taxGroups | 
*SfeInvoiceApi* | [**apiInvoiceGet**](docs/Api/SfeInvoiceApi.md#apiinvoiceget) | **GET** /api/invoice | 
*SfeInvoiceApi* | [**apiInvoicePost**](docs/Api/SfeInvoiceApi.md#apiinvoicepost) | **POST** /api/invoice | 
*SfeInvoiceApi* | [**apiInvoiceUidCancelPut**](docs/Api/SfeInvoiceApi.md#apiinvoiceuidcancelput) | **PUT** /api/invoice/{uid}/cancel | 
*SfeInvoiceApi* | [**apiInvoiceUidConfirmPut**](docs/Api/SfeInvoiceApi.md#apiinvoiceuidconfirmput) | **PUT** /api/invoice/{uid}/confirm | 
*SfeInvoiceApi* | [**apiInvoiceUidGet**](docs/Api/SfeInvoiceApi.md#apiinvoiceuidget) | **GET** /api/invoice/{uid} | 

## Documentation For Models

 - [AibGroupTypeEnum](docs/Model/AibGroupTypeEnum.md)
 - [ClientDto](docs/Model/ClientDto.md)
 - [EmcfInfoDto](docs/Model/EmcfInfoDto.md)
 - [InfoResponseDto](docs/Model/InfoResponseDto.md)
 - [InvoiceDetailsDto](docs/Model/InvoiceDetailsDto.md)
 - [InvoiceRequestDataDto](docs/Model/InvoiceRequestDataDto.md)
 - [InvoiceResponseDto](docs/Model/InvoiceResponseDto.md)
 - [InvoiceTypeDto](docs/Model/InvoiceTypeDto.md)
 - [InvoiceTypeEnum](docs/Model/InvoiceTypeEnum.md)
 - [ItemDto](docs/Model/ItemDto.md)
 - [OperatorDto](docs/Model/OperatorDto.md)
 - [PaymentDto](docs/Model/PaymentDto.md)
 - [PaymentTypeDto](docs/Model/PaymentTypeDto.md)
 - [PaymentTypeEnum](docs/Model/PaymentTypeEnum.md)
 - [PendingRequestDto](docs/Model/PendingRequestDto.md)
 - [SecurityElementsDto](docs/Model/SecurityElementsDto.md)
 - [StatusResponseDto](docs/Model/StatusResponseDto.md)
 - [TaxGroupTypeEnum](docs/Model/TaxGroupTypeEnum.md)
 - [TaxGroupsDto](docs/Model/TaxGroupsDto.md)

## Documentation For Authorization


## Bearer

- **Type**: API key
- **API key parameter name**: Authorization
- **Location**: HTTP header


## Author



