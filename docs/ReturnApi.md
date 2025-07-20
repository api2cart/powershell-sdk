# PSOpenAPITools.PSOpenAPITools\Api.ReturnApi

All URIs are relative to *https://api.api2cart.local.com/v1.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Invoke-ReturnActionList**](ReturnApi.md#Invoke-ReturnActionList) | **GET** /return.action.list.json | return.action.list
[**Invoke-ReturnCount**](ReturnApi.md#Invoke-ReturnCount) | **GET** /return.count.json | return.count
[**Invoke-ReturnInfo**](ReturnApi.md#Invoke-ReturnInfo) | **GET** /return.info.json | return.info
[**Invoke-ReturnList**](ReturnApi.md#Invoke-ReturnList) | **GET** /return.list.json | return.list
[**Invoke-ReturnReasonList**](ReturnApi.md#Invoke-ReturnReasonList) | **GET** /return.reason.list.json | return.reason.list
[**Invoke-ReturnStatusList**](ReturnApi.md#Invoke-ReturnStatusList) | **GET** /return.status.list.json | return.status.list


<a id="Invoke-ReturnActionList"></a>
# **Invoke-ReturnActionList**
> ReturnActionList200Response Invoke-ReturnActionList<br>

return.action.list

Retrieve list of return actions

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


# return.action.list
try {
    $Result = Invoke-ReturnActionList
} catch {
    Write-Host ("Exception occurred when calling Invoke-ReturnActionList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ReturnActionList200Response**](ReturnActionList200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-ReturnCount"></a>
# **Invoke-ReturnCount**
> ReturnCount200Response Invoke-ReturnCount<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderIds] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Status] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ReturnType] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ReportRequestId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DisableReportCache] <System.Nullable[Boolean]><br>

return.count

Count returns in store

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

$OrderIds = "24,25" # String | Counts return requests specified by order ids (optional)
$CustomerId = "5" # String | Counts return requests quantity specified by customer id (optional)
$StoreId = "1" # String | Store Id (optional)
$Status = "disabled" # String | Defines status (optional)
$ReturnType = "FBA" # String | Retrieves returns specified by return type (optional)
$CreatedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their creation date (optional)
$CreatedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their creation date (optional)
$ModifiedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their modification date (optional)
$ModifiedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their modification date (optional)
$ReportRequestId = "105245017661" # String | Report request id (optional)
$DisableReportCache = $false # Boolean | Disable report cache for current request (optional) (default to $false)

# return.count
try {
    $Result = Invoke-ReturnCount -OrderIds $OrderIds -CustomerId $CustomerId -StoreId $StoreId -Status $Status -ReturnType $ReturnType -CreatedFrom $CreatedFrom -CreatedTo $CreatedTo -ModifiedFrom $ModifiedFrom -ModifiedTo $ModifiedTo -ReportRequestId $ReportRequestId -DisableReportCache $DisableReportCache
} catch {
    Write-Host ("Exception occurred when calling Invoke-ReturnCount: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **OrderIds** | **String**| Counts return requests specified by order ids | [optional] 
 **CustomerId** | **String**| Counts return requests quantity specified by customer id | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **Status** | **String**| Defines status | [optional] 
 **ReturnType** | **String**| Retrieves returns specified by return type | [optional] 
 **CreatedFrom** | **String**| Retrieve entities from their creation date | [optional] 
 **CreatedTo** | **String**| Retrieve entities to their creation date | [optional] 
 **ModifiedFrom** | **String**| Retrieve entities from their modification date | [optional] 
 **ModifiedTo** | **String**| Retrieve entities to their modification date | [optional] 
 **ReportRequestId** | **String**| Report request id | [optional] 
 **DisableReportCache** | **Boolean**| Disable report cache for current request | [optional] [default to $false]

### Return type

[**ReturnCount200Response**](ReturnCount200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-ReturnInfo"></a>
# **Invoke-ReturnInfo**
> ReturnInfo200Response Invoke-ReturnInfo<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

return.info

Retrieve return information.

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
$OrderId = "25" # String | Defines the order id (optional)
$StoreId = "1" # String | Store Id (optional)
$ResponseFields = "{return_code,return_message,result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,order_products" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,order_products")
$Exclude = "id,order_id" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# return.info
try {
    $Result = Invoke-ReturnInfo -Id $Id -OrderId $OrderId -StoreId $StoreId -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-ReturnInfo: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Entity id | 
 **OrderId** | **String**| Defines the order id | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,order_products&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ReturnInfo200Response**](ReturnInfo200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-ReturnList"></a>
# **Invoke-ReturnList**
> ModelResponseReturnList Invoke-ReturnList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderIds] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Status] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ReturnType] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ReportRequestId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DisableReportCache] <System.Nullable[Boolean]><br>

return.list

Get list of return requests from store.

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
$PageCursor = "MyPageCursor" # String | Used to retrieve entities via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$OrderId = "25" # String | Defines the order id (optional)
$OrderIds = "24,25" # String | Retrieves return requests specified by order ids (optional)
$CustomerId = "5" # String | Retrieves return requests specified by customer id (optional)
$StoreId = "1" # String | Store Id (optional)
$Status = "disabled" # String | Defines status (optional)
$ReturnType = "FBA" # String | Retrieves returns specified by return type (optional)
$CreatedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their creation date (optional)
$CreatedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their creation date (optional)
$ModifiedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their modification date (optional)
$ModifiedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their modification date (optional)
$ResponseFields = "{return_code,return_message,pagination,result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,order_products" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,order_products")
$Exclude = "id,order_id" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)
$ReportRequestId = "105245017661" # String | Report request id (optional)
$DisableReportCache = $false # Boolean | Disable report cache for current request (optional) (default to $false)

# return.list
try {
    $Result = Invoke-ReturnList -Start $Start -Count $Count -PageCursor $PageCursor -OrderId $OrderId -OrderIds $OrderIds -CustomerId $CustomerId -StoreId $StoreId -Status $Status -ReturnType $ReturnType -CreatedFrom $CreatedFrom -CreatedTo $CreatedTo -ModifiedFrom $ModifiedFrom -ModifiedTo $ModifiedTo -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude -ReportRequestId $ReportRequestId -DisableReportCache $DisableReportCache
} catch {
    Write-Host ("Exception occurred when calling Invoke-ReturnList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **OrderId** | **String**| Defines the order id | [optional] 
 **OrderIds** | **String**| Retrieves return requests specified by order ids | [optional] 
 **CustomerId** | **String**| Retrieves return requests specified by customer id | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **Status** | **String**| Defines status | [optional] 
 **ReturnType** | **String**| Retrieves returns specified by return type | [optional] 
 **CreatedFrom** | **String**| Retrieve entities from their creation date | [optional] 
 **CreatedTo** | **String**| Retrieve entities to their creation date | [optional] 
 **ModifiedFrom** | **String**| Retrieve entities from their modification date | [optional] 
 **ModifiedTo** | **String**| Retrieve entities to their modification date | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,order_products&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 
 **ReportRequestId** | **String**| Report request id | [optional] 
 **DisableReportCache** | **Boolean**| Disable report cache for current request | [optional] [default to $false]

### Return type

[**ModelResponseReturnList**](ModelResponseReturnList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-ReturnReasonList"></a>
# **Invoke-ReturnReasonList**
> ReturnReasonList200Response Invoke-ReturnReasonList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

return.reason.list

Retrieve list of return reasons

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

$StoreId = "1" # String | Store Id (optional)

# return.reason.list
try {
    $Result = Invoke-ReturnReasonList -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-ReturnReasonList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**ReturnReasonList200Response**](ReturnReasonList200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-ReturnStatusList"></a>
# **Invoke-ReturnStatusList**
> ReturnStatusList200Response Invoke-ReturnStatusList<br>

return.status.list

Retrieve list of statuses

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


# return.status.list
try {
    $Result = Invoke-ReturnStatusList
} catch {
    Write-Host ("Exception occurred when calling Invoke-ReturnStatusList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ReturnStatusList200Response**](ReturnStatusList200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

