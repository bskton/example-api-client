# example-api-client
Provide a client for Example API

This PHP package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 1.0.0
- Build package: io.swagger.codegen.languages.PhpClientCodegen

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
      "url": "https://github.com/bskton/example-api-client.git"
    }
  ],
  "require": {
    "bskton/example-api-client": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/example-api-client/vendor/autoload.php');
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

$apiInstance = new Bskton\Example\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->getComments();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->getComments: ', $e->getMessage(), PHP_EOL;
}

?>
```

## Documentation for API Endpoints

All URIs are relative to *http://localhost*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*DefaultApi* | [**getComments**](docs/Api/DefaultApi.md#getcomments) | **GET** /comments | 
*DefaultApi* | [**postComment**](docs/Api/DefaultApi.md#postcomment) | **POST** /comment | 
*DefaultApi* | [**updateComment**](docs/Api/DefaultApi.md#updatecomment) | **PATCH** /comment | 


## Documentation For Models

 - [Comment](docs/Model/Comment.md)
 - [CommentPatch](docs/Model/CommentPatch.md)
 - [CommentsList](docs/Model/CommentsList.md)


## Documentation For Authorization

 All endpoints do not require authorization.


## Author




