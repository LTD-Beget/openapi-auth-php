# OpenAPI\Client\AuthServiceApi

All URIs are relative to https://api.beget.com, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**authServiceAuth()**](AuthServiceApi.md#authServiceAuth) | **POST** /v1/auth |  |
| [**authServiceLogout()**](AuthServiceApi.md#authServiceLogout) | **POST** /v1/auth/logout |  |
| [**authServiceRefreshToken()**](AuthServiceApi.md#authServiceRefreshToken) | **POST** /v1/auth/refresh |  |
| [**authServiceSwitchUser()**](AuthServiceApi.md#authServiceSwitchUser) | **POST** /v1/auth/switch |  |


## `authServiceAuth()`

```php
authServiceAuth($auth_auth_request): \OpenAPI\Client\Model\AuthAuthResponse
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearerAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\AuthServiceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$auth_auth_request = new \OpenAPI\Client\Model\AuthAuthRequest(); // \OpenAPI\Client\Model\AuthAuthRequest

try {
    $result = $apiInstance->authServiceAuth($auth_auth_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthServiceApi->authServiceAuth: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **auth_auth_request** | [**\OpenAPI\Client\Model\AuthAuthRequest**](../Model/AuthAuthRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\AuthAuthResponse**](../Model/AuthAuthResponse.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `authServiceLogout()`

```php
authServiceLogout(): object
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearerAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\AuthServiceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->authServiceLogout();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthServiceApi->authServiceLogout: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `authServiceRefreshToken()`

```php
authServiceRefreshToken(): \OpenAPI\Client\Model\AuthRefreshTokenResponse
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearerAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\AuthServiceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->authServiceRefreshToken();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthServiceApi->authServiceRefreshToken: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\OpenAPI\Client\Model\AuthRefreshTokenResponse**](../Model/AuthRefreshTokenResponse.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `authServiceSwitchUser()`

```php
authServiceSwitchUser($auth_switch_user_request): \OpenAPI\Client\Model\AuthSwitchUserResponse
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearerAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\AuthServiceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$auth_switch_user_request = new \OpenAPI\Client\Model\AuthSwitchUserRequest(); // \OpenAPI\Client\Model\AuthSwitchUserRequest

try {
    $result = $apiInstance->authServiceSwitchUser($auth_switch_user_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthServiceApi->authServiceSwitchUser: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **auth_switch_user_request** | [**\OpenAPI\Client\Model\AuthSwitchUserRequest**](../Model/AuthSwitchUserRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\AuthSwitchUserResponse**](../Model/AuthSwitchUserResponse.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
