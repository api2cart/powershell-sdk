# PSOpenAPITools.PSOpenAPITools\Api.BridgeApi

All URIs are relative to *https://api.api2cart.local.com/v1.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Invoke-BridgeDelete**](BridgeApi.md#Invoke-BridgeDelete) | **POST** /bridge.delete.json | bridge.delete
[**Invoke-BridgeDownload**](BridgeApi.md#Invoke-BridgeDownload) | **GET** /bridge.download.file | bridge.download
[**Invoke-BridgeUpdate**](BridgeApi.md#Invoke-BridgeUpdate) | **POST** /bridge.update.json | bridge.update


<a id="Invoke-BridgeDelete"></a>
# **Invoke-BridgeDelete**
> AttributeValueDelete200Response Invoke-BridgeDelete<br>

bridge.delete

Delete bridge from the store.

### Example
```powershell
# general setting of the PowerShell module, e.g. base URL, authentication, etc
$Configuration = Get-Configuration
# Configure API key authorization: StoreKeyAuth
$Configuration.ApiKey.x-store-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-store-key = "Bearer"

# Configure API key authorization: ApiKeyAuth
$Configuration.ApiKey.x-api-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-api-key = "Bearer"


# bridge.delete
try {
    $Result = Invoke-BridgeDelete
} catch {
    Write-Host ("Exception occurred when calling Invoke-BridgeDelete: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AttributeValueDelete200Response**](AttributeValueDelete200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-BridgeDownload"></a>
# **Invoke-BridgeDownload**
> System.IO.FileInfo Invoke-BridgeDownload<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Whitelabel] <System.Nullable[Boolean]><br>

bridge.download

Download bridge for store.</br>Please note that the method would not work if you call it from Swagger UI.

### Example
```powershell
# general setting of the PowerShell module, e.g. base URL, authentication, etc
$Configuration = Get-Configuration
# Configure API key authorization: StoreKeyAuth
$Configuration.ApiKey.x-store-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-store-key = "Bearer"

# Configure API key authorization: ApiKeyAuth
$Configuration.ApiKey.x-api-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-api-key = "Bearer"

$Whitelabel = $true # Boolean | Identifies if there is a necessity to download whitelabel bridge. (optional) (default to $false)

# bridge.download
try {
    $Result = Invoke-BridgeDownload -Whitelabel $Whitelabel
} catch {
    Write-Host ("Exception occurred when calling Invoke-BridgeDownload: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Whitelabel** | **Boolean**| Identifies if there is a necessity to download whitelabel bridge. | [optional] [default to $false]

### Return type

**System.IO.FileInfo**

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/zip

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-BridgeUpdate"></a>
# **Invoke-BridgeUpdate**
> AttributeUpdate200Response Invoke-BridgeUpdate<br>

bridge.update

Update bridge in the store.

### Example
```powershell
# general setting of the PowerShell module, e.g. base URL, authentication, etc
$Configuration = Get-Configuration
# Configure API key authorization: StoreKeyAuth
$Configuration.ApiKey.x-store-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-store-key = "Bearer"

# Configure API key authorization: ApiKeyAuth
$Configuration.ApiKey.x-api-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-api-key = "Bearer"


# bridge.update
try {
    $Result = Invoke-BridgeUpdate
} catch {
    Write-Host ("Exception occurred when calling Invoke-BridgeUpdate: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AttributeUpdate200Response**](AttributeUpdate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

