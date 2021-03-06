# Bskton\Example\DefaultApi

All URIs are relative to *http://example.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getComments**](DefaultApi.md#getComments) | **GET** /comments | 
[**postComment**](DefaultApi.md#postComment) | **POST** /comment | 
[**updateComment**](DefaultApi.md#updateComment) | **PATCH** /comment/{id} | 


# **getComments**
> \Bskton\Example\Api\Model\Comment[] getComments()



### Example
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

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Bskton\Example\Api\Model\Comment[]**](../Model/Comment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postComment**
> \Bskton\Example\Api\Model\Comment postComment($body)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Bskton\Example\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Bskton\Example\Api\Model\Comment(); // \Bskton\Example\Api\Model\Comment | 

try {
    $result = $apiInstance->postComment($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->postComment: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Bskton\Example\Api\Model\Comment**](../Model/Comment.md)|  | [optional]

### Return type

[**\Bskton\Example\Api\Model\Comment**](../Model/Comment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateComment**
> \Bskton\Example\Api\Model\Comment updateComment($id, $body)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Bskton\Example\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = 56; // int | Comment identifier
$body = new \Bskton\Example\Api\Model\Comment(); // \Bskton\Example\Api\Model\Comment | 

try {
    $result = $apiInstance->updateComment($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->updateComment: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Comment identifier |
 **body** | [**\Bskton\Example\Api\Model\Comment**](../Model/Comment.md)|  | [optional]

### Return type

[**\Bskton\Example\Api\Model\Comment**](../Model/Comment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

