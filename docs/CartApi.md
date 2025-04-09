# PSOpenAPITools.PSOpenAPITools\Api.CartApi

All URIs are relative to *https://api.api2cart.com/v1.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Invoke-CartBridge**](CartApi.md#Invoke-CartBridge) | **GET** /cart.bridge.json | cart.bridge
[**Invoke-CartCatalogPriceRulesCount**](CartApi.md#Invoke-CartCatalogPriceRulesCount) | **GET** /cart.catalog_price_rules.count.json | cart.catalog_price_rules.count
[**Invoke-CartCatalogPriceRulesList**](CartApi.md#Invoke-CartCatalogPriceRulesList) | **GET** /cart.catalog_price_rules.list.json | cart.catalog_price_rules.list
[**Invoke-CartClearCache**](CartApi.md#Invoke-CartClearCache) | **POST** /cart.clear_cache.json | cart.clear_cache
[**Invoke-CartConfig**](CartApi.md#Invoke-CartConfig) | **GET** /cart.config.json | cart.config
[**Invoke-CartConfigUpdate**](CartApi.md#Invoke-CartConfigUpdate) | **PUT** /cart.config.update.json | cart.config.update
[**Invoke-CartCouponAdd**](CartApi.md#Invoke-CartCouponAdd) | **POST** /cart.coupon.add.json | cart.coupon.add
[**Invoke-CartCouponConditionAdd**](CartApi.md#Invoke-CartCouponConditionAdd) | **POST** /cart.coupon.condition.add.json | cart.coupon.condition.add
[**Invoke-CartCouponCount**](CartApi.md#Invoke-CartCouponCount) | **GET** /cart.coupon.count.json | cart.coupon.count
[**Invoke-CartCouponDelete**](CartApi.md#Invoke-CartCouponDelete) | **DELETE** /cart.coupon.delete.json | cart.coupon.delete
[**Invoke-CartCouponList**](CartApi.md#Invoke-CartCouponList) | **GET** /cart.coupon.list.json | cart.coupon.list
[**Invoke-CartCreate**](CartApi.md#Invoke-CartCreate) | **POST** /cart.create.json | cart.create
[**Invoke-CartDelete**](CartApi.md#Invoke-CartDelete) | **DELETE** /cart.delete.json | cart.delete
[**Invoke-CartDisconnect**](CartApi.md#Invoke-CartDisconnect) | **GET** /cart.disconnect.json | cart.disconnect
[**Invoke-CartGiftcardAdd**](CartApi.md#Invoke-CartGiftcardAdd) | **POST** /cart.giftcard.add.json | cart.giftcard.add
[**Invoke-CartGiftcardCount**](CartApi.md#Invoke-CartGiftcardCount) | **GET** /cart.giftcard.count.json | cart.giftcard.count
[**Invoke-CartGiftcardDelete**](CartApi.md#Invoke-CartGiftcardDelete) | **DELETE** /cart.giftcard.delete.json | cart.giftcard.delete
[**Invoke-CartGiftcardList**](CartApi.md#Invoke-CartGiftcardList) | **GET** /cart.giftcard.list.json | cart.giftcard.list
[**Invoke-CartInfo**](CartApi.md#Invoke-CartInfo) | **GET** /cart.info.json | cart.info
[**Invoke-CartList**](CartApi.md#Invoke-CartList) | **GET** /cart.list.json | cart.list
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


<a id="Invoke-CartBridge"></a>
# **Invoke-CartBridge**
> CartBridge200Response Invoke-CartBridge<br>

cart.bridge

Get bridge key and store key

### Example
```powershell
# general setting of the PowerShell module, e.g. base URL, authentication, etc
$Configuration = Get-Configuration
# Configure API key authorization: ApiKeyAuth
$Configuration.ApiKey.x-api-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-api-key = "Bearer"


# cart.bridge
try {
    $Result = Invoke-CartBridge
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartBridge: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CartBridge200Response**](CartBridge200Response.md) (PSCustomObject)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

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
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Ids] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
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

$PageCursor = "MyPageCursor" # String | Used to retrieve entities via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$Start = 0 # Int32 | This parameter sets the number from which you want to get entities (optional) (default to 0)
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$Ids = "24,25" # String | Retrieves  catalog_price_rules by ids (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,name,description")
$ResponseFields = "{result{catalog_price_rules_count,catalog_price_rules{id,type,name,avail,usage_count,actions,conditions}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# cart.catalog_price_rules.list
try {
    $Result = Invoke-CartCatalogPriceRulesList -PageCursor $PageCursor -Start $Start -Count $Count -Ids $Ids -Params $Params -ResponseFields $ResponseFields -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartCatalogPriceRulesList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **Ids** | **String**| Retrieves  catalog_price_rules by ids | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,name,description&quot;]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseCartCatalogPriceRulesList**](ModelResponseCartCatalogPriceRulesList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartClearCache"></a>
# **Invoke-CartClearCache**
> CartClearCache200Response Invoke-CartClearCache<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CacheType] <String><br>

cart.clear_cache

Clear cache on store.

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

$CacheType = "storage_cache" # String | Defines which cache should be cleared.

# cart.clear_cache
try {
    $Result = Invoke-CartClearCache -CacheType $CacheType
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartClearCache: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **CacheType** | **String**| Defines which cache should be cleared. | 

### Return type

[**CartClearCache200Response**](CartClearCache200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartConfig"></a>
# **Invoke-CartConfig**
> CartConfig200Response Invoke-CartConfig<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

cart.config

Get list of cart configs

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

$Params = "store_name,store_url,db_prefix" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "store_name,store_url,db_prefix")
$Exclude = "store_name,store_url,db_prefix" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# cart.config
try {
    $Result = Invoke-CartConfig -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartConfig: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;store_name,store_url,db_prefix&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**CartConfig200Response**](CartConfig200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartConfigUpdate"></a>
# **Invoke-CartConfigUpdate**
> CartConfigUpdate200Response Invoke-CartConfigUpdate<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CartConfigUpdate] <PSCustomObject><br>

cart.config.update

Use this API method to update custom data in client database.

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

$CartConfigUpdate = Initialize-CartConfigUpdate -DbTablesPrefix "oc_" -CustomFields  -StoreId "1" -UserAgent "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:47.0) Gecko/20100101 Firefox/47.0" # CartConfigUpdate | 

# cart.config.update
try {
    $Result = Invoke-CartConfigUpdate -CartConfigUpdate $CartConfigUpdate
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartConfigUpdate: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **CartConfigUpdate** | [**CartConfigUpdate**](CartConfigUpdate.md)|  | 

### Return type

[**CartConfigUpdate200Response**](CartConfigUpdate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
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

$CartCouponAdd = Initialize-CartCouponAdd -StoreId "1" -Code "000_BIG_SALE_000" -Name "Sale! -30%" -Codes "MyCodes" -ActionType "percent" -ActionApplyTo "order_total" -ActionScope "order" -ActionAmount 15.5 -DateStart "2019-12-29 06:44:30" -DateEnd "2020-01-05 01:00:00" -UsageLimit 99 -UsageLimitPerCustomer 1 -ActionConditionEntity "order" -ActionConditionKey "product_id" -ActionConditionOperator "ONE_OF" -ActionConditionValue "17834222,45466663" -IncludeTax $true # CartCouponAdd | 

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
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Target] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-IncludeTax] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-IncludeShipping] <System.Nullable[Boolean]><br>

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
$StoreId = "1" # String | Store Id (optional)
$Target = "coupon_action" # String | Defines condition operator (optional) (default to "coupon_prerequisite")
$IncludeTax = $true # Boolean | Indicates whether to apply a discount for taxes. (optional) (default to $false)
$IncludeShipping = $true # Boolean | Indicates whether to apply a discount for shipping. (optional) (default to $false)

# cart.coupon.condition.add
try {
    $Result = Invoke-CartCouponConditionAdd -CouponId $CouponId -Entity $Entity -Key $Key -Operator $Operator -Value $Value -StoreId $StoreId -Target $Target -IncludeTax $IncludeTax -IncludeShipping $IncludeShipping
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
 **StoreId** | **String**| Store Id | [optional] 
 **Target** | **String**| Defines condition operator | [optional] [default to &quot;coupon_prerequisite&quot;]
 **IncludeTax** | **Boolean**| Indicates whether to apply a discount for taxes. | [optional] [default to $false]
 **IncludeShipping** | **Boolean**| Indicates whether to apply a discount for shipping. | [optional] [default to $false]

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
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateStartFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateStartTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateEndFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateEndTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Avail] <System.Nullable[Boolean]><br>

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
$DateStartFrom = "2016-12-29 16:44:30" # String | Filter entity by date_start (greater or equal) (optional)
$DateStartTo = "2016-12-29 16:44:30" # String | Filter entity by date_start (less or equal) (optional)
$DateEndFrom = "2016-12-29 16:44:30" # String | Filter entity by date_end (greater or equal) (optional)
$DateEndTo = "2016-12-29 16:44:30" # String | Filter entity by date_end (less or equal) (optional)
$Avail = $false # Boolean | Defines category's visibility status (optional) (default to $true)

# cart.coupon.count
try {
    $Result = Invoke-CartCouponCount -StoreId $StoreId -DateStartFrom $DateStartFrom -DateStartTo $DateStartTo -DateEndFrom $DateEndFrom -DateEndTo $DateEndTo -Avail $Avail
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartCouponCount: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **StoreId** | **String**| Store Id | [optional] 
 **DateStartFrom** | **String**| Filter entity by date_start (greater or equal) | [optional] 
 **DateStartTo** | **String**| Filter entity by date_start (less or equal) | [optional] 
 **DateEndFrom** | **String**| Filter entity by date_end (greater or equal) | [optional] 
 **DateEndTo** | **String**| Filter entity by date_end (less or equal) | [optional] 
 **Avail** | **Boolean**| Defines category&#39;s visibility status | [optional] [default to $true]

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
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CouponsIds] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateStartFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateStartTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateEndFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateEndTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Avail] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
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

$PageCursor = "MyPageCursor" # String | Used to retrieve entities via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$Start = 0 # Int32 | This parameter sets the number from which you want to get entities (optional) (default to 0)
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$CouponsIds = "1,2,3" # String | Filter coupons by ids (optional)
$StoreId = "1" # String | Filter coupons by store id (optional)
$DateStartFrom = "2016-12-29 16:44:30" # String | Filter entity by date_start (greater or equal) (optional)
$DateStartTo = "2016-12-29 16:44:30" # String | Filter entity by date_start (less or equal) (optional)
$DateEndFrom = "2016-12-29 16:44:30" # String | Filter entity by date_end (greater or equal) (optional)
$DateEndTo = "2016-12-29 16:44:30" # String | Filter entity by date_end (less or equal) (optional)
$Avail = $false # Boolean | Filter coupons by avail status (optional)
$LangId = "3" # String | Language id (optional)
$Params = "id,code,type,amount" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,code,name,description")
$ResponseFields = "{pagination,result{coupon_count,coupon{id,code,name,conditions,actions{scope,amount,conditions{id,value,sub-conditions}},date_start,avail}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Exclude = "usage_history,type" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# cart.coupon.list
try {
    $Result = Invoke-CartCouponList -PageCursor $PageCursor -Start $Start -Count $Count -CouponsIds $CouponsIds -StoreId $StoreId -DateStartFrom $DateStartFrom -DateStartTo $DateStartTo -DateEndFrom $DateEndFrom -DateEndTo $DateEndTo -Avail $Avail -LangId $LangId -Params $Params -ResponseFields $ResponseFields -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartCouponList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **CouponsIds** | **String**| Filter coupons by ids | [optional] 
 **StoreId** | **String**| Filter coupons by store id | [optional] 
 **DateStartFrom** | **String**| Filter entity by date_start (greater or equal) | [optional] 
 **DateStartTo** | **String**| Filter entity by date_start (less or equal) | [optional] 
 **DateEndFrom** | **String**| Filter entity by date_end (greater or equal) | [optional] 
 **DateEndTo** | **String**| Filter entity by date_end (less or equal) | [optional] 
 **Avail** | **Boolean**| Filter coupons by avail status | [optional] 
 **LangId** | **String**| Language id | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,code,name,description&quot;]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseCartCouponList**](ModelResponseCartCouponList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartCreate"></a>
# **Invoke-CartCreate**
> AccountCartAdd200Response Invoke-CartCreate<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CartCreate] <PSCustomObject><br>

cart.create

Add store to the account

### Example
```powershell
# general setting of the PowerShell module, e.g. base URL, authentication, etc
$Configuration = Get-Configuration
# Configure API key authorization: ApiKeyAuth
$Configuration.ApiKey.x-api-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-api-key = "Bearer"

$AccountCartAddHybrisWebsitesInner = Initialize-AccountCartAddHybrisWebsitesInner -Uid "MyUid" -Url "MyUrl" -StoreIds "MyStoreIds"
$CartCreate = Initialize-CartCreate -CartId "3DCart" -StoreUrl "http://mystore.com" -BridgeUrl "https://your-store.com/custom/bridge/path/bridge.php" -StoreRoot "/home/www/stores/magento1922" -StoreKey "ab37fc230bc5df63a5be1b11220949be" -SharedSecret "gmz3iz45x2" -ValidateVersion $true -Verify $false -DbTablesPrefix "oc_" -UserAgent "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:47.0) Gecko/20100101 Firefox/47.0" -FtpHost "ftp.mystore.com" -FtpUser "user" -FtpPassword "G4}q215D4_H9$Be" -FtpPort 22 -FtpStoreDir "/public" -ApiKey3dcart "82cc921c6a5c67082cc921c6a5c6707e1d6e6862ba3201a" -AdminAccount "admin" -ApiPath "http://mystore.bigcommerce.com/api/v1" -ApiKeyBigcommerce "6b89704cd75738cb0f9f6468d5462aba" -ClientId "p1r37bt131z86675nofv9xmhietoe4t" -AccessToken "igse8e4rdmzkxdi937qe69d59en1imw" -Context "stores/etplnf8o8v" -AccessToken "igse8e4rdmzkxdi937qe69d59en1imw" -ApiKeyShopify "bbca57d8ff3c3677128112c15556d9e3" -ApiPassword "860f3a6fc87632301a42cd88e4b5ab3d" -AccessTokenShopify "igse8e4rdmzkxdi937qe69d59en1imw" -ApiKey "bbca57d8ff3c3677128112c15556d9e3" -ApiUsername "mylogin" -EncryptedPassword "7943CA5F3990E00D9A4CCF0BD998211F" -Login "admin" -ApiUserAdnsf "admin" -ApiPass "f6471ef78f72b41849a8b8b67791b0b5" -PrivateKey "2xo0m9ib5ty7rv84num9uic3e9mio0cy73nsdey7e5270" -AppToken "82cc921c6a5c67082cc921c6a5c6707e1d6e6862ba3201a" -EtsyKeystring "a9psel85v1wy5faeyjw03y0r" -EtsySharedSecret "gmz3iz45x2" -TokenSecret "igse8e4rdmzkxdi937qe69d59en1imw" -EtsyClientId "w0fi0igk2w29bjcd7ydr2s35" -EtsyRefreshToken "223577551.L07_RE-y7unmKf2dox4djsHkVxwpUfs1ikG_uQmHhF-aASEReNn_Qns1Wqn3dDa0ZMxrt9CIael3dgudeDZb31ZUdS" -EbayClientId "a9psel85v1wy5faeyjw03y0r" -EbayClientSecret "gmz3iz45x2" -EbayRuname "gmz3iz45x2" -EbayAccessToken "v^1.1#i ... AjRV4yNjA=" -EbayRefreshToken "v^1.1#i ... rAewqVasdA=" -EbayEnvironment "sandbox" -EbaySiteId 101 -DwClientId "b849eb85-v8b9-1dw8-9fe2-97e1d6ffc7b0" -DwApiPass "testpassword" -DemandwareUserName "admin" -DemandwareUserPassword "12345" -StoreId "1" -SellerId "A9PSDFGFGHFOQD" -Environment "sandbox" -HybrisClientId "api_client_1" -HybrisClientSecret "secret_phrase_1" -HybrisUsername "admin" -HybrisPassword "nimda" -HybrisWebsites $AccountCartAddHybrisWebsitesInner -WalmartClientId "423f6A24-123z-8654-989u-6fa96478289" -WalmartClientSecret "1gf85fea-8974-2648-w12w-rt54284tdf54" -WalmartEnvironment "production" -WalmartChannelType "0f3e4dd4-0514-4346-b39d-af0e00ea066d" -WalmartRegion "us" -LightspeedApiKey "cf5444729c2abd6b6a5d983691767cb5" -LightspeedApiSecret "2620ee52a8bc942f9d5d3a575f4d363e" -ShoplazzaAccessToken "igse8e4rdmzkxdi937qe69d59en1imw" -ShoplazzaSharedSecret "gmz3iz45x2" -ShopwareAccessKey "SWSCS3O1RJBSRNBYQLFIYJN2ZQ" -ShopwareApiKey "SWSCS3O1RJBSRNBYQLFIYJN2ZQ" -ShopwareApiSecret "V3NYNWg2b1dZdHBUWDN1cmdKdGhnenp5enVJYlJ0WlJvOFF2bnQ" -CommercehqApiKey "sJrD-LM0eddhe63rfgfva0dDydXfre4" -CommercehqApiPassword "4Grr_ZCLNNoSUuhAjesKuchxo9SL" -Var3dcartPrivateKey "7dba81f90bdbe25e7000e73214ca51b" -Var3dcartAccessToken "4Grr_ZCLNNoSUuhAjesKuchxo9SL" -WcConsumerKey "ck_26d8e2ad604f3917e429df6961722282bdcf109d" -WcConsumerSecret "cs_931ced666118a15c5f7b4a33a15gf5589cbeba55" -MagentoConsumerKey "ktv4n9rgrj0evjuy2t6p2xlb1f8u5pmy" -MagentoConsumerSecret "a46abc3kxyinlbggy06i9g975xqo6gjq" -MagentoAccessToken "igse8e4rdmzkxdi937qe69d59en1imw" -MagentoTokenSecret "igse8e4rdmzkxdi937qe69d59en1imw" -PrestashopWebserviceKey "CKJ1ZEWRJWRLTPVBQJ9FGGRORD4AGS96" -WixAppId "6b0b5b7b-7d87-45b5-bf34-ac6b438e63da" -WixAppSecretKey "316c0a09-f195-42be-74f6-a02cebb9cae6" -WixInstanceId "58b893a4-6b16-5c2f-qt78-qa3r61t32rt8" -WixRefreshToken "
        OAUTH2.eyJraWQiOiJkZ0x3cjNRMCIsImFsZyI6IkhTMjU2In0.
        eyJkYXRhIjoie1wiaWRcIjpcImJlZjM3MmRmLTUyNGItNDI3NS05M2RkL
        Tg4NDBlOTU3ZWU2OFwifSIsImlhdCI6MTY0ODA0NTEyNiwiZXhwIjoxNzExMTE3MTI2fQ.
        VRR2lGSbcTVmaArtmyyhy6o4WRDwTn-nlDCQpZ97eYw
      " -MercadoLibreAppId "211188015100135" -MercadoLibreAppSecretKey "e2qoG2zklLlfP7cEngEJ94YjhkejkjAm" -MercadoLibreRefreshToken "TG-63h13529vb5464110188d2x9-703754376" -ZidClientId 1234 -ZidClientSecret "nl5l1lE0vxgv6cV111fHsdlOOIfb0Ms5IR7l4Igs" -ZidAccessToken "def50eyfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe657e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65de64a0c865d" -ZidAuthorization "def50eyfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe657e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65de64a0c865d" -ZidRefreshToken "def50eyfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe657e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65d7e64a0cfe9fe65de64a0c865d" -FlipkartClientId "19414773883a13a850b6a52350b7246499a24" -FlipkartClientSecret "nl5l1lE0vxgv6cV111fHsdlOOIfb0Ms5IR7l4Igs" -AllegroClientId "2915e189ce3d23d23d2327d204ae6a0bd" -AllegroClientSecret "DNHtqdL2WPIefeUhQWYgtXPS23fgbfgasdsGHHJGhg3RTFDQWFGZmVoFRT5IfkQj1E7eR5" -AllegroAccessToken "eyJhbGciOiJSUzI1NiIsInR5cCI6IsfddfdfdeyJ1c2VyX25hbWUiOiI5NDUxMzE1MSIsInNjb3BlIjpbImFsbGVncm86YXBpOm9yZGVyczpyZWFkIiwiYWxsZWdybzphcGk6cHJvZmlsZTp3cml0ZSIsImFsbGVncm86YXBpOnNhbGU6b2ZmZXJzOndyaXRlIiwiYWxsZWdybzphcGk6YmlsbGluZzpyZWFkIiwiYWxsZWdybzphcGk6Y2FtcGFpZ25zIiwiYWxsZWdybzphcGk6ZGlzcHV0ZXMiLCJhbGxlZ3JvOmFwaTpzYWxlOm9mZmVyczpyZWFkIiwiYWxsZWdybzphcGk6YmlkcyIsImFsbGVncm86YXBpOm9yZGVyczp3cml0ZSIsImFsbGVncm86YXBpOnBheW1lbnRzOndyaXRlIiwiYWxsZWdybzphcGk6c2FsZTpzZXR0aW5nczp3cml0ZSIsImFsbGVncm86YXBpOnByb2ZpbGU6cmVhZCIsImFsbGVncm86YXBpOnJhdGluZ3MiLCJhbGxlZ3JvOmFwaTpzYWxlOnNldHRpbmdzOnJlYWQiLCJhbGxlZ3JvOmFwaTpwYXltZW50czpyZWFkIiwiYWxsZWdybzphcGk6bWVzc2FnaW5nIl0sI" -AllegroRefreshToken "eyJhbGciOiJSUzI1NiIsInR5cCI6IsfddfdfdeyJ1c2VyX25hbWUiOiI5NDUxMzE1MSIsInNjb3BlIjpbImFsbGVncm86YXBpOm9yZGVyczpyZWFkIiwiYWxsZWdybzphcGk6cHJvZmlsZTp3cml0ZSIsImFsbGVncm86YXBpOnNhbGU6b2ZmZXJzOndyaXRlIiwiYWxsZWdybzphcGk6YmlsbGluZzpyZWFkIiwiYWxsZWdybzphcGk6Y2FtcGFpZ25zIiwiYWxsZWdybzphcGk6ZGlzcHV0ZXMiLCJhbGxlZ3JvOmFwaTpzYWxlOm9mZmVyczpyZWFkIiwiYWxsZWdybzphcGk6YmlkcyIsImFsbGVncm86YXBpOm9yZGVyczp3cml0ZSIsImFsbGVncm86YXBpOnBheW1lbnRzOndyaXRlIiwiYWxsZWdybzphcGk6c2FsZTpzZXR0aW5nczp3cml0ZSIsImFsbGVncm86YXBpOnByb2ZpbGU6cmVhZCIsImFsbGVncm86YXBpOnJhdGluZ3MiLCJhbGxlZ3JvOmFwaTpzYWxlOnNldHRpbmdzOnJlYWQiLCJhbGxlZ3JvOmFwaTpwYXltZW50czpyZWFkIiwiYWxsZWdybzphcGk6bWVzc2FnaW5nIl0sI" -AllegroEnvironment "sandbox" # CartCreate | 

# cart.create
try {
    $Result = Invoke-CartCreate -CartCreate $CartCreate
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartCreate: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **CartCreate** | [**CartCreate**](CartCreate.md)|  | 

### Return type

[**AccountCartAdd200Response**](AccountCartAdd200Response.md) (PSCustomObject)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
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

<a id="Invoke-CartDisconnect"></a>
# **Invoke-CartDisconnect**
> CartDisconnect200Response Invoke-CartDisconnect<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DeleteBridge] <System.Nullable[Boolean]><br>

cart.disconnect

Disconnect with the store and clear store session data.

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

$DeleteBridge = $true # Boolean | Identifies if there is a necessity to delete bridge (optional) (default to $false)

# cart.disconnect
try {
    $Result = Invoke-CartDisconnect -DeleteBridge $DeleteBridge
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartDisconnect: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **DeleteBridge** | **Boolean**| Identifies if there is a necessity to delete bridge | [optional] [default to $false]

### Return type

[**CartDisconnect200Response**](CartDisconnect200Response.md) (PSCustomObject)

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
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
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

$PageCursor = "MyPageCursor" # String | Used to retrieve entities via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$Start = 0 # Int32 | This parameter sets the number from which you want to get entities (optional) (default to 0)
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$StoreId = "1" # String | Store Id (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,code,name")
$ResponseFields = "{pagination,result{gift_card{id,code,amount,status}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# cart.giftcard.list
try {
    $Result = Invoke-CartGiftcardList -PageCursor $PageCursor -Start $Start -Count $Count -StoreId $StoreId -Params $Params -ResponseFields $ResponseFields -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartGiftcardList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **StoreId** | **String**| Store Id | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,code,name&quot;]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
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
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

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

$Params = "name,url" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "store_name,store_url,db_prefix")
$ResponseFields = "{result{name,url,stores_info{store_id,name,currency{id,iso3},store_owner_info}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Exclude = "name,url" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)
$StoreId = "1" # String | Store Id (optional)

# cart.info
try {
    $Result = Invoke-CartInfo -Params $Params -ResponseFields $ResponseFields -Exclude $Exclude -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartInfo: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;store_name,store_url,db_prefix&quot;]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**CartInfo200Response**](CartInfo200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartList"></a>
# **Invoke-CartList**
> CartList200Response Invoke-CartList<br>

cart.list

Get list of supported carts

### Example
```powershell
# general setting of the PowerShell module, e.g. base URL, authentication, etc
$Configuration = Get-Configuration
# Configure API key authorization: ApiKeyAuth
$Configuration.ApiKey.x-api-key = "YOUR_API_KEY"
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
#$Configuration.ApiKeyPrefix.x-api-key = "Bearer"


# cart.list
try {
    $Result = Invoke-CartList
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CartList200Response**](CartList200Response.md) (PSCustomObject)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-CartMetaDataList"></a>
# **Invoke-CartMetaDataList**
> ModelResponseCartMetaDataList Invoke-CartMetaDataList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EntityId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Entity] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-LangId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Key] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
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
$Entity = "order" # String | Entity (optional) (default to "product")
$StoreId = "1" # String | Store Id (optional)
$LangId = "3" # String | Language id (optional)
$Key = "subtotal" # String | Key (optional)
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$PageCursor = "MyPageCursor" # String | Used to retrieve entities via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "key,value")
$ResponseFields = "{result{items{key,value}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# cart.meta_data.list
try {
    $Result = Invoke-CartMetaDataList -EntityId $EntityId -Entity $Entity -StoreId $StoreId -LangId $LangId -Key $Key -Count $Count -PageCursor $PageCursor -Params $Params -ResponseFields $ResponseFields -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartMetaDataList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **EntityId** | **String**| Entity Id | 
 **Entity** | **String**| Entity | [optional] [default to &quot;product&quot;]
 **StoreId** | **String**| Store Id | [optional] 
 **LangId** | **String**| Language id | [optional] 
 **Key** | **String**| Key | [optional] 
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;key,value&quot;]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
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
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>

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

$StoreId = "1" # String | Store Id (optional)
$Start = 0 # Int32 | This parameter sets the number from which you want to get entities (optional) (default to 0)
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)

# cart.plugin.list
try {
    $Result = Invoke-CartPluginList -StoreId $StoreId -Start $Start -Count $Count
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartPluginList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **StoreId** | **String**| Store Id | [optional] 
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]

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
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ScriptIds] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
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

$PageCursor = "MyPageCursor" # String | Used to retrieve entities via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$Start = 0 # Int32 | This parameter sets the number from which you want to get entities (optional) (default to 0)
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$CreatedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their creation date (optional)
$CreatedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their creation date (optional)
$ModifiedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their modification date (optional)
$ModifiedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their modification date (optional)
$ScriptIds = "34023324,34024032" # String | Retrieves only scripts with specific ids (optional)
$StoreId = "1" # String | Store Id (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,name,description")
$ResponseFields = "{pagination,result{total_count,scripts{id,name,src,created_time{value}}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# cart.script.list
try {
    $Result = Invoke-CartScriptList -PageCursor $PageCursor -Start $Start -Count $Count -CreatedFrom $CreatedFrom -CreatedTo $CreatedTo -ModifiedFrom $ModifiedFrom -ModifiedTo $ModifiedTo -ScriptIds $ScriptIds -StoreId $StoreId -Params $Params -ResponseFields $ResponseFields -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartScriptList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
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
 **ScriptIds** | **String**| Retrieves only scripts with specific ids | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,name,description&quot;]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
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
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
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

$StoreId = "1" # String | Store Id (optional)
$Start = 0 # Int32 | This parameter sets the number from which you want to get entities (optional) (default to 0)
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,name,enabled")
$ResponseFields = "{result{id,name,enabled,countries,shipping_methods{name,rates}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# cart.shipping_zones.list
try {
    $Result = Invoke-CartShippingZonesList -StoreId $StoreId -Start $Start -Count $Count -Params $Params -ResponseFields $ResponseFields -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-CartShippingZonesList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **StoreId** | **String**| Store Id | [optional] 
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,name,enabled&quot;]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
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

