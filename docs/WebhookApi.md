# PSOpenAPITools.PSOpenAPITools\Api.WebhookApi

All URIs are relative to *https://api.api2cart.com/v1.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Invoke-WebhookCount**](WebhookApi.md#Invoke-WebhookCount) | **GET** /webhook.count.json | webhook.count
[**Invoke-WebhookCreate**](WebhookApi.md#Invoke-WebhookCreate) | **POST** /webhook.create.json | webhook.create
[**Invoke-WebhookDelete**](WebhookApi.md#Invoke-WebhookDelete) | **DELETE** /webhook.delete.json | webhook.delete
[**Invoke-WebhookEvents**](WebhookApi.md#Invoke-WebhookEvents) | **GET** /webhook.events.json | webhook.events
[**Invoke-WebhookList**](WebhookApi.md#Invoke-WebhookList) | **GET** /webhook.list.json | webhook.list
[**Invoke-WebhookUpdate**](WebhookApi.md#Invoke-WebhookUpdate) | **PUT** /webhook.update.json | webhook.update


<a id="Invoke-WebhookCount"></a>
# **Invoke-WebhookCount**
> WebhookCount200Response Invoke-WebhookCount<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Entity] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Action] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Active] <System.Nullable[Boolean]><br>

webhook.count

Count registered webhooks on the store.

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

$Entity = "product" # String | The entity you want to filter webhooks by (e.g. order or product) (optional)
$Action = "add" # String | The action you want to filter webhooks by (e.g. order or product) (optional)
$Active = $true # Boolean | The webhook status you want to filter webhooks by (optional)

# webhook.count
try {
    $Result = Invoke-WebhookCount -Entity $Entity -Action $Action -Active $Active
} catch {
    Write-Host ("Exception occurred when calling Invoke-WebhookCount: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Entity** | **String**| The entity you want to filter webhooks by (e.g. order or product) | [optional] 
 **Action** | **String**| The action you want to filter webhooks by (e.g. order or product) | [optional] 
 **Active** | **Boolean**| The webhook status you want to filter webhooks by | [optional] 

### Return type

[**WebhookCount200Response**](WebhookCount200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-WebhookCreate"></a>
# **Invoke-WebhookCreate**
> BasketLiveShippingServiceCreate200Response Invoke-WebhookCreate<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Entity] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Action] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Callback] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Label] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Fields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Active] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

webhook.create

Create webhook on the store and subscribe to it.

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

$Entity = "product" # String | Specify the entity that you want to enable webhooks for (e.g product, order, customer, category)
$Action = "add" # String | Specify what action (event) will trigger the webhook (e.g add, delete, or update)
$Callback = "https://example.com/callback" # String | Callback url that returns shipping rates. It should be able to accept POST requests with json data. (optional)
$Label = "Super webhook" # String | The name you give to the webhook (optional)
$Fields = "id, name, description" # String | Fields the webhook should send (optional) (default to "force_all")
$ResponseFields = "{result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Active = $true # Boolean | Webhook status (optional) (default to $true)
$LangId = "3" # String | Language id (optional)
$StoreId = "1" # String | Defines store id where the webhook should be assigned (optional)

# webhook.create
try {
    $Result = Invoke-WebhookCreate -Entity $Entity -Action $Action -Callback $Callback -Label $Label -Fields $Fields -ResponseFields $ResponseFields -Active $Active -LangId $LangId -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-WebhookCreate: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Entity** | **String**| Specify the entity that you want to enable webhooks for (e.g product, order, customer, category) | 
 **Action** | **String**| Specify what action (event) will trigger the webhook (e.g add, delete, or update) | 
 **Callback** | **String**| Callback url that returns shipping rates. It should be able to accept POST requests with json data. | [optional] 
 **Label** | **String**| The name you give to the webhook | [optional] 
 **Fields** | **String**| Fields the webhook should send | [optional] [default to &quot;force_all&quot;]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Active** | **Boolean**| Webhook status | [optional] [default to $true]
 **LangId** | **String**| Language id | [optional] 
 **StoreId** | **String**| Defines store id where the webhook should be assigned | [optional] 

### Return type

[**BasketLiveShippingServiceCreate200Response**](BasketLiveShippingServiceCreate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-WebhookDelete"></a>
# **Invoke-WebhookDelete**
> AttributeDelete200Response Invoke-WebhookDelete<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>

webhook.delete

Delete registered webhook on the store.

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

$Id = "25" # String | Webhook id

# webhook.delete
try {
    $Result = Invoke-WebhookDelete -Id $Id
} catch {
    Write-Host ("Exception occurred when calling Invoke-WebhookDelete: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Webhook id | 

### Return type

[**AttributeDelete200Response**](AttributeDelete200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-WebhookEvents"></a>
# **Invoke-WebhookEvents**
> WebhookEvents200Response Invoke-WebhookEvents<br>

webhook.events

List all Webhooks that are available on this store.

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


# webhook.events
try {
    $Result = Invoke-WebhookEvents
} catch {
    Write-Host ("Exception occurred when calling Invoke-WebhookEvents: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**WebhookEvents200Response**](WebhookEvents200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-WebhookList"></a>
# **Invoke-WebhookList**
> WebhookList200Response Invoke-WebhookList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Entity] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Action] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Active] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Ids] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>

webhook.list

List registered webhook on the store.

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
$Entity = "product" # String | The entity you want to filter webhooks by (e.g. order or product) (optional)
$Action = "add" # String | The action you want to filter webhooks by (e.g. add, update, or delete) (optional)
$Active = $true # Boolean | The webhook status you want to filter webhooks by (optional)
$Ids = "3,14,25" # String | List of сomma-separated webhook ids (optional)
$Params = "id,entity,callback,fields" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,entity,action,callback")

# webhook.list
try {
    $Result = Invoke-WebhookList -Start $Start -Count $Count -Entity $Entity -Action $Action -Active $Active -Ids $Ids -Params $Params
} catch {
    Write-Host ("Exception occurred when calling Invoke-WebhookList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **Entity** | **String**| The entity you want to filter webhooks by (e.g. order or product) | [optional] 
 **Action** | **String**| The action you want to filter webhooks by (e.g. add, update, or delete) | [optional] 
 **Active** | **Boolean**| The webhook status you want to filter webhooks by | [optional] 
 **Ids** | **String**| List of сomma-separated webhook ids | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,entity,action,callback&quot;]

### Return type

[**WebhookList200Response**](WebhookList200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-WebhookUpdate"></a>
# **Invoke-WebhookUpdate**
> ProductImageUpdate200Response Invoke-WebhookUpdate<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Callback] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Label] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Fields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Active] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>

webhook.update

Update Webhooks parameters.

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

$Id = "25" # String | Webhook id
$Callback = "https://example.com/callback" # String | Callback url that returns shipping rates. It should be able to accept POST requests with json data. (optional)
$Label = "Super webhook" # String | The name you give to the webhook (optional)
$Fields = "id, name, description" # String | Fields the webhook should send (optional)
$ResponseFields = "{result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Active = $true # Boolean | Webhook status (optional)
$LangId = "3" # String | Language id (optional)

# webhook.update
try {
    $Result = Invoke-WebhookUpdate -Id $Id -Callback $Callback -Label $Label -Fields $Fields -ResponseFields $ResponseFields -Active $Active -LangId $LangId
} catch {
    Write-Host ("Exception occurred when calling Invoke-WebhookUpdate: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Webhook id | 
 **Callback** | **String**| Callback url that returns shipping rates. It should be able to accept POST requests with json data. | [optional] 
 **Label** | **String**| The name you give to the webhook | [optional] 
 **Fields** | **String**| Fields the webhook should send | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Active** | **Boolean**| Webhook status | [optional] 
 **LangId** | **String**| Language id | [optional] 

### Return type

[**ProductImageUpdate200Response**](ProductImageUpdate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

