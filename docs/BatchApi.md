# PSOpenAPITools.PSOpenAPITools\Api.BatchApi

All URIs are relative to *https://api.api2cart.com/v1.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Invoke-BatchJobList**](BatchApi.md#Invoke-BatchJobList) | **GET** /batch.job.list.json | batch.job.list
[**Invoke-BatchJobResult**](BatchApi.md#Invoke-BatchJobResult) | **GET** /batch.job.result.json | batch.job.result


<a id="Invoke-BatchJobList"></a>
# **Invoke-BatchJobList**
> ModelResponseBatchJobList Invoke-BatchJobList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Ids] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ProcessedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ProcessedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>

batch.job.list

Get list of recent jobs

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

$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$PageCursor = "MyPageCursor" # String | Used to retrieve entities via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$Ids = "24,25" # String | Filter batch jobs by ids (optional)
$CreatedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their creation date (optional)
$CreatedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their creation date (optional)
$ProcessedFrom = "2100-08-29 13:45:52" # String | Retrieve entities according to their processing datetime (optional)
$ProcessedTo = "2100-08-29 13:45:52" # String | Retrieve entities according to their processing datetime (optional)
$ResponseFields = "{result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "{return_code,return_message,pagination,result}")

# batch.job.list
try {
    $Result = Invoke-BatchJobList -Count $Count -PageCursor $PageCursor -Ids $Ids -CreatedFrom $CreatedFrom -CreatedTo $CreatedTo -ProcessedFrom $ProcessedFrom -ProcessedTo $ProcessedTo -ResponseFields $ResponseFields
} catch {
    Write-Host ("Exception occurred when calling Invoke-BatchJobList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **Ids** | **String**| Filter batch jobs by ids | [optional] 
 **CreatedFrom** | **String**| Retrieve entities from their creation date | [optional] 
 **CreatedTo** | **String**| Retrieve entities to their creation date | [optional] 
 **ProcessedFrom** | **String**| Retrieve entities according to their processing datetime | [optional] 
 **ProcessedTo** | **String**| Retrieve entities according to their processing datetime | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;{return_code,return_message,pagination,result}&quot;]

### Return type

[**ModelResponseBatchJobList**](ModelResponseBatchJobList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-BatchJobResult"></a>
# **Invoke-BatchJobResult**
> ResponseBatchJobResult Invoke-BatchJobResult<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>

batch.job.result

Get job result data

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

# batch.job.result
try {
    $Result = Invoke-BatchJobResult -Id $Id
} catch {
    Write-Host ("Exception occurred when calling Invoke-BatchJobResult: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Entity id | 

### Return type

[**ResponseBatchJobResult**](ResponseBatchJobResult.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

