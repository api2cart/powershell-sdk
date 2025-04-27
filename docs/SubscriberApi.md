# PSOpenAPITools.PSOpenAPITools\Api.SubscriberApi

All URIs are relative to *https://api.api2cart.com/v1.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Invoke-SubscriberList**](SubscriberApi.md#Invoke-SubscriberList) | **GET** /subscriber.list.json | subscriber.list


<a id="Invoke-SubscriberList"></a>
# **Invoke-SubscriberList**
> ModelResponseSubscriberList Invoke-SubscriberList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Subscribed] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Email] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

subscriber.list

Get subscribers list

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
$Subscribed = $false # Boolean | Filter by subscription status (optional)
$StoreId = "1" # String | Store Id (optional)
$Email = "mail@example.com" # String | Filter subscribers by email (optional)
$CreatedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their creation date (optional)
$CreatedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their creation date (optional)
$ModifiedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their modification date (optional)
$ModifiedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their modification date (optional)
$ResponseFields = "{return_code,return_message,pagination,result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "force_all")
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# subscriber.list
try {
    $Result = Invoke-SubscriberList -Start $Start -Count $Count -PageCursor $PageCursor -Subscribed $Subscribed -StoreId $StoreId -Email $Email -CreatedFrom $CreatedFrom -CreatedTo $CreatedTo -ModifiedFrom $ModifiedFrom -ModifiedTo $ModifiedTo -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-SubscriberList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **Subscribed** | **Boolean**| Filter by subscription status | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **Email** | **String**| Filter subscribers by email | [optional] 
 **CreatedFrom** | **String**| Retrieve entities from their creation date | [optional] 
 **CreatedTo** | **String**| Retrieve entities to their creation date | [optional] 
 **ModifiedFrom** | **String**| Retrieve entities from their modification date | [optional] 
 **ModifiedTo** | **String**| Retrieve entities to their modification date | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;force_all&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseSubscriberList**](ModelResponseSubscriberList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

