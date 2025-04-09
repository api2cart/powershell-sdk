# PSOpenAPITools.PSOpenAPITools\Api.CategoryApi

All URIs are relative to *https://api.api2cart.com/v1.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Get-egoryAdd**](CategoryApi.md#Get-egoryAdd) | **POST** /category.add.json | category.add
[**Get-egoryAddBatch**](CategoryApi.md#Get-egoryAddBatch) | **POST** /category.add.batch.json | category.add.batch
[**Get-egoryAssign**](CategoryApi.md#Get-egoryAssign) | **POST** /category.assign.json | category.assign
[**Get-egoryCount**](CategoryApi.md#Get-egoryCount) | **GET** /category.count.json | category.count
[**Get-egoryDelete**](CategoryApi.md#Get-egoryDelete) | **DELETE** /category.delete.json | category.delete
[**Get-egoryFind**](CategoryApi.md#Get-egoryFind) | **GET** /category.find.json | category.find
[**Get-egoryImageAdd**](CategoryApi.md#Get-egoryImageAdd) | **POST** /category.image.add.json | category.image.add
[**Get-egoryImageDelete**](CategoryApi.md#Get-egoryImageDelete) | **DELETE** /category.image.delete.json | category.image.delete
[**Get-egoryInfo**](CategoryApi.md#Get-egoryInfo) | **GET** /category.info.json | category.info
[**Get-egoryList**](CategoryApi.md#Get-egoryList) | **GET** /category.list.json | category.list
[**Get-egoryUnassign**](CategoryApi.md#Get-egoryUnassign) | **POST** /category.unassign.json | category.unassign
[**Get-egoryUpdate**](CategoryApi.md#Get-egoryUpdate) | **PUT** /category.update.json | category.update


<a id="Get-egoryAdd"></a>
# **Get-egoryAdd**
> CategoryAdd200Response Get-egoryAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Name] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ParentId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoresIds] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Avail] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SortOrder] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTime] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTime] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Description] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShortDescription] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-MetaTitle] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-MetaDescription] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-MetaKeywords] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SeoUrl] <String><br>

category.add

Add new category in store

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

$Name = "Shoes" # String | Defines category's name that has to be added
$ParentId = "6" # String | Adds categories specified by parent id (optional)
$StoresIds = "1,2" # String | Create category in the stores that is specified by comma-separated stores' id (optional)
$StoreId = "1" # String | Store Id (optional)
$LangId = "3" # String | Language id (optional)
$Avail = $false # Boolean | Defines category's visibility status (optional) (default to $true)
$SortOrder = 2 # Int32 | Sort number in the list (optional) (default to 0)
$CreatedTime = "2014-01-30 15:58:41" # String | Entity's date creation (optional)
$ModifiedTime = "2014-07-30 15:58:41" # String | Entity's date modification (optional)
$Description = "Test category" # String | Defines category's description (optional)
$ShortDescription = "Short description. This is very short description" # String | Defines short description (optional)
$MetaTitle = "category,test" # String | Defines unique meta title for each entity (optional)
$MetaDescription = "category,test" # String | Defines unique meta description of a entity (optional)
$MetaKeywords = "category,test" # String | Defines unique meta keywords for each entity (optional)
$SeoUrl = "category,test" # String | Defines unique category's URL for SEO (optional)

# category.add
try {
    $Result = Get-egoryAdd -Name $Name -ParentId $ParentId -StoresIds $StoresIds -StoreId $StoreId -LangId $LangId -Avail $Avail -SortOrder $SortOrder -CreatedTime $CreatedTime -ModifiedTime $ModifiedTime -Description $Description -ShortDescription $ShortDescription -MetaTitle $MetaTitle -MetaDescription $MetaDescription -MetaKeywords $MetaKeywords -SeoUrl $SeoUrl
} catch {
    Write-Host ("Exception occurred when calling Get-egoryAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Name** | **String**| Defines category&#39;s name that has to be added | 
 **ParentId** | **String**| Adds categories specified by parent id | [optional] 
 **StoresIds** | **String**| Create category in the stores that is specified by comma-separated stores&#39; id | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **LangId** | **String**| Language id | [optional] 
 **Avail** | **Boolean**| Defines category&#39;s visibility status | [optional] [default to $true]
 **SortOrder** | **Int32**| Sort number in the list | [optional] [default to 0]
 **CreatedTime** | **String**| Entity&#39;s date creation | [optional] 
 **ModifiedTime** | **String**| Entity&#39;s date modification | [optional] 
 **Description** | **String**| Defines category&#39;s description | [optional] 
 **ShortDescription** | **String**| Defines short description | [optional] 
 **MetaTitle** | **String**| Defines unique meta title for each entity | [optional] 
 **MetaDescription** | **String**| Defines unique meta description of a entity | [optional] 
 **MetaKeywords** | **String**| Defines unique meta keywords for each entity | [optional] 
 **SeoUrl** | **String**| Defines unique category&#39;s URL for SEO | [optional] 

### Return type

[**CategoryAdd200Response**](CategoryAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Get-egoryAddBatch"></a>
# **Get-egoryAddBatch**
> CategoryAddBatch200Response Get-egoryAddBatch<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CategoryAddBatch] <PSCustomObject><br>

category.add.batch

Add new categories to the store.

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

$CategoryAddBatchPayloadInnerImagesInner = Initialize-CategoryAddBatchPayloadInnerImagesInner -Url "MyUrl" -ImageName "MyImageName" -Type "MyType" -Label "MyLabel"
$CategoryAddBatchPayloadInner = Initialize-CategoryAddBatchPayloadInner -Name "MyName" -Avail $false -Description "MyDescription" -MetaTitle "MyMetaTitle" -MetaDescription "MyMetaDescription" -MetaKeywords "MyMetaKeywords" -ParentId "MyParentId" -SortOrder 0 -SeoUrl "MySeoUrl" -StoreId "MyStoreId" -Images $CategoryAddBatchPayloadInnerImagesInner -StoresIds "MyStoresIds"

$CategoryAddBatch = Initialize-CategoryAddBatch -Payload $CategoryAddBatchPayloadInner # CategoryAddBatch | 

# category.add.batch
try {
    $Result = Get-egoryAddBatch -CategoryAddBatch $CategoryAddBatch
} catch {
    Write-Host ("Exception occurred when calling Get-egoryAddBatch: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **CategoryAddBatch** | [**CategoryAddBatch**](CategoryAddBatch.md)|  | 

### Return type

[**CategoryAddBatch200Response**](CategoryAddBatch200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Get-egoryAssign"></a>
# **Get-egoryAssign**
> CartConfigUpdate200Response Get-egoryAssign<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ProductId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CategoryId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

category.assign

Assign category to product

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

$ProductId = "10" # String | Defines category assign to the product, specified by product id
$CategoryId = "6" # String | Defines category assign, specified by category id
$StoreId = "1" # String | Store Id (optional)

# category.assign
try {
    $Result = Get-egoryAssign -ProductId $ProductId -CategoryId $CategoryId -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Get-egoryAssign: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ProductId** | **String**| Defines category assign to the product, specified by product id | 
 **CategoryId** | **String**| Defines category assign, specified by category id | 
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**CartConfigUpdate200Response**](CartConfigUpdate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Get-egoryCount"></a>
# **Get-egoryCount**
> CategoryCount200Response Get-egoryCount<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ParentId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Avail] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ProductType] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FindValue] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FindWhere] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ReportRequestId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DisableReportCache] <System.Nullable[Boolean]><br>

category.count

Count categories in store.

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

$ParentId = "6" # String | Counts categories specified by parent id (optional)
$StoreId = "1" # String | Counts category specified by store id (optional)
$LangId = "3" # String | Counts category specified by language id (optional)
$CreatedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their creation date (optional)
$CreatedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their creation date (optional)
$ModifiedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their modification date (optional)
$ModifiedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their modification date (optional)
$Avail = $false # Boolean | Defines category's visibility status (optional) (default to $true)
$ProductType = "BICYCLE" # String | A categorization for the product (optional)
$FindValue = "Demo category 1" # String | Entity search that is specified by some value (optional)
$FindWhere = "email" # String | Counts categories that are searched specified by field (optional)
$ReportRequestId = "105245017661" # String | Report request id (optional)
$DisableReportCache = $false # Boolean | Disable report cache for current request (optional) (default to $false)

# category.count
try {
    $Result = Get-egoryCount -ParentId $ParentId -StoreId $StoreId -LangId $LangId -CreatedFrom $CreatedFrom -CreatedTo $CreatedTo -ModifiedFrom $ModifiedFrom -ModifiedTo $ModifiedTo -Avail $Avail -ProductType $ProductType -FindValue $FindValue -FindWhere $FindWhere -ReportRequestId $ReportRequestId -DisableReportCache $DisableReportCache
} catch {
    Write-Host ("Exception occurred when calling Get-egoryCount: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ParentId** | **String**| Counts categories specified by parent id | [optional] 
 **StoreId** | **String**| Counts category specified by store id | [optional] 
 **LangId** | **String**| Counts category specified by language id | [optional] 
 **CreatedFrom** | **String**| Retrieve entities from their creation date | [optional] 
 **CreatedTo** | **String**| Retrieve entities to their creation date | [optional] 
 **ModifiedFrom** | **String**| Retrieve entities from their modification date | [optional] 
 **ModifiedTo** | **String**| Retrieve entities to their modification date | [optional] 
 **Avail** | **Boolean**| Defines category&#39;s visibility status | [optional] [default to $true]
 **ProductType** | **String**| A categorization for the product | [optional] 
 **FindValue** | **String**| Entity search that is specified by some value | [optional] 
 **FindWhere** | **String**| Counts categories that are searched specified by field | [optional] 
 **ReportRequestId** | **String**| Report request id | [optional] 
 **DisableReportCache** | **Boolean**| Disable report cache for current request | [optional] [default to $false]

### Return type

[**CategoryCount200Response**](CategoryCount200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Get-egoryDelete"></a>
# **Get-egoryDelete**
> CategoryDelete200Response Get-egoryDelete<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

category.delete

Delete category in store

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

$Id = "10" # String | Defines category removal, specified by category id
$StoreId = "1" # String | Store Id (optional)

# category.delete
try {
    $Result = Get-egoryDelete -Id $Id -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Get-egoryDelete: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Defines category removal, specified by category id | 
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**CategoryDelete200Response**](CategoryDelete200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Get-egoryFind"></a>
# **Get-egoryFind**
> CategoryFind200Response Get-egoryFind<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FindValue] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FindWhere] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FindParams] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>

category.find

Search category in store. ""Laptop"" is specified here by default.

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

$FindValue = "Demo category 1" # String | Entity search that is specified by some value
$FindWhere = "name" # String | Entity search that is specified by the comma-separated unique fields (optional) (default to "name")
$FindParams = "regex" # String | Entity search that is specified by comma-separated parameters (optional) (default to "whole_words")
$StoreId = "1" # String | Store Id (optional)
$LangId = "3" # String | Language id (optional)

# category.find
try {
    $Result = Get-egoryFind -FindValue $FindValue -FindWhere $FindWhere -FindParams $FindParams -StoreId $StoreId -LangId $LangId
} catch {
    Write-Host ("Exception occurred when calling Get-egoryFind: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **FindValue** | **String**| Entity search that is specified by some value | 
 **FindWhere** | **String**| Entity search that is specified by the comma-separated unique fields | [optional] [default to &quot;name&quot;]
 **FindParams** | **String**| Entity search that is specified by comma-separated parameters | [optional] [default to &quot;whole_words&quot;]
 **StoreId** | **String**| Store Id | [optional] 
 **LangId** | **String**| Language id | [optional] 

### Return type

[**CategoryFind200Response**](CategoryFind200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Get-egoryImageAdd"></a>
# **Get-egoryImageAdd**
> CategoryImageAdd200Response Get-egoryImageAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CategoryId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ImageName] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Url] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Type] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Label] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Mime] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Position] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

category.image.add

Add image to category

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

$CategoryId = "6" # String | Defines category id where the image should be added
$ImageName = "bag-gray.png" # String | Defines image's name
$Url = "http://docs.api2cart.com/img/logo.png" # String | Defines URL of the image that has to be added
$Type = "base" # String | Defines image's types that are specified by comma-separated list
$Label = "This cool image" # String | Defines alternative text that has to be attached to the picture (optional)
$Mime = "image/jpeg" # String | Mime type of image http://en.wikipedia.org/wiki/Internet_media_type. (optional)
$Position = 5 # Int32 | Defines image’s position in the list (optional) (default to 0)
$StoreId = "1" # String | Store Id (optional)

# category.image.add
try {
    $Result = Get-egoryImageAdd -CategoryId $CategoryId -ImageName $ImageName -Url $Url -Type $Type -Label $Label -Mime $Mime -Position $Position -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Get-egoryImageAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **CategoryId** | **String**| Defines category id where the image should be added | 
 **ImageName** | **String**| Defines image&#39;s name | 
 **Url** | **String**| Defines URL of the image that has to be added | 
 **Type** | **String**| Defines image&#39;s types that are specified by comma-separated list | 
 **Label** | **String**| Defines alternative text that has to be attached to the picture | [optional] 
 **Mime** | **String**| Mime type of image http://en.wikipedia.org/wiki/Internet_media_type. | [optional] 
 **Position** | **Int32**| Defines image’s position in the list | [optional] [default to 0]
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**CategoryImageAdd200Response**](CategoryImageAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Get-egoryImageDelete"></a>
# **Get-egoryImageDelete**
> AttributeDelete200Response Get-egoryImageDelete<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CategoryId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ImageId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

category.image.delete

Delete image

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

$CategoryId = "6" # String | Defines category id where the image should be deleted
$ImageId = "82950b84f468edff480680f99cedbe0d" # String | Define image id
$StoreId = "1" # String | Store Id (optional)

# category.image.delete
try {
    $Result = Get-egoryImageDelete -CategoryId $CategoryId -ImageId $ImageId -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Get-egoryImageDelete: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **CategoryId** | **String**| Defines category id where the image should be deleted | 
 **ImageId** | **String**| Define image id | 
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**AttributeDelete200Response**](AttributeDelete200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Get-egoryInfo"></a>
# **Get-egoryInfo**
> CategoryInfo200Response Get-egoryInfo<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SchemaType] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ReportRequestId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DisableReportCache] <System.Nullable[Boolean]><br>

category.info

Get category info about category ID*** or specify other category ID.

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

$Id = "10" # String | Retrieves category's info specified by category id
$Params = "id,parent_id,name" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,parent_id,name,description")
$ResponseFields = "{result{id,name,parent_id,modified_at{value},images}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Exclude = "id,parent_id,name" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)
$StoreId = "1" # String | Retrieves category info  specified by store id (optional)
$LangId = "3" # String | Retrieves category info  specified by language id (optional)
$SchemaType = "LISTING" # String | The name of the requirements set for the provided schema. (optional)
$ReportRequestId = "105245017661" # String | Report request id (optional)
$DisableReportCache = $false # Boolean | Disable report cache for current request (optional) (default to $false)

# category.info
try {
    $Result = Get-egoryInfo -Id $Id -Params $Params -ResponseFields $ResponseFields -Exclude $Exclude -StoreId $StoreId -LangId $LangId -SchemaType $SchemaType -ReportRequestId $ReportRequestId -DisableReportCache $DisableReportCache
} catch {
    Write-Host ("Exception occurred when calling Get-egoryInfo: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Retrieves category&#39;s info specified by category id | 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,parent_id,name,description&quot;]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 
 **StoreId** | **String**| Retrieves category info  specified by store id | [optional] 
 **LangId** | **String**| Retrieves category info  specified by language id | [optional] 
 **SchemaType** | **String**| The name of the requirements set for the provided schema. | [optional] 
 **ReportRequestId** | **String**| Report request id | [optional] 
 **DisableReportCache** | **Boolean**| Disable report cache for current request | [optional] [default to $false]

### Return type

[**CategoryInfo200Response**](CategoryInfo200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Get-egoryList"></a>
# **Get-egoryList**
> ModelResponseCategoryList Get-egoryList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ParentId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Avail] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ProductType] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FindValue] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FindWhere] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ReportRequestId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DisableReportCache] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DisableCache] <System.Nullable[Boolean]><br>

category.list

Get list of categories from store.

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
$ParentId = "6" # String | Retrieves categories specified by parent id (optional)
$Params = "id,parent_id,name" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,parent_id,name,description")
$ResponseFields = "{result{categories_count,category{id,parent_id,modified_at{value},images}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Exclude = "id,parent_id,name" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)
$StoreId = "1" # String | Retrieves categories specified by store id (optional)
$LangId = "3" # String | Retrieves categorys specified by language id (optional)
$CreatedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their creation date (optional)
$CreatedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their creation date (optional)
$ModifiedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their modification date (optional)
$ModifiedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their modification date (optional)
$Avail = $false # Boolean | Defines category's visibility status (optional) (default to $true)
$ProductType = "BICYCLE" # String | A categorization for the product (optional)
$FindValue = "Demo category 1" # String | Entity search that is specified by some value (optional)
$FindWhere = "name" # String | Category search that is specified by field (optional)
$ReportRequestId = "105245017661" # String | Report request id (optional)
$DisableReportCache = $false # Boolean | Disable report cache for current request (optional) (default to $false)
$DisableCache = $false # Boolean | Disable cache for current request (optional) (default to $false)

# category.list
try {
    $Result = Get-egoryList -Start $Start -Count $Count -PageCursor $PageCursor -ParentId $ParentId -Params $Params -ResponseFields $ResponseFields -Exclude $Exclude -StoreId $StoreId -LangId $LangId -CreatedFrom $CreatedFrom -CreatedTo $CreatedTo -ModifiedFrom $ModifiedFrom -ModifiedTo $ModifiedTo -Avail $Avail -ProductType $ProductType -FindValue $FindValue -FindWhere $FindWhere -ReportRequestId $ReportRequestId -DisableReportCache $DisableReportCache -DisableCache $DisableCache
} catch {
    Write-Host ("Exception occurred when calling Get-egoryList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **ParentId** | **String**| Retrieves categories specified by parent id | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,parent_id,name,description&quot;]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 
 **StoreId** | **String**| Retrieves categories specified by store id | [optional] 
 **LangId** | **String**| Retrieves categorys specified by language id | [optional] 
 **CreatedFrom** | **String**| Retrieve entities from their creation date | [optional] 
 **CreatedTo** | **String**| Retrieve entities to their creation date | [optional] 
 **ModifiedFrom** | **String**| Retrieve entities from their modification date | [optional] 
 **ModifiedTo** | **String**| Retrieve entities to their modification date | [optional] 
 **Avail** | **Boolean**| Defines category&#39;s visibility status | [optional] [default to $true]
 **ProductType** | **String**| A categorization for the product | [optional] 
 **FindValue** | **String**| Entity search that is specified by some value | [optional] 
 **FindWhere** | **String**| Category search that is specified by field | [optional] 
 **ReportRequestId** | **String**| Report request id | [optional] 
 **DisableReportCache** | **Boolean**| Disable report cache for current request | [optional] [default to $false]
 **DisableCache** | **Boolean**| Disable cache for current request | [optional] [default to $false]

### Return type

[**ModelResponseCategoryList**](ModelResponseCategoryList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Get-egoryUnassign"></a>
# **Get-egoryUnassign**
> CartConfigUpdate200Response Get-egoryUnassign<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CategoryId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ProductId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

category.unassign

Unassign category to product

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

$CategoryId = "6" # String | Defines category unassign, specified by category id
$ProductId = "10" # String | Defines category unassign to the product, specified by product id
$StoreId = "1" # String | Store Id (optional)

# category.unassign
try {
    $Result = Get-egoryUnassign -CategoryId $CategoryId -ProductId $ProductId -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Get-egoryUnassign: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **CategoryId** | **String**| Defines category unassign, specified by category id | 
 **ProductId** | **String**| Defines category unassign to the product, specified by product id | 
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**CartConfigUpdate200Response**](CartConfigUpdate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Get-egoryUpdate"></a>
# **Get-egoryUpdate**
> AccountConfigUpdate200Response Get-egoryUpdate<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Name] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ParentId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoresIds] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Avail] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SortOrder] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTime] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Description] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShortDescription] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-MetaTitle] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-MetaDescription] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-MetaKeywords] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SeoUrl] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

category.update

Update category in store

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

$Id = "10" # String | Defines category update specified by category id
$Name = "NEW Shoes" # String | Defines new category’s name (optional)
$ParentId = "6" # String | Defines new parent category id (optional)
$StoresIds = "1,2" # String | Update category in the stores that is specified by comma-separated stores' id (optional)
$Avail = $false # Boolean | Defines category's visibility status (optional)
$SortOrder = 2 # Int32 | Sort number in the list (optional)
$ModifiedTime = "2014-07-30 15:58:41" # String | Entity's date modification (optional)
$Description = "New test category" # String | Defines new category's description (optional)
$ShortDescription = "Short description. This is very short description" # String | Defines short description (optional)
$MetaTitle = "category,test" # String | Defines unique meta title for each entity (optional)
$MetaDescription = "category,test" # String | Defines unique meta description of a entity (optional)
$MetaKeywords = "category,test" # String | Defines unique meta keywords for each entity (optional)
$SeoUrl = "category,test" # String | Defines unique category's URL for SEO (optional)
$LangId = "3" # String | Language id (optional)
$StoreId = "1" # String | Store Id (optional)

# category.update
try {
    $Result = Get-egoryUpdate -Id $Id -Name $Name -ParentId $ParentId -StoresIds $StoresIds -Avail $Avail -SortOrder $SortOrder -ModifiedTime $ModifiedTime -Description $Description -ShortDescription $ShortDescription -MetaTitle $MetaTitle -MetaDescription $MetaDescription -MetaKeywords $MetaKeywords -SeoUrl $SeoUrl -LangId $LangId -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Get-egoryUpdate: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Defines category update specified by category id | 
 **Name** | **String**| Defines new category’s name | [optional] 
 **ParentId** | **String**| Defines new parent category id | [optional] 
 **StoresIds** | **String**| Update category in the stores that is specified by comma-separated stores&#39; id | [optional] 
 **Avail** | **Boolean**| Defines category&#39;s visibility status | [optional] 
 **SortOrder** | **Int32**| Sort number in the list | [optional] 
 **ModifiedTime** | **String**| Entity&#39;s date modification | [optional] 
 **Description** | **String**| Defines new category&#39;s description | [optional] 
 **ShortDescription** | **String**| Defines short description | [optional] 
 **MetaTitle** | **String**| Defines unique meta title for each entity | [optional] 
 **MetaDescription** | **String**| Defines unique meta description of a entity | [optional] 
 **MetaKeywords** | **String**| Defines unique meta keywords for each entity | [optional] 
 **SeoUrl** | **String**| Defines unique category&#39;s URL for SEO | [optional] 
 **LangId** | **String**| Language id | [optional] 
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**AccountConfigUpdate200Response**](AccountConfigUpdate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

