# PSOpenAPITools.PSOpenAPITools\Api.CustomerApi

All URIs are relative to *https://api.api2cart.com/v1.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Invoke-CustomerAdd**](CustomerApi.md#Invoke-CustomerAdd) | **POST** /customer.add.json | customer.add
[**Invoke-CustomerAddressAdd**](CustomerApi.md#Invoke-CustomerAddressAdd) | **POST** /customer.address.add.json | customer.address.add
[**Invoke-CustomerAttributeList**](CustomerApi.md#Invoke-CustomerAttributeList) | **GET** /customer.attribute.list.json | customer.attribute.list
[**Invoke-CustomerCount**](CustomerApi.md#Invoke-CustomerCount) | **GET** /customer.count.json | customer.count
[**Invoke-CustomerDelete**](CustomerApi.md#Invoke-CustomerDelete) | **DELETE** /customer.delete.json | customer.delete
[**Invoke-CustomerFind**](CustomerApi.md#Invoke-CustomerFind) | **GET** /customer.find.json | customer.find
[**Invoke-CustomerGroupAdd**](CustomerApi.md#Invoke-CustomerGroupAdd) | **POST** /customer.group.add.json | customer.group.add
[**Invoke-CustomerGroupList**](CustomerApi.md#Invoke-CustomerGroupList) | **GET** /customer.group.list.json | customer.group.list
[**Invoke-CustomerInfo**](CustomerApi.md#Invoke-CustomerInfo) | **GET** /customer.info.json | customer.info
[**Invoke-CustomerList**](CustomerApi.md#Invoke-CustomerList) | **GET** /customer.list.json | customer.list
[**Invoke-CustomerUpdate**](CustomerApi.md#Invoke-CustomerUpdate) | **PUT** /customer.update.json | customer.update
[**Invoke-CustomerWishlistList**](CustomerApi.md#Invoke-CustomerWishlistList) | **GET** /customer.wishlist.list.json | customer.wishlist.list


<a id="Invoke-CustomerAdd"></a>
# **Invoke-CustomerAdd**
> CustomerAdd200Response Invoke-CustomerAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerAdd] <PSCustomObject><br>

customer.add

Add customer into store.

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

$CustomerAddConsentsInner = Initialize-CustomerAddConsentsInner -Type "email" -Status "MyStatus" -OptInLevel "MyOptInLevel"
$CustomerAddAddressInner = Initialize-CustomerAddAddressInner -AddressBookType "billing" -AddressBookFirstName "John" -AddressBookLastName "Smith" -AddressBookCompany "Samsung" -AddressBookFax "5758787" -AddressBookPhone "5758787" -AddressBookPhoneMobile "5758787" -AddressBookWebsite "http://api2cart.com" -AddressBookAddress1 "Green str. 35" -AddressBookAddress2 "Green str. 35" -AddressBookCity "Chicago" -AddressBookCountry "US" -AddressBookState "IL" -AddressBookPostcode "12345" -AddressBookGender "male" -AddressBookRegion "Alabama" -AddressBookDefault $true -AddressBookTaxId "`12345678`" -AddressBookIdentificationNumber "`123-456-7890`" -AddressBookAlias "Address alias"
$CustomerAdd = Initialize-CustomerAdd -Email "mail@example.com" -FirstName "John" -LastName "Smith" -Password "fd5gfd5g75fd" -Group "Register" -GroupIds "1,2,3" -CreatedTime "2014-01-30 15:58:41" -ModifiedTime "2014-07-30 15:58:41" -Login "makaka" -LastLogin "2013-02-26 15:00:00" -BirthDay "2013-02-26 15:00:00" -Status "disabled" -NewsLetterSubscription $true -Consents $CustomerAddConsentsInner -Gender "male" -Website "http://api2cart.com" -StoreId "1" -Fax "54545787" -Company "Apple" -Phone "56686868654" -Note "Customer note" -Country "US" -Address $CustomerAddAddressInner # CustomerAdd | 

# customer.add
try {
    $Result = Invoke-CustomerAdd -CustomerAdd $CustomerAdd
} catch {
    Write-Host ("Exception occurred when calling Invoke-CustomerAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **CustomerAdd** | [**CustomerAdd**](CustomerAdd.md)|  | 

### Return type

[**CustomerAdd200Response**](CustomerAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CustomerAddressAdd"></a>
# **Invoke-CustomerAddressAdd**
> AttributeAdd200Response Invoke-CustomerAddressAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerAddressAdd] <PSCustomObject><br>

customer.address.add

Add customer address.

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

$CustomerAddressAdd = Initialize-CustomerAddressAdd -CustomerId "5" -StoreId "1" -FirstName "John" -LastName "Smith" -Company "Apple" -Address1 "Green str. 35" -Address2 "Green str. 35" -City "Chicago" -Country "US" -State "IL" -Postcode "12345" -IdentificationNumber "`123-456-7890`" -Types "MyTypes" -Default $true -Phone "56686868654" -PhoneMobile "56686868654" -Fax "54545787" -Website "http://api2cart.com" -Gender "male" -TaxId "`12345678`" -Alias "Address alias" # CustomerAddressAdd | 

# customer.address.add
try {
    $Result = Invoke-CustomerAddressAdd -CustomerAddressAdd $CustomerAddressAdd
} catch {
    Write-Host ("Exception occurred when calling Invoke-CustomerAddressAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **CustomerAddressAdd** | [**CustomerAddressAdd**](CustomerAddressAdd.md)|  | 

### Return type

[**AttributeAdd200Response**](AttributeAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CustomerAttributeList"></a>
# **Invoke-CustomerAttributeList**
> ModelResponseCustomerAttributeList Invoke-CustomerAttributeList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>

customer.attribute.list

Get attributes for specific customer

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
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$PageCursor = "MyPageCursor" # String | Used to retrieve entities via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$StoreId = "1" # String | Store Id (optional)
$LangId = "3" # String | Language id (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "force_all")
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)
$ResponseFields = "{return_code,return_message,pagination,result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)

# customer.attribute.list
try {
    $Result = Invoke-CustomerAttributeList -CustomerId $CustomerId -Count $Count -PageCursor $PageCursor -StoreId $StoreId -LangId $LangId -Params $Params -Exclude $Exclude -ResponseFields $ResponseFields
} catch {
    Write-Host ("Exception occurred when calling Invoke-CustomerAttributeList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **CustomerId** | **String**| Retrieves orders specified by customer id | 
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **LangId** | **String**| Language id | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;force_all&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 

### Return type

[**ModelResponseCustomerAttributeList**](ModelResponseCustomerAttributeList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CustomerCount"></a>
# **Invoke-CustomerCount**
> CustomerCount200Response Invoke-CustomerCount<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-GroupId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerListId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Avail] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FindValue] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FindWhere] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Ids] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SinceId] <String><br>

customer.count

Get number of customers from store.

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

$GroupId = "3" # String | Customer group_id (optional)
$CreatedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their creation date (optional)
$CreatedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their creation date (optional)
$ModifiedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their modification date (optional)
$ModifiedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their modification date (optional)
$StoreId = "1" # String | Counts customer specified by store id (optional)
$CustomerListId = "exampleListId" # String | The numeric ID of the customer list in Demandware. (optional)
$Avail = $false # Boolean | Defines category's visibility status (optional) (default to $true)
$FindValue = "mail@gmail.com" # String | Entity search that is specified by some value (optional)
$FindWhere = "email" # String | Counts customers that are searched specified by field (optional)
$Ids = "24,25" # String | Counts customers specified by ids (optional)
$SinceId = "56" # String | Retrieve entities starting from the specified id. (optional)

# customer.count
try {
    $Result = Invoke-CustomerCount -GroupId $GroupId -CreatedFrom $CreatedFrom -CreatedTo $CreatedTo -ModifiedFrom $ModifiedFrom -ModifiedTo $ModifiedTo -StoreId $StoreId -CustomerListId $CustomerListId -Avail $Avail -FindValue $FindValue -FindWhere $FindWhere -Ids $Ids -SinceId $SinceId
} catch {
    Write-Host ("Exception occurred when calling Invoke-CustomerCount: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **GroupId** | **String**| Customer group_id | [optional] 
 **CreatedFrom** | **String**| Retrieve entities from their creation date | [optional] 
 **CreatedTo** | **String**| Retrieve entities to their creation date | [optional] 
 **ModifiedFrom** | **String**| Retrieve entities from their modification date | [optional] 
 **ModifiedTo** | **String**| Retrieve entities to their modification date | [optional] 
 **StoreId** | **String**| Counts customer specified by store id | [optional] 
 **CustomerListId** | **String**| The numeric ID of the customer list in Demandware. | [optional] 
 **Avail** | **Boolean**| Defines category&#39;s visibility status | [optional] [default to $true]
 **FindValue** | **String**| Entity search that is specified by some value | [optional] 
 **FindWhere** | **String**| Counts customers that are searched specified by field | [optional] 
 **Ids** | **String**| Counts customers specified by ids | [optional] 
 **SinceId** | **String**| Retrieve entities starting from the specified id. | [optional] 

### Return type

[**CustomerCount200Response**](CustomerCount200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CustomerDelete"></a>
# **Invoke-CustomerDelete**
> CustomerDelete200Response Invoke-CustomerDelete<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>

customer.delete

Delete customer from store.

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

$Id = "10" # String | Identifies customer specified by the id

# customer.delete
try {
    $Result = Invoke-CustomerDelete -Id $Id
} catch {
    Write-Host ("Exception occurred when calling Invoke-CustomerDelete: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Identifies customer specified by the id | 

### Return type

[**CustomerDelete200Response**](CustomerDelete200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CustomerFind"></a>
# **Invoke-CustomerFind**
> CustomerFind200Response Invoke-CustomerFind<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FindValue] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FindWhere] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FindParams] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

customer.find

Find customers in store.

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

$FindValue = "mail@gmail.com" # String | Entity search that is specified by some value
$FindWhere = "email" # String | Entity search that is specified by the comma-separated unique fields (optional) (default to "email")
$FindParams = "regex" # String | Entity search that is specified by comma-separated parameters (optional) (default to "whole_words")
$StoreId = "1" # String | Store Id (optional)

# customer.find
try {
    $Result = Invoke-CustomerFind -FindValue $FindValue -FindWhere $FindWhere -FindParams $FindParams -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-CustomerFind: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **FindValue** | **String**| Entity search that is specified by some value | 
 **FindWhere** | **String**| Entity search that is specified by the comma-separated unique fields | [optional] [default to &quot;email&quot;]
 **FindParams** | **String**| Entity search that is specified by comma-separated parameters | [optional] [default to &quot;whole_words&quot;]
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**CustomerFind200Response**](CustomerFind200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CustomerGroupAdd"></a>
# **Invoke-CustomerGroupAdd**
> CustomerGroupAdd200Response Invoke-CustomerGroupAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Name] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoresIds] <String><br>

customer.group.add

Create customer group.

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

$Name = "new_group" # String | Customer group name
$StoreId = "1" # String | Store Id (optional)
$StoresIds = "1,2" # String | Assign customer group to the stores that is specified by comma-separated stores' id (optional)

# customer.group.add
try {
    $Result = Invoke-CustomerGroupAdd -Name $Name -StoreId $StoreId -StoresIds $StoresIds
} catch {
    Write-Host ("Exception occurred when calling Invoke-CustomerGroupAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Name** | **String**| Customer group name | 
 **StoreId** | **String**| Store Id | [optional] 
 **StoresIds** | **String**| Assign customer group to the stores that is specified by comma-separated stores&#39; id | [optional] 

### Return type

[**CustomerGroupAdd200Response**](CustomerGroupAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CustomerGroupList"></a>
# **Invoke-CustomerGroupList**
> ModelResponseCustomerGroupList Invoke-CustomerGroupList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DisableCache] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-GroupIds] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>

customer.group.list

Get list of customers groups.

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

$DisableCache = $false # Boolean | Disable cache for current request (optional) (default to $false)
$PageCursor = "MyPageCursor" # String | Used to retrieve entities via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$Start = 0 # Int32 | This parameter sets the number from which you want to get entities (optional) (default to 0)
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$StoreId = "1" # String | Store Id (optional)
$LangId = "3" # String | Language id (optional)
$GroupIds = "1,2,3" # String | Groups that will be assigned to a customer (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,name,additional_fields")
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)
$ResponseFields = "{return_code,return_message,pagination,result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)

# customer.group.list
try {
    $Result = Invoke-CustomerGroupList -DisableCache $DisableCache -PageCursor $PageCursor -Start $Start -Count $Count -StoreId $StoreId -LangId $LangId -GroupIds $GroupIds -Params $Params -Exclude $Exclude -ResponseFields $ResponseFields
} catch {
    Write-Host ("Exception occurred when calling Invoke-CustomerGroupList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **DisableCache** | **Boolean**| Disable cache for current request | [optional] [default to $false]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **StoreId** | **String**| Store Id | [optional] 
 **LangId** | **String**| Language id | [optional] 
 **GroupIds** | **String**| Groups that will be assigned to a customer | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,name,additional_fields&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 

### Return type

[**ModelResponseCustomerGroupList**](ModelResponseCustomerGroupList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CustomerInfo"></a>
# **Invoke-CustomerInfo**
> CustomerInfo200Response Invoke-CustomerInfo<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

customer.info

Get customers' details from store.

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

$Id = "10" # String | Retrieves customer's info specified by customer id
$Params = "id,email" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,email,first_name,last_name")
$ResponseFields = "{result{id,parent_id,sku,upc,images,combination}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Exclude = "id,email" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)
$StoreId = "1" # String | Retrieves customer info specified by store id (optional)

# customer.info
try {
    $Result = Invoke-CustomerInfo -Id $Id -Params $Params -ResponseFields $ResponseFields -Exclude $Exclude -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-CustomerInfo: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Retrieves customer&#39;s info specified by customer id | 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,email,first_name,last_name&quot;]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 
 **StoreId** | **String**| Retrieves customer info specified by store id | [optional] 

### Return type

[**CustomerInfo200Response**](CustomerInfo200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CustomerList"></a>
# **Invoke-CustomerList**
> ModelResponseCustomerList Invoke-CustomerList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-GroupId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerListId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Avail] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FindValue] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FindWhere] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SortBy] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SortDirection] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Ids] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SinceId] <String><br>

customer.list

Get list of customers from store.

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

$PageCursor = "MyPageCursor" # String | Used to retrieve entities via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$Start = 0 # Int32 | This parameter sets the number from which you want to get entities (optional) (default to 0)
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$CreatedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their creation date (optional)
$CreatedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their creation date (optional)
$ModifiedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their modification date (optional)
$ModifiedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their modification date (optional)
$Params = "id,email" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,email,first_name,last_name")
$ResponseFields = "{result{customer}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Exclude = "id,email" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)
$GroupId = "3" # String | Customer group_id (optional)
$StoreId = "1" # String | Retrieves customers specified by store id (optional)
$CustomerListId = "exampleListId" # String | The numeric ID of the customer list in Demandware. (optional)
$Avail = $false # Boolean | Defines category's visibility status (optional) (default to $true)
$FindValue = "mail@gmail.com" # String | Entity search that is specified by some value (optional)
$FindWhere = "email" # String | Customer search that is specified by field (optional)
$SortBy = "value_id" # String | Set field to sort by (optional) (default to "created_time")
$SortDirection = "asc" # String | Set sorting direction (optional) (default to "asc")
$Ids = "24,25" # String | Retrieves customers specified by ids (optional)
$SinceId = "56" # String | Retrieve entities starting from the specified id. (optional)

# customer.list
try {
    $Result = Invoke-CustomerList -PageCursor $PageCursor -Start $Start -Count $Count -CreatedFrom $CreatedFrom -CreatedTo $CreatedTo -ModifiedFrom $ModifiedFrom -ModifiedTo $ModifiedTo -Params $Params -ResponseFields $ResponseFields -Exclude $Exclude -GroupId $GroupId -StoreId $StoreId -CustomerListId $CustomerListId -Avail $Avail -FindValue $FindValue -FindWhere $FindWhere -SortBy $SortBy -SortDirection $SortDirection -Ids $Ids -SinceId $SinceId
} catch {
    Write-Host ("Exception occurred when calling Invoke-CustomerList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **CreatedFrom** | **String**| Retrieve entities from their creation date | [optional] 
 **CreatedTo** | **String**| Retrieve entities to their creation date | [optional] 
 **ModifiedFrom** | **String**| Retrieve entities from their modification date | [optional] 
 **ModifiedTo** | **String**| Retrieve entities to their modification date | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,email,first_name,last_name&quot;]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 
 **GroupId** | **String**| Customer group_id | [optional] 
 **StoreId** | **String**| Retrieves customers specified by store id | [optional] 
 **CustomerListId** | **String**| The numeric ID of the customer list in Demandware. | [optional] 
 **Avail** | **Boolean**| Defines category&#39;s visibility status | [optional] [default to $true]
 **FindValue** | **String**| Entity search that is specified by some value | [optional] 
 **FindWhere** | **String**| Customer search that is specified by field | [optional] 
 **SortBy** | **String**| Set field to sort by | [optional] [default to &quot;created_time&quot;]
 **SortDirection** | **String**| Set sorting direction | [optional] [default to &quot;asc&quot;]
 **Ids** | **String**| Retrieves customers specified by ids | [optional] 
 **SinceId** | **String**| Retrieve entities starting from the specified id. | [optional] 

### Return type

[**ModelResponseCustomerList**](ModelResponseCustomerList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CustomerUpdate"></a>
# **Invoke-CustomerUpdate**
> AccountConfigUpdate200Response Invoke-CustomerUpdate<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerUpdate] <PSCustomObject><br>

customer.update

Update information of customer in store.

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

$CustomerAddConsentsInner = Initialize-CustomerAddConsentsInner -Type "email" -Status "MyStatus" -OptInLevel "MyOptInLevel"
$CustomerUpdateAddressInner = Initialize-CustomerUpdateAddressInner -AddressBookId "7805807034473" -AddressBookFirstName "John" -AddressBookLastName "Smith" -AddressBookCompany "Samsung" -AddressBookFax "5758787" -AddressBookPhone "5758787" -AddressBookPhoneMobile "5758787" -AddressBookAddress1 "Green str. 35" -AddressBookAddress2 "Green str. 35" -AddressBookCity "Chicago" -AddressBookCountry "US" -AddressBookState "IL" -AddressBookPostcode "12345" -AddressBookTaxId "`12345678`" -AddressBookIdentificationNumber "`123-456-7890`" -AddressBookGender "male" -AddressBookAlias "Address alias" -AddressBookType "billing" -AddressBookDefault $true
$CustomerUpdate = Initialize-CustomerUpdate -Id "10" -GroupId "3" -GroupIds "1,2,3" -Group "Register" -Email "mail@example.com" -Phone "56686868654" -FirstName "John" -LastName "Smith" -BirthDay "2013-02-26 15:00:00" -NewsLetterSubscription $true -Consents $CustomerAddConsentsInner -Tags "tag1,tag2" -Gender "male" -StoreId "1" -Note "Customer note" -Status "disabled" -Address $CustomerUpdateAddressInner # CustomerUpdate | 

# customer.update
try {
    $Result = Invoke-CustomerUpdate -CustomerUpdate $CustomerUpdate
} catch {
    Write-Host ("Exception occurred when calling Invoke-CustomerUpdate: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **CustomerUpdate** | [**CustomerUpdate**](CustomerUpdate.md)|  | 

### Return type

[**AccountConfigUpdate200Response**](AccountConfigUpdate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CustomerWishlistList"></a>
# **Invoke-CustomerWishlistList**
> ModelResponseCustomerWishlistList Invoke-CustomerWishlistList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>

customer.wishlist.list

Get a Wish List of customer from the store.

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
$Id = "10" # String | Entity id (optional)
$StoreId = "1" # String | Store Id (optional)
$Start = 0 # Int32 | This parameter sets the number from which you want to get entities (optional) (default to 0)
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$PageCursor = "MyPageCursor" # String | Used to retrieve entities via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$ResponseFields = "{return_code,return_message,pagination,result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "{return_code,return_message,pagination,result}")

# customer.wishlist.list
try {
    $Result = Invoke-CustomerWishlistList -CustomerId $CustomerId -Id $Id -StoreId $StoreId -Start $Start -Count $Count -PageCursor $PageCursor -ResponseFields $ResponseFields
} catch {
    Write-Host ("Exception occurred when calling Invoke-CustomerWishlistList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **CustomerId** | **String**| Retrieves orders specified by customer id | 
 **Id** | **String**| Entity id | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;{return_code,return_message,pagination,result}&quot;]

### Return type

[**ModelResponseCustomerWishlistList**](ModelResponseCustomerWishlistList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

