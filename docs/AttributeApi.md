# PSOpenAPITools.PSOpenAPITools\Api.AttributeApi

All URIs are relative to *https://api.api2cart.local.com/v1.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Invoke-AttributeAdd**](AttributeApi.md#Invoke-AttributeAdd) | **POST** /attribute.add.json | attribute.add
[**Invoke-AttributeAssignGroup**](AttributeApi.md#Invoke-AttributeAssignGroup) | **POST** /attribute.assign.group.json | attribute.assign.group
[**Invoke-AttributeAssignSet**](AttributeApi.md#Invoke-AttributeAssignSet) | **POST** /attribute.assign.set.json | attribute.assign.set
[**Invoke-AttributeAttributesetList**](AttributeApi.md#Invoke-AttributeAttributesetList) | **GET** /attribute.attributeset.list.json | attribute.attributeset.list
[**Invoke-AttributeCount**](AttributeApi.md#Invoke-AttributeCount) | **GET** /attribute.count.json | attribute.count
[**Invoke-AttributeDelete**](AttributeApi.md#Invoke-AttributeDelete) | **DELETE** /attribute.delete.json | attribute.delete
[**Invoke-AttributeGroupList**](AttributeApi.md#Invoke-AttributeGroupList) | **GET** /attribute.group.list.json | attribute.group.list
[**Invoke-AttributeInfo**](AttributeApi.md#Invoke-AttributeInfo) | **GET** /attribute.info.json | attribute.info
[**Invoke-AttributeList**](AttributeApi.md#Invoke-AttributeList) | **GET** /attribute.list.json | attribute.list
[**Invoke-AttributeTypeList**](AttributeApi.md#Invoke-AttributeTypeList) | **GET** /attribute.type.list.json | attribute.type.list
[**Invoke-AttributeUnassignGroup**](AttributeApi.md#Invoke-AttributeUnassignGroup) | **POST** /attribute.unassign.group.json | attribute.unassign.group
[**Invoke-AttributeUnassignSet**](AttributeApi.md#Invoke-AttributeUnassignSet) | **POST** /attribute.unassign.set.json | attribute.unassign.set
[**Invoke-AttributeUpdate**](AttributeApi.md#Invoke-AttributeUpdate) | **PUT** /attribute.update.json | attribute.update
[**Invoke-AttributeValueAdd**](AttributeApi.md#Invoke-AttributeValueAdd) | **POST** /attribute.value.add.json | attribute.value.add
[**Invoke-AttributeValueDelete**](AttributeApi.md#Invoke-AttributeValueDelete) | **DELETE** /attribute.value.delete.json | attribute.value.delete
[**Invoke-AttributeValueUpdate**](AttributeApi.md#Invoke-AttributeValueUpdate) | **PUT** /attribute.value.update.json | attribute.value.update


<a id="Invoke-AttributeAdd"></a>
# **Invoke-AttributeAdd**
> AttributeAdd200Response Invoke-AttributeAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Type] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Name] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Code] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Visible] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Required] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Position] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AttributeGroupId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-IsGlobal] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-IsSearchable] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-IsFilterable] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-IsComparable] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-IsHtmlAllowedOnFront] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-IsFilterableInSearch] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-IsConfigurable] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-IsVisibleInAdvancedSearch] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-IsUsedForPromoRules] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-UsedInProductListing] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-UsedForSortBy] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ApplyTo] <String><br>

attribute.add

Add new attribute

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

$Type = "text" # String | Defines attribute's type
$Name = "Specification" # String | Defines attributes's name
$Code = "code" # String | Entity code (optional)
$StoreId = "1" # String | Store Id (optional)
$LangId = "3" # String | Language id (optional)
$Visible = $true # Boolean | Set visibility status (optional) (default to $false)
$Required = $true # Boolean | Defines if the option is required (optional) (default to $false)
$Position = 5 # Int32 | Attribute`s position (optional) (default to 0)
$AttributeGroupId = "202" # String | Filter by attribute_group_id (optional)
$IsGlobal = "Global" # String | Attribute saving scope (optional) (default to "Store")
$IsSearchable = $false # Boolean | Use attribute in Quick Search (optional) (default to $false)
$IsFilterable = "No" # String | Use In Layered Navigation (optional) (default to "No")
$IsComparable = $true # Boolean | Comparable on Front-end (optional) (default to $false)
$IsHtmlAllowedOnFront = $true # Boolean | Allow HTML Tags on Frontend (optional) (default to $false)
$IsFilterableInSearch = $true # Boolean | Use In Search Results Layered Navigation (optional) (default to $false)
$IsConfigurable = $true # Boolean | Use To Create Configurable Product (optional) (default to $false)
$IsVisibleInAdvancedSearch = $true # Boolean | Use in Advanced Search (optional) (default to $false)
$IsUsedForPromoRules = $true # Boolean | Use for Promo Rule Conditions (optional) (default to $false)
$UsedInProductListing = $true # Boolean | Used in Product Listing (optional) (default to $false)
$UsedForSortBy = $true # Boolean | Used for Sorting in Product Listing (optional) (default to $false)
$ApplyTo = "Global" # String | Types of products which can have this attribute (optional) (default to "all_types")

# attribute.add
try {
    $Result = Invoke-AttributeAdd -Type $Type -Name $Name -Code $Code -StoreId $StoreId -LangId $LangId -Visible $Visible -Required $Required -Position $Position -AttributeGroupId $AttributeGroupId -IsGlobal $IsGlobal -IsSearchable $IsSearchable -IsFilterable $IsFilterable -IsComparable $IsComparable -IsHtmlAllowedOnFront $IsHtmlAllowedOnFront -IsFilterableInSearch $IsFilterableInSearch -IsConfigurable $IsConfigurable -IsVisibleInAdvancedSearch $IsVisibleInAdvancedSearch -IsUsedForPromoRules $IsUsedForPromoRules -UsedInProductListing $UsedInProductListing -UsedForSortBy $UsedForSortBy -ApplyTo $ApplyTo
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Type** | **String**| Defines attribute&#39;s type | 
 **Name** | **String**| Defines attributes&#39;s name | 
 **Code** | **String**| Entity code | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **LangId** | **String**| Language id | [optional] 
 **Visible** | **Boolean**| Set visibility status | [optional] [default to $false]
 **Required** | **Boolean**| Defines if the option is required | [optional] [default to $false]
 **Position** | **Int32**| Attribute&#x60;s position | [optional] [default to 0]
 **AttributeGroupId** | **String**| Filter by attribute_group_id | [optional] 
 **IsGlobal** | **String**| Attribute saving scope | [optional] [default to &quot;Store&quot;]
 **IsSearchable** | **Boolean**| Use attribute in Quick Search | [optional] [default to $false]
 **IsFilterable** | **String**| Use In Layered Navigation | [optional] [default to &quot;No&quot;]
 **IsComparable** | **Boolean**| Comparable on Front-end | [optional] [default to $false]
 **IsHtmlAllowedOnFront** | **Boolean**| Allow HTML Tags on Frontend | [optional] [default to $false]
 **IsFilterableInSearch** | **Boolean**| Use In Search Results Layered Navigation | [optional] [default to $false]
 **IsConfigurable** | **Boolean**| Use To Create Configurable Product | [optional] [default to $false]
 **IsVisibleInAdvancedSearch** | **Boolean**| Use in Advanced Search | [optional] [default to $false]
 **IsUsedForPromoRules** | **Boolean**| Use for Promo Rule Conditions | [optional] [default to $false]
 **UsedInProductListing** | **Boolean**| Used in Product Listing | [optional] [default to $false]
 **UsedForSortBy** | **Boolean**| Used for Sorting in Product Listing | [optional] [default to $false]
 **ApplyTo** | **String**| Types of products which can have this attribute | [optional] [default to &quot;all_types&quot;]

### Return type

[**AttributeAdd200Response**](AttributeAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AttributeAssignGroup"></a>
# **Invoke-AttributeAssignGroup**
> AttributeAssignGroup200Response Invoke-AttributeAssignGroup<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-GroupId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AttributeSetId] <String><br>

attribute.assign.group

Assign attribute to the group

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
$GroupId = "3" # String | Attribute group_id
$AttributeSetId = "4" # String | Attribute set id (optional)

# attribute.assign.group
try {
    $Result = Invoke-AttributeAssignGroup -Id $Id -GroupId $GroupId -AttributeSetId $AttributeSetId
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeAssignGroup: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Entity id | 
 **GroupId** | **String**| Attribute group_id | 
 **AttributeSetId** | **String**| Attribute set id | [optional] 

### Return type

[**AttributeAssignGroup200Response**](AttributeAssignGroup200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AttributeAssignSet"></a>
# **Invoke-AttributeAssignSet**
> AttributeAssignGroup200Response Invoke-AttributeAssignSet<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AttributeSetId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-GroupId] <String><br>

attribute.assign.set

Assign attribute to the attribute set

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
$AttributeSetId = "4" # String | Attribute set id
$GroupId = "3" # String | Attribute group_id (optional)

# attribute.assign.set
try {
    $Result = Invoke-AttributeAssignSet -Id $Id -AttributeSetId $AttributeSetId -GroupId $GroupId
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeAssignSet: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Entity id | 
 **AttributeSetId** | **String**| Attribute set id | 
 **GroupId** | **String**| Attribute group_id | [optional] 

### Return type

[**AttributeAssignGroup200Response**](AttributeAssignGroup200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AttributeAttributesetList"></a>
# **Invoke-AttributeAttributesetList**
> ModelResponseAttributeAttributesetList Invoke-AttributeAttributesetList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

attribute.attributeset.list

Get attribute_set list

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
$ResponseFields = "{result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,name" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,name")
$Exclude = "id,name" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# attribute.attributeset.list
try {
    $Result = Invoke-AttributeAttributesetList -Start $Start -Count $Count -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeAttributesetList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,name&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseAttributeAttributesetList**](ModelResponseAttributeAttributesetList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AttributeCount"></a>
# **Invoke-AttributeCount**
> AttributeCount200Response Invoke-AttributeCount<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Type] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AttributeSetId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Visible] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Required] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-System] <System.Nullable[Boolean]><br>

attribute.count

Get attributes count

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

$Type = "text" # String | Defines attribute's type (optional)
$AttributeSetId = "4" # String | Filter items by attribute set id (optional)
$StoreId = "1" # String | Store Id (optional)
$LangId = "3" # String | Language id (optional)
$Visible = $true # Boolean | Filter items by visibility status (optional)
$Required = $true # Boolean | Defines if the option is required (optional)
$System = $false # Boolean | True if attribute is system (optional)

# attribute.count
try {
    $Result = Invoke-AttributeCount -Type $Type -AttributeSetId $AttributeSetId -StoreId $StoreId -LangId $LangId -Visible $Visible -Required $Required -System $System
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeCount: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Type** | **String**| Defines attribute&#39;s type | [optional] 
 **AttributeSetId** | **String**| Filter items by attribute set id | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **LangId** | **String**| Language id | [optional] 
 **Visible** | **Boolean**| Filter items by visibility status | [optional] 
 **Required** | **Boolean**| Defines if the option is required | [optional] 
 **System** | **Boolean**| True if attribute is system | [optional] 

### Return type

[**AttributeCount200Response**](AttributeCount200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AttributeDelete"></a>
# **Invoke-AttributeDelete**
> AttributeDelete200Response Invoke-AttributeDelete<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

attribute.delete

Delete attribute from store

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

# attribute.delete
try {
    $Result = Invoke-AttributeDelete -Id $Id -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeDelete: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Entity id | 
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**AttributeDelete200Response**](AttributeDelete200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AttributeGroupList"></a>
# **Invoke-AttributeGroupList**
> ModelResponseAttributeGroupList Invoke-AttributeGroupList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AttributeSetId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

attribute.group.list

Get attribute group list

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
$AttributeSetId = "4" # String | Attribute set id (optional)
$LangId = "3" # String | Language id (optional)
$ResponseFields = "{result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,name" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,name")
$Exclude = "id,name" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# attribute.group.list
try {
    $Result = Invoke-AttributeGroupList -Start $Start -Count $Count -AttributeSetId $AttributeSetId -LangId $LangId -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeGroupList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **AttributeSetId** | **String**| Attribute set id | [optional] 
 **LangId** | **String**| Language id | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,name&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseAttributeGroupList**](ModelResponseAttributeGroupList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AttributeInfo"></a>
# **Invoke-AttributeInfo**
> AttributeInfo200Response Invoke-AttributeInfo<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AttributeSetId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

attribute.info

Get information about a specific global attribute by its ID.

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
$AttributeSetId = "4" # String | Attribute set id (optional)
$StoreId = "1" # String | Store Id (optional)
$LangId = "3" # String | Language id (optional)
$ResponseFields = "{result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "force_all" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "force_all")
$Exclude = "name" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# attribute.info
try {
    $Result = Invoke-AttributeInfo -Id $Id -AttributeSetId $AttributeSetId -StoreId $StoreId -LangId $LangId -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeInfo: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Entity id | 
 **AttributeSetId** | **String**| Attribute set id | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **LangId** | **String**| Language id | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;force_all&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**AttributeInfo200Response**](AttributeInfo200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AttributeList"></a>
# **Invoke-AttributeList**
> ModelResponseAttributeList Invoke-AttributeList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AttributeIds] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AttributeSetId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Type] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Visible] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Required] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-System] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

attribute.list

Get a list of global attributes.

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
$AttributeIds = "1,2,3" # String | Filter attributes by ids (optional)
$AttributeSetId = "4" # String | Filter items by attribute set id (optional)
$StoreId = "1" # String | Store Id (optional)
$LangId = "3" # String | Retrieves attributes on specified language id (optional)
$Type = "text" # String | Defines attribute's type (optional)
$Visible = $true # Boolean | Filter items by visibility status (optional)
$Required = $true # Boolean | Defines if the option is required (optional)
$System = $false # Boolean | True if attribute is system (optional)
$ResponseFields = "{return_code,return_message,pagination,result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,name" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,name,code,type")
$Exclude = "id,name" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# attribute.list
try {
    $Result = Invoke-AttributeList -Start $Start -Count $Count -AttributeIds $AttributeIds -AttributeSetId $AttributeSetId -StoreId $StoreId -LangId $LangId -Type $Type -Visible $Visible -Required $Required -System $System -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **AttributeIds** | **String**| Filter attributes by ids | [optional] 
 **AttributeSetId** | **String**| Filter items by attribute set id | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **LangId** | **String**| Retrieves attributes on specified language id | [optional] 
 **Type** | **String**| Defines attribute&#39;s type | [optional] 
 **Visible** | **Boolean**| Filter items by visibility status | [optional] 
 **Required** | **Boolean**| Defines if the option is required | [optional] 
 **System** | **Boolean**| True if attribute is system | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,name,code,type&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseAttributeList**](ModelResponseAttributeList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AttributeTypeList"></a>
# **Invoke-AttributeTypeList**
> AttributeTypeList200Response Invoke-AttributeTypeList<br>

attribute.type.list

Get list of supported attributes types

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


# attribute.type.list
try {
    $Result = Invoke-AttributeTypeList
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeTypeList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AttributeTypeList200Response**](AttributeTypeList200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AttributeUnassignGroup"></a>
# **Invoke-AttributeUnassignGroup**
> AttributeUnassignGroup200Response Invoke-AttributeUnassignGroup<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-GroupId] <String><br>

attribute.unassign.group

Unassign attribute from group

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
$GroupId = "3" # String | Customer group_id

# attribute.unassign.group
try {
    $Result = Invoke-AttributeUnassignGroup -Id $Id -GroupId $GroupId
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeUnassignGroup: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Entity id | 
 **GroupId** | **String**| Customer group_id | 

### Return type

[**AttributeUnassignGroup200Response**](AttributeUnassignGroup200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AttributeUnassignSet"></a>
# **Invoke-AttributeUnassignSet**
> AttributeUnassignGroup200Response Invoke-AttributeUnassignSet<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AttributeSetId] <String><br>

attribute.unassign.set

Unassign attribute from attribute set

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
$AttributeSetId = "4" # String | Attribute set id

# attribute.unassign.set
try {
    $Result = Invoke-AttributeUnassignSet -Id $Id -AttributeSetId $AttributeSetId
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeUnassignSet: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Entity id | 
 **AttributeSetId** | **String**| Attribute set id | 

### Return type

[**AttributeUnassignGroup200Response**](AttributeUnassignGroup200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AttributeUpdate"></a>
# **Invoke-AttributeUpdate**
> AttributeUpdate200Response Invoke-AttributeUpdate<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Name] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>

attribute.update

Update attribute data

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
$Name = "Test name" # String | Defines new attributes's name
$StoreId = "1" # String | Store Id (optional)
$LangId = "3" # String | Language id (optional)

# attribute.update
try {
    $Result = Invoke-AttributeUpdate -Id $Id -Name $Name -StoreId $StoreId -LangId $LangId
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeUpdate: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Entity id | 
 **Name** | **String**| Defines new attributes&#39;s name | 
 **StoreId** | **String**| Store Id | [optional] 
 **LangId** | **String**| Language id | [optional] 

### Return type

[**AttributeUpdate200Response**](AttributeUpdate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AttributeValueAdd"></a>
# **Invoke-AttributeValueAdd**
> AttributeAdd200Response Invoke-AttributeValueAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AttributeId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Name] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Code] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Description] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>

attribute.value.add

Add new value to attribute.

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

$AttributeId = "156" # String | Attribute Id
$Name = "Test name" # String | Defines attribute value's name
$Code = "code" # String | Entity code (optional)
$Description = "Test value" # String | Defines attribute value's description (optional)
$StoreId = "1" # String | Store Id (optional)
$LangId = "3" # String | Language id (optional)

# attribute.value.add
try {
    $Result = Invoke-AttributeValueAdd -AttributeId $AttributeId -Name $Name -Code $Code -Description $Description -StoreId $StoreId -LangId $LangId
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeValueAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **AttributeId** | **String**| Attribute Id | 
 **Name** | **String**| Defines attribute value&#39;s name | 
 **Code** | **String**| Entity code | [optional] 
 **Description** | **String**| Defines attribute value&#39;s description | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **LangId** | **String**| Language id | [optional] 

### Return type

[**AttributeAdd200Response**](AttributeAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AttributeValueDelete"></a>
# **Invoke-AttributeValueDelete**
> AttributeValueDelete200Response Invoke-AttributeValueDelete<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AttributeId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

attribute.value.delete

Delete attribute value.

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
$AttributeId = "156" # String | Attribute Id
$StoreId = "1" # String | Store Id (optional)

# attribute.value.delete
try {
    $Result = Invoke-AttributeValueDelete -Id $Id -AttributeId $AttributeId -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeValueDelete: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Entity id | 
 **AttributeId** | **String**| Attribute Id | 
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**AttributeValueDelete200Response**](AttributeValueDelete200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-AttributeValueUpdate"></a>
# **Invoke-AttributeValueUpdate**
> AttributeUpdate200Response Invoke-AttributeValueUpdate<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AttributeId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Name] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Description] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Code] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>

attribute.value.update

Update attribute value.

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

$Id = "10" # String | Defines attribute value's id
$AttributeId = "156" # String | Attribute Id
$Name = "Test name" # String | Defines attribute value's name (optional)
$Description = "Test value" # String | Defines new attribute value's description (optional)
$Code = "code" # String | Entity code (optional)
$StoreId = "1" # String | Store Id (optional)
$LangId = "3" # String | Language id (optional)

# attribute.value.update
try {
    $Result = Invoke-AttributeValueUpdate -Id $Id -AttributeId $AttributeId -Name $Name -Description $Description -Code $Code -StoreId $StoreId -LangId $LangId
} catch {
    Write-Host ("Exception occurred when calling Invoke-AttributeValueUpdate: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Defines attribute value&#39;s id | 
 **AttributeId** | **String**| Attribute Id | 
 **Name** | **String**| Defines attribute value&#39;s name | [optional] 
 **Description** | **String**| Defines new attribute value&#39;s description | [optional] 
 **Code** | **String**| Entity code | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **LangId** | **String**| Language id | [optional] 

### Return type

[**AttributeUpdate200Response**](AttributeUpdate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

