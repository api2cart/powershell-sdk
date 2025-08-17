# PSOpenAPITools.PSOpenAPITools\Api.CartApi

All URIs are relative to *https://api.api2cart.local.com/v1.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Invoke-CartCatalogPriceRulesCount**](CartApi.md#Invoke-CartCatalogPriceRulesCount) | **GET** /cart.catalog_price_rules.count.json | cart.catalog_price_rules.count
[**Invoke-CartCatalogPriceRulesList**](CartApi.md#Invoke-CartCatalogPriceRulesList) | **GET** /cart.catalog_price_rules.list.json | cart.catalog_price_rules.list
[**Invoke-CartCouponAdd**](CartApi.md#Invoke-CartCouponAdd) | **POST** /cart.coupon.add.json | cart.coupon.add
[**Invoke-CartCouponConditionAdd**](CartApi.md#Invoke-CartCouponConditionAdd) | **POST** /cart.coupon.condition.add.json | cart.coupon.condition.add
[**Invoke-CartCouponCount**](CartApi.md#Invoke-CartCouponCount) | **GET** /cart.coupon.count.json | cart.coupon.count
[**Invoke-CartCouponDelete**](CartApi.md#Invoke-CartCouponDelete) | **DELETE** /cart.coupon.delete.json | cart.coupon.delete
[**Invoke-CartCouponList**](CartApi.md#Invoke-CartCouponList) | **GET** /cart.coupon.list.json | cart.coupon.list
[**Invoke-CartDelete**](CartApi.md#Invoke-CartDelete) | **DELETE** /cart.delete.json | cart.delete
[**Invoke-CartGiftcardAdd**](CartApi.md#Invoke-CartGiftcardAdd) | **POST** /cart.giftcard.add.json | cart.giftcard.add
[**Invoke-CartGiftcardCount**](CartApi.md#Invoke-CartGiftcardCount) | **GET** /cart.giftcard.count.json | cart.giftcard.count
[**Invoke-CartGiftcardDelete**](CartApi.md#Invoke-CartGiftcardDelete) | **DELETE** /cart.giftcard.delete.json | cart.giftcard.delete
[**Invoke-CartGiftcardList**](CartApi.md#Invoke-CartGiftcardList) | **GET** /cart.giftcard.list.json | cart.giftcard.list
[**Invoke-CartInfo**](CartApi.md#Invoke-CartInfo) | **GET** /cart.info.json | cart.info
[**Invoke-CartMetaDataList**](CartApi.md#Invoke-CartMetaDataList) | **GET** /cart.meta_data.list.json | cart.meta_data.list
[**Invoke-CartMetaDataSet**](CartApi.md#Invoke-CartMetaDataSet) | **POST** /cart.meta_data.set.json | cart.meta_data.set
[**Invoke-CartMetaDataUnset**](CartApi.md#Invoke-CartMetaDataUnset) | **DELETE** /cart.meta_data.unset.json | cart.meta_data.unset
[**Invoke-CartMethods**](CartApi.md#Invoke-CartMethods) | **GET** /cart.methods.json | cart.methods
[**Invoke-CartPluginList**](CartApi.md#Invoke-CartPluginList) | **GET** /cart.plugin.list.json | cart.plugin.list
[**Invoke-CartScriptAdd**](CartApi.md#Invoke-CartScriptAdd) | **POST** /cart.script.add.json | cart.script.add
[**Invoke-CartScriptDelete**](CartApi.md#Invoke-CartScriptDelete) | **DELETE** /cart.script.delete.json | cart.script.delete
[**Invoke-CartScriptList**](CartApi.md#Invoke-CartScriptList) | **GET** /cart.script.list.json | cart.script.list
[**Invoke-CartShippingZonesList**](CartApi.md#Invoke-CartShippingZonesList) | **GET** /cart.shipping_zones.list.json | cart.shipping_zones.list
[**Invoke-CartValidate**](CartApi.md#Invoke-CartValidate) | **GET** /cart.validate.json | cart.validate


<a id="Invoke-CartCatalogPriceRulesCount"></a>
# **Invoke-CartCatalogPriceRulesCount**
> CartCatalogPriceRulesCount200Response Invoke-CartCatalogPriceRulesCount<br>

cart.catalog_price_rules.count

Get count of cart catalog price rules discounts.

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


# cart.catalog_price_rules.count
try {
    $Result = Invoke-CartCatalogPriceRulesCount
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartCatalogPriceRulesCount: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CartCatalogPriceRulesCount200Response**](CartCatalogPriceRulesCount200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartCatalogPriceRulesList"></a>
# **Invoke-CartCatalogPriceRulesList**
> ModelResponseCartCatalogPriceRulesList Invoke-CartCatalogPriceRulesList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Ids] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

cart.catalog_price_rules.list

Get cart catalog price rules discounts.

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
$Ids = "24,25" # String | Retrieves  catalog_price_rules by ids (optional)
$ResponseFields = "{result{catalog_price_rules_count,catalog_price_rules{id,type,name,avail,usage_count,actions,conditions}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,name,description")
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# cart.catalog_price_rules.list
try {
    $Result = Invoke-CartCatalogPriceRulesList -Start $Start -Count $Count -PageCursor $PageCursor -Ids $Ids -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartCatalogPriceRulesList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **Ids** | **String**| Retrieves  catalog_price_rules by ids | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,name,description&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseCartCatalogPriceRulesList**](ModelResponseCartCatalogPriceRulesList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartCouponAdd"></a>
# **Invoke-CartCouponAdd**
> CartCouponAdd200Response Invoke-CartCouponAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CartCouponAdd] <PSCustomObject><br>

cart.coupon.add

Use this method to create a coupon with specified conditions.

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

$CartCouponAdd = Initialize-CartCouponAdd -Code "000_BIG_SALE_000" -ActionType "percent" -ActionApplyTo "order_total" -ActionScope "order" -ActionAmount 15.5 -Codes "MyCodes" -Name "Sale! -30%" -DateStart "2019-12-29 06:44:30" -DateEnd "2020-01-05 01:00:00" -UsageLimit 99 -UsageLimitPerCustomer 1 -ActionConditionEntity "order" -ActionConditionKey "product_id" -ActionConditionOperator "ONE_OF" -ActionConditionValue "17834222,45466663" -IncludeTax $true -StoreId "1" -FreeCashOnDelivery $true -CustomerId "5" # CartCouponAdd | 

# cart.coupon.add
try {
    $Result = Invoke-CartCouponAdd -CartCouponAdd $CartCouponAdd
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartCouponAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **CartCouponAdd** | [**CartCouponAdd**](CartCouponAdd.md)|  | 

### Return type

[**CartCouponAdd200Response**](CartCouponAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartCouponConditionAdd"></a>
# **Invoke-CartCouponConditionAdd**
> BasketLiveShippingServiceDelete200Response Invoke-CartCouponConditionAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CouponId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Entity] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Key] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Operator] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Value] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Target] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-IncludeTax] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-IncludeShipping] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

cart.coupon.condition.add

Use this method to add additional conditions for coupon application.

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

$CouponId = "45845" # String | Coupon Id
$Entity = "order" # String | Defines condition entity type
$Key = "total" # String | Defines condition entity attribute key
$Operator = "==" # String | Defines condition operator
$Value = "2" # String | Defines condition value, can be comma separated according to the operator.
$Target = "coupon_action" # String | Defines condition operator (optional) (default to "coupon_prerequisite")
$IncludeTax = $true # Boolean | Indicates whether to apply a discount for taxes. (optional) (default to $false)
$IncludeShipping = $true # Boolean | Indicates whether to apply a discount for shipping. (optional) (default to $false)
$StoreId = "1" # String | Store Id (optional)

# cart.coupon.condition.add
try {
    $Result = Invoke-CartCouponConditionAdd -CouponId $CouponId -Entity $Entity -Key $Key -Operator $Operator -Value $Value -Target $Target -IncludeTax $IncludeTax -IncludeShipping $IncludeShipping -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartCouponConditionAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **CouponId** | **String**| Coupon Id | 
 **Entity** | **String**| Defines condition entity type | 
 **Key** | **String**| Defines condition entity attribute key | 
 **Operator** | **String**| Defines condition operator | 
 **Value** | **String**| Defines condition value, can be comma separated according to the operator. | 
 **Target** | **String**| Defines condition operator | [optional] [default to &quot;coupon_prerequisite&quot;]
 **IncludeTax** | **Boolean**| Indicates whether to apply a discount for taxes. | [optional] [default to $false]
 **IncludeShipping** | **Boolean**| Indicates whether to apply a discount for shipping. | [optional] [default to $false]
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**BasketLiveShippingServiceDelete200Response**](BasketLiveShippingServiceDelete200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartCouponCount"></a>
# **Invoke-CartCouponCount**
> CartCouponCount200Response Invoke-CartCouponCount<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Avail] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateStartFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateStartTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateEndFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateEndTo] <String><br>

cart.coupon.count

This method allows you to get the number of coupons. On some platforms, you can filter the coupons by the date they were active.

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
$Avail = $false # Boolean | Defines category's visibility status (optional) (default to $true)
$DateStartFrom = "2016-12-29 16:44:30" # String | Filter entity by date_start (greater or equal) (optional)
$DateStartTo = "2016-12-29 16:44:30" # String | Filter entity by date_start (less or equal) (optional)
$DateEndFrom = "2016-12-29 16:44:30" # String | Filter entity by date_end (greater or equal) (optional)
$DateEndTo = "2016-12-29 16:44:30" # String | Filter entity by date_end (less or equal) (optional)

# cart.coupon.count
try {
    $Result = Invoke-CartCouponCount -StoreId $StoreId -Avail $Avail -DateStartFrom $DateStartFrom -DateStartTo $DateStartTo -DateEndFrom $DateEndFrom -DateEndTo $DateEndTo
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartCouponCount: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **StoreId** | **String**| Store Id | [optional] 
 **Avail** | **Boolean**| Defines category&#39;s visibility status | [optional] [default to $true]
 **DateStartFrom** | **String**| Filter entity by date_start (greater or equal) | [optional] 
 **DateStartTo** | **String**| Filter entity by date_start (less or equal) | [optional] 
 **DateEndFrom** | **String**| Filter entity by date_end (greater or equal) | [optional] 
 **DateEndTo** | **String**| Filter entity by date_end (less or equal) | [optional] 

### Return type

[**CartCouponCount200Response**](CartCouponCount200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartCouponDelete"></a>
# **Invoke-CartCouponDelete**
> AttributeDelete200Response Invoke-CartCouponDelete<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

cart.coupon.delete

Delete coupon

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

# cart.coupon.delete
try {
    $Result = Invoke-CartCouponDelete -Id $Id -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartCouponDelete: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
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

<a id="Invoke-CartCouponList"></a>
# **Invoke-CartCouponList**
> ModelResponseCartCouponList Invoke-CartCouponList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CouponsIds] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Avail] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Status] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateStartFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateStartTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateEndFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateEndTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

cart.coupon.list

Get cart coupon discounts.

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
$CouponsIds = "1,2,3" # String | Filter coupons by ids (optional)
$StoreId = "1" # String | Filter coupons by store id (optional)
$LangId = "3" # String | Language id (optional)
$Avail = $false # Boolean | Filter coupons by avail status (optional)
$Status = "disabled" # String | Defines coupon's status (optional)
$DateStartFrom = "2016-12-29 16:44:30" # String | Filter entity by date_start (greater or equal) (optional)
$DateStartTo = "2016-12-29 16:44:30" # String | Filter entity by date_start (less or equal) (optional)
$DateEndFrom = "2016-12-29 16:44:30" # String | Filter entity by date_end (greater or equal) (optional)
$DateEndTo = "2016-12-29 16:44:30" # String | Filter entity by date_end (less or equal) (optional)
$ResponseFields = "{pagination,result{coupon_count,coupon{id,code,name,conditions,actions{scope,amount,conditions{id,value,sub-conditions}},date_start,avail}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,code,type,amount" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,code,name,description")
$Exclude = "usage_history,type" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# cart.coupon.list
try {
    $Result = Invoke-CartCouponList -Start $Start -Count $Count -PageCursor $PageCursor -CouponsIds $CouponsIds -StoreId $StoreId -LangId $LangId -Avail $Avail -Status $Status -DateStartFrom $DateStartFrom -DateStartTo $DateStartTo -DateEndFrom $DateEndFrom -DateEndTo $DateEndTo -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartCouponList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **CouponsIds** | **String**| Filter coupons by ids | [optional] 
 **StoreId** | **String**| Filter coupons by store id | [optional] 
 **LangId** | **String**| Language id | [optional] 
 **Avail** | **Boolean**| Filter coupons by avail status | [optional] 
 **Status** | **String**| Defines coupon&#39;s status | [optional] 
 **DateStartFrom** | **String**| Filter entity by date_start (greater or equal) | [optional] 
 **DateStartTo** | **String**| Filter entity by date_start (less or equal) | [optional] 
 **DateEndFrom** | **String**| Filter entity by date_end (greater or equal) | [optional] 
 **DateEndTo** | **String**| Filter entity by date_end (less or equal) | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,code,name,description&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseCartCouponList**](ModelResponseCartCouponList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartDelete"></a>
# **Invoke-CartDelete**
> CartDelete200Response Invoke-CartDelete<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DeleteBridge] <System.Nullable[Boolean]><br>

cart.delete

Remove store from API2Cart

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

$DeleteBridge = $true # Boolean | Identifies if there is a necessity to delete bridge (optional) (default to $true)

# cart.delete
try {
    $Result = Invoke-CartDelete -DeleteBridge $DeleteBridge
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartDelete: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **DeleteBridge** | **Boolean**| Identifies if there is a necessity to delete bridge | [optional] [default to $true]

### Return type

[**CartDelete200Response**](CartDelete200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartGiftcardAdd"></a>
# **Invoke-CartGiftcardAdd**
> CartGiftcardAdd200Response Invoke-CartGiftcardAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Amount] <Decimal><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Code] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OwnerEmail] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-RecipientEmail] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-RecipientName] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OwnerName] <String><br>

cart.giftcard.add

Use this method to create a gift card for a specified amount.

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

$Amount = 15.5 # Decimal | Defines the gift card amount value.
$Code = "GFT1 A4S5 AA11 RD61" # String | Gift card code (optional)
$OwnerEmail = "jubari@hannsgroup.com" # String | Gift card owner email (optional)
$RecipientEmail = "jubari@hannsgroup.com" # String | Gift card recipient email (optional)
$RecipientName = "John Doe" # String | Gift card recipient name (optional)
$OwnerName = "John Doe" # String | Gift card owner name (optional)

# cart.giftcard.add
try {
    $Result = Invoke-CartGiftcardAdd -Amount $Amount -Code $Code -OwnerEmail $OwnerEmail -RecipientEmail $RecipientEmail -RecipientName $RecipientName -OwnerName $OwnerName
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartGiftcardAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Amount** | **Decimal**| Defines the gift card amount value. | 
 **Code** | **String**| Gift card code | [optional] 
 **OwnerEmail** | **String**| Gift card owner email | [optional] 
 **RecipientEmail** | **String**| Gift card recipient email | [optional] 
 **RecipientName** | **String**| Gift card recipient name | [optional] 
 **OwnerName** | **String**| Gift card owner name | [optional] 

### Return type

[**CartGiftcardAdd200Response**](CartGiftcardAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartGiftcardCount"></a>
# **Invoke-CartGiftcardCount**
> CartGiftcardCount200Response Invoke-CartGiftcardCount<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

cart.giftcard.count

Get gift cards count.

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

# cart.giftcard.count
try {
    $Result = Invoke-CartGiftcardCount -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartGiftcardCount: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**CartGiftcardCount200Response**](CartGiftcardCount200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartGiftcardDelete"></a>
# **Invoke-CartGiftcardDelete**
> AttributeDelete200Response Invoke-CartGiftcardDelete<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>

cart.giftcard.delete

Delete giftcard

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

# cart.giftcard.delete
try {
    $Result = Invoke-CartGiftcardDelete -Id $Id
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartGiftcardDelete: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Entity id | 

### Return type

[**AttributeDelete200Response**](AttributeDelete200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartGiftcardList"></a>
# **Invoke-CartGiftcardList**
> ModelResponseCartGiftCardList Invoke-CartGiftcardList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

cart.giftcard.list

Get gift cards list.

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
$StoreId = "1" # String | Store Id (optional)
$ResponseFields = "{pagination,result{gift_card{id,code,amount,status}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,code,name")
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# cart.giftcard.list
try {
    $Result = Invoke-CartGiftcardList -Start $Start -Count $Count -PageCursor $PageCursor -StoreId $StoreId -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartGiftcardList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,code,name&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseCartGiftCardList**](ModelResponseCartGiftCardList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartInfo"></a>
# **Invoke-CartInfo**
> CartInfo200Response Invoke-CartInfo<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

cart.info

This method allows you to get various information about the store, including a list of stores (in the case of a multistore configuration), a list of supported languages, currencies, carriers, warehouses, and many other information. This information contains data that is relatively stable and rarely changes, so API2Cart can cache certain data to reduce the load on the store and speed up the execution of the request. We also recommend that you cache the response of this method on your side to save requests. If you need to clear the cache for a specific store, then use the cart.validate method.

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
$ResponseFields = "{result{name,url,stores_info{store_id,name,currency{id,iso3},store_owner_info}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "name,url" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "store_name,store_url,db_prefix")
$Exclude = "name,url" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# cart.info
try {
    $Result = Invoke-CartInfo -StoreId $StoreId -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartInfo: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **StoreId** | **String**| Store Id | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;store_name,store_url,db_prefix&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**CartInfo200Response**](CartInfo200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartMetaDataList"></a>
# **Invoke-CartMetaDataList**
> ModelResponseCartMetaDataList Invoke-CartMetaDataList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EntityId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Entity] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Key] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

cart.meta_data.list

Using this method, you can get a list of metadata for various entities (products, options, customers, orders). Usually this is data created by third-party plugins.

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

$EntityId = "1" # String | Entity Id
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$PageCursor = "MyPageCursor" # String | Used to retrieve entities via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$Entity = "order" # String | Entity (optional) (default to "product")
$StoreId = "1" # String | Store Id (optional)
$LangId = "3" # String | Language id (optional)
$Key = "subtotal" # String | Key (optional)
$ResponseFields = "{result{items{key,value}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "key,value")
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# cart.meta_data.list
try {
    $Result = Invoke-CartMetaDataList -EntityId $EntityId -Count $Count -PageCursor $PageCursor -Entity $Entity -StoreId $StoreId -LangId $LangId -Key $Key -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartMetaDataList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **EntityId** | **String**| Entity Id | 
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **Entity** | **String**| Entity | [optional] [default to &quot;product&quot;]
 **StoreId** | **String**| Store Id | [optional] 
 **LangId** | **String**| Language id | [optional] 
 **Key** | **String**| Key | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;key,value&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseCartMetaDataList**](ModelResponseCartMetaDataList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartMetaDataSet"></a>
# **Invoke-CartMetaDataSet**
> AttributeAdd200Response Invoke-CartMetaDataSet<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EntityId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Key] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Value] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Namespace] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Entity] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>

cart.meta_data.set

Set meta data for a specific entity

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

$EntityId = "1" # String | Entity Id
$Key = "subtotal" # String | Key
$Value = "2" # String | Value
$Namespace = "order" # String | Metafield namespace
$Entity = "order" # String | Entity (optional) (default to "product")
$StoreId = "1" # String | Store Id (optional)
$LangId = "3" # String | Language id (optional)

# cart.meta_data.set
try {
    $Result = Invoke-CartMetaDataSet -EntityId $EntityId -Key $Key -Value $Value -Namespace $Namespace -Entity $Entity -StoreId $StoreId -LangId $LangId
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartMetaDataSet: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **EntityId** | **String**| Entity Id | 
 **Key** | **String**| Key | 
 **Value** | **String**| Value | 
 **Namespace** | **String**| Metafield namespace | 
 **Entity** | **String**| Entity | [optional] [default to &quot;product&quot;]
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

<a id="Invoke-CartMetaDataUnset"></a>
# **Invoke-CartMetaDataUnset**
> BasketLiveShippingServiceDelete200Response Invoke-CartMetaDataUnset<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EntityId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Key] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Entity] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

cart.meta_data.unset

Unset meta data for a specific entity

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

$EntityId = "1" # String | Entity Id
$Key = "subtotal" # String | Key
$Id = "10" # String | Entity id
$Entity = "order" # String | Entity (optional) (default to "product")
$StoreId = "1" # String | Store Id (optional)

# cart.meta_data.unset
try {
    $Result = Invoke-CartMetaDataUnset -EntityId $EntityId -Key $Key -Id $Id -Entity $Entity -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartMetaDataUnset: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **EntityId** | **String**| Entity Id | 
 **Key** | **String**| Key | 
 **Id** | **String**| Entity id | 
 **Entity** | **String**| Entity | [optional] [default to &quot;product&quot;]
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**BasketLiveShippingServiceDelete200Response**](BasketLiveShippingServiceDelete200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartMethods"></a>
# **Invoke-CartMethods**
> CartMethods200Response Invoke-CartMethods<br>

cart.methods

Returns a list of supported API methods.

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


# cart.methods
try {
    $Result = Invoke-CartMethods
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartMethods: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CartMethods200Response**](CartMethods200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartPluginList"></a>
# **Invoke-CartPluginList**
> CartPluginList200Response Invoke-CartPluginList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

cart.plugin.list

Get a list of third-party plugins installed on the store.

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

# cart.plugin.list
try {
    $Result = Invoke-CartPluginList -Start $Start -Count $Count -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartPluginList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
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

[**CartPluginList200Response**](CartPluginList200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartScriptAdd"></a>
# **Invoke-CartScriptAdd**
> CartScriptAdd200Response Invoke-CartScriptAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Name] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Description] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Html] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Src] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LoadMethod] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Scope] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Events] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

cart.script.add

Add new script to the storefront

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

$Name = "jQuery Minimized" # String | The user-friendly script name (optional)
$Description = "The Write Less, Do More, JavaScript Library" # String | The user-friendly description (optional)
$Html = "&#x3C;script&#x3E;alert(&#x27;foo&#x27;)&#x3C;/script&#x3E;" # String | An html string containing exactly one `script` tag. (optional)
$Src = "https://js-aplenty.com/foo.js" # String | The URL of the remote script (optional)
$LoadMethod = "async" # String | The load method to use for the script (optional)
$Scope = "all" # String | The page or pages on the online store where the script should be included (optional) (default to "storefront")
$Events = "purchase_event" # String | Event for run scripts (optional)
$StoreId = "1" # String | Store Id (optional)

# cart.script.add
try {
    $Result = Invoke-CartScriptAdd -Name $Name -Description $Description -Html $Html -Src $Src -LoadMethod $LoadMethod -Scope $Scope -Events $Events -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartScriptAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Name** | **String**| The user-friendly script name | [optional] 
 **Description** | **String**| The user-friendly description | [optional] 
 **Html** | **String**| An html string containing exactly one &#x60;script&#x60; tag. | [optional] 
 **Src** | **String**| The URL of the remote script | [optional] 
 **LoadMethod** | **String**| The load method to use for the script | [optional] 
 **Scope** | **String**| The page or pages on the online store where the script should be included | [optional] [default to &quot;storefront&quot;]
 **Events** | **String**| Event for run scripts | [optional] 
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**CartScriptAdd200Response**](CartScriptAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartScriptDelete"></a>
# **Invoke-CartScriptDelete**
> AttributeDelete200Response Invoke-CartScriptDelete<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

cart.script.delete

Remove script from the storefront

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

# cart.script.delete
try {
    $Result = Invoke-CartScriptDelete -Id $Id -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartScriptDelete: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
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

<a id="Invoke-CartScriptList"></a>
# **Invoke-CartScriptList**
> ModelResponseCartScriptList Invoke-CartScriptList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ScriptIds] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

cart.script.list

Get scripts installed to the storefront

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
$ScriptIds = "34023324,34024032" # String | Retrieves only scripts with specific ids (optional)
$StoreId = "1" # String | Store Id (optional)
$CreatedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their creation date (optional)
$CreatedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their creation date (optional)
$ModifiedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their modification date (optional)
$ModifiedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their modification date (optional)
$ResponseFields = "{pagination,result{total_count,scripts{id,name,src,created_time{value}}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,name,description")
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# cart.script.list
try {
    $Result = Invoke-CartScriptList -Start $Start -Count $Count -PageCursor $PageCursor -ScriptIds $ScriptIds -StoreId $StoreId -CreatedFrom $CreatedFrom -CreatedTo $CreatedTo -ModifiedFrom $ModifiedFrom -ModifiedTo $ModifiedTo -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartScriptList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **ScriptIds** | **String**| Retrieves only scripts with specific ids | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **CreatedFrom** | **String**| Retrieve entities from their creation date | [optional] 
 **CreatedTo** | **String**| Retrieve entities to their creation date | [optional] 
 **ModifiedFrom** | **String**| Retrieve entities from their modification date | [optional] 
 **ModifiedTo** | **String**| Retrieve entities to their modification date | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,name,description&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseCartScriptList**](ModelResponseCartScriptList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartShippingZonesList"></a>
# **Invoke-CartShippingZonesList**
> ModelResponseCartShippingZonesList Invoke-CartShippingZonesList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

cart.shipping_zones.list

Get list of shipping zones

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
$ResponseFields = "{result{id,name,enabled,countries,shipping_methods{name,rates}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,name,enabled")
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# cart.shipping_zones.list
try {
    $Result = Invoke-CartShippingZonesList -Start $Start -Count $Count -StoreId $StoreId -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartShippingZonesList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **StoreId** | **String**| Store Id | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,name,enabled&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseCartShippingZonesList**](ModelResponseCartShippingZonesList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartValidate"></a>
# **Invoke-CartValidate**
> CartValidate200Response Invoke-CartValidate<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ValidateVersion] <System.Nullable[Boolean]><br>

cart.validate

This method clears the cache in API2Cart for a particular store and checks whether the connection to the store is available. Use this method if there have been any changes in the settings on the storе, for example, if a new plugin has been installed or removed.

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

$ValidateVersion = $true # Boolean | Specify if api2cart should validate cart version (optional) (default to $false)

# cart.validate
try {
    $Result = Invoke-CartValidate -ValidateVersion $ValidateVersion
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartValidate: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ValidateVersion** | **Boolean**| Specify if api2cart should validate cart version | [optional] [default to $false]

### Return type

[**CartValidate200Response**](CartValidate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

