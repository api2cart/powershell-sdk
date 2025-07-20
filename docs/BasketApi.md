# PSOpenAPITools.PSOpenAPITools\Api.BasketApi

All URIs are relative to *https://api.api2cart.local.com/v1.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Invoke-BasketInfo**](BasketApi.md#Invoke-BasketInfo) | **GET** /basket.info.json | basket.info
[**Invoke-BasketItemAdd**](BasketApi.md#Invoke-BasketItemAdd) | **POST** /basket.item.add.json | basket.item.add
[**Invoke-BasketLiveShippingServiceCreate**](BasketApi.md#Invoke-BasketLiveShippingServiceCreate) | **POST** /basket.live_shipping_service.create.json | basket.live_shipping_service.create
[**Invoke-BasketLiveShippingServiceDelete**](BasketApi.md#Invoke-BasketLiveShippingServiceDelete) | **DELETE** /basket.live_shipping_service.delete.json | basket.live_shipping_service.delete
[**Invoke-BasketLiveShippingServiceList**](BasketApi.md#Invoke-BasketLiveShippingServiceList) | **GET** /basket.live_shipping_service.list.json | basket.live_shipping_service.list


<a id="Invoke-BasketInfo"></a>
# **Invoke-BasketInfo**
> BasketInfo200Response Invoke-BasketInfo<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

basket.info

Retrieve basket information.

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

$Id = "10" # String | Entity id
$StoreId = "1" # String | Store Id (optional)
$ResponseFields = "{result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "force_all")
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# basket.info
try {
    $Result = Invoke-BasketInfo -Id $Id -StoreId $StoreId -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-BasketInfo: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Entity id | 
 **StoreId** | **String**| Store Id | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;force_all&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**BasketInfo200Response**](BasketInfo200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-BasketItemAdd"></a>
# **Invoke-BasketItemAdd**
> BasketItemAdd200Response Invoke-BasketItemAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ProductId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-VariantId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Quantity] <System.Nullable[Decimal]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

basket.item.add

Add item to basket

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

$CustomerId = "5" # String | Retrieves orders specified by customer id
$ProductId = "10" # String | Defines id of the product which should be added to the basket
$VariantId = "45" # String | Defines product's variants specified by variant id (optional)
$Quantity = 6 # Decimal | Defines new items quantity (optional) (default to 0)
$StoreId = "1" # String | Store Id (optional)

# basket.item.add
try {
    $Result = Invoke-BasketItemAdd -CustomerId $CustomerId -ProductId $ProductId -VariantId $VariantId -Quantity $Quantity -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-BasketItemAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **CustomerId** | **String**| Retrieves orders specified by customer id | 
 **ProductId** | **String**| Defines id of the product which should be added to the basket | 
 **VariantId** | **String**| Defines product&#39;s variants specified by variant id | [optional] 
 **Quantity** | **Decimal**| Defines new items quantity | [optional] [default to 0]
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**BasketItemAdd200Response**](BasketItemAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-BasketLiveShippingServiceCreate"></a>
# **Invoke-BasketLiveShippingServiceCreate**
> BasketLiveShippingServiceCreate200Response Invoke-BasketLiveShippingServiceCreate<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Name] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Callback] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

basket.live_shipping_service.create

Create live shipping rate service.

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

$Name = "BestDelivery" # String | Shipping Service Name
$Callback = "https://example.com/callback" # String | Callback url that returns shipping rates. It should be able to accept POST requests with json data.
$StoreId = "1" # String | Store Id (optional)

# basket.live_shipping_service.create
try {
    $Result = Invoke-BasketLiveShippingServiceCreate -Name $Name -Callback $Callback -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-BasketLiveShippingServiceCreate: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Name** | **String**| Shipping Service Name | 
 **Callback** | **String**| Callback url that returns shipping rates. It should be able to accept POST requests with json data. | 
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**BasketLiveShippingServiceCreate200Response**](BasketLiveShippingServiceCreate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-BasketLiveShippingServiceDelete"></a>
# **Invoke-BasketLiveShippingServiceDelete**
> BasketLiveShippingServiceDelete200Response Invoke-BasketLiveShippingServiceDelete<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <Int32><br>

basket.live_shipping_service.delete

Delete live shipping rate service.

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

$Id = 5 # Int32 | Entity id

# basket.live_shipping_service.delete
try {
    $Result = Invoke-BasketLiveShippingServiceDelete -Id $Id
} catch {
    Write-Host ("Exception occurred when calling Invoke-BasketLiveShippingServiceDelete: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **Int32**| Entity id | 

### Return type

[**BasketLiveShippingServiceDelete200Response**](BasketLiveShippingServiceDelete200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-BasketLiveShippingServiceList"></a>
# **Invoke-BasketLiveShippingServiceList**
> BasketLiveShippingServiceList200Response Invoke-BasketLiveShippingServiceList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

basket.live_shipping_service.list

Retrieve a list of live shipping rate services.

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

$Start = 0 # Int32 | This parameter sets the number from which you want to get entities (optional) (default to 0)
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$StoreId = "1" # String | Store Id (optional)

# basket.live_shipping_service.list
try {
    $Result = Invoke-BasketLiveShippingServiceList -Start $Start -Count $Count -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-BasketLiveShippingServiceList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**BasketLiveShippingServiceList200Response**](BasketLiveShippingServiceList200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

