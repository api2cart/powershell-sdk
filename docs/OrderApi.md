# PSOpenAPITools.PSOpenAPITools\Api.OrderApi

All URIs are relative to *https://api.api2cart.com/v1.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Invoke-OrderAbandonedList**](OrderApi.md#Invoke-OrderAbandonedList) | **GET** /order.abandoned.list.json | order.abandoned.list
[**Invoke-OrderAdd**](OrderApi.md#Invoke-OrderAdd) | **POST** /order.add.json | order.add
[**Invoke-OrderCount**](OrderApi.md#Invoke-OrderCount) | **GET** /order.count.json | order.count
[**Invoke-OrderFinancialStatusList**](OrderApi.md#Invoke-OrderFinancialStatusList) | **GET** /order.financial_status.list.json | order.financial_status.list
[**Invoke-OrderFind**](OrderApi.md#Invoke-OrderFind) | **GET** /order.find.json | order.find
[**Invoke-OrderFulfillmentStatusList**](OrderApi.md#Invoke-OrderFulfillmentStatusList) | **GET** /order.fulfillment_status.list.json | order.fulfillment_status.list
[**Invoke-OrderInfo**](OrderApi.md#Invoke-OrderInfo) | **GET** /order.info.json | order.info
[**Invoke-OrderList**](OrderApi.md#Invoke-OrderList) | **GET** /order.list.json | order.list
[**Invoke-OrderPreestimateShippingList**](OrderApi.md#Invoke-OrderPreestimateShippingList) | **POST** /order.preestimate_shipping.list.json | order.preestimate_shipping.list
[**Invoke-OrderRefundAdd**](OrderApi.md#Invoke-OrderRefundAdd) | **POST** /order.refund.add.json | order.refund.add
[**Invoke-OrderReturnAdd**](OrderApi.md#Invoke-OrderReturnAdd) | **POST** /order.return.add.json | order.return.add
[**Invoke-OrderReturnDelete**](OrderApi.md#Invoke-OrderReturnDelete) | **DELETE** /order.return.delete.json | order.return.delete
[**Invoke-OrderReturnUpdate**](OrderApi.md#Invoke-OrderReturnUpdate) | **PUT** /order.return.update.json | order.return.update
[**Invoke-OrderShipmentAdd**](OrderApi.md#Invoke-OrderShipmentAdd) | **POST** /order.shipment.add.json | order.shipment.add
[**Invoke-OrderShipmentAddBatch**](OrderApi.md#Invoke-OrderShipmentAddBatch) | **POST** /order.shipment.add.batch.json | order.shipment.add.batch
[**Invoke-OrderShipmentDelete**](OrderApi.md#Invoke-OrderShipmentDelete) | **DELETE** /order.shipment.delete.json | order.shipment.delete
[**Invoke-OrderShipmentInfo**](OrderApi.md#Invoke-OrderShipmentInfo) | **GET** /order.shipment.info.json | order.shipment.info
[**Invoke-OrderShipmentList**](OrderApi.md#Invoke-OrderShipmentList) | **GET** /order.shipment.list.json | order.shipment.list
[**Invoke-OrderShipmentTrackingAdd**](OrderApi.md#Invoke-OrderShipmentTrackingAdd) | **POST** /order.shipment.tracking.add.json | order.shipment.tracking.add
[**Invoke-OrderShipmentUpdate**](OrderApi.md#Invoke-OrderShipmentUpdate) | **PUT** /order.shipment.update.json | order.shipment.update
[**Invoke-OrderStatusList**](OrderApi.md#Invoke-OrderStatusList) | **GET** /order.status.list.json | order.status.list
[**Invoke-OrderTransactionList**](OrderApi.md#Invoke-OrderTransactionList) | **GET** /order.transaction.list.json | order.transaction.list
[**Invoke-OrderUpdate**](OrderApi.md#Invoke-OrderUpdate) | **PUT** /order.update.json | order.update


<a id="Invoke-OrderAbandonedList"></a>
# **Invoke-OrderAbandonedList**
> ModelResponseOrderAbandonedList Invoke-OrderAbandonedList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerEmail] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SkipEmptyEmail] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

order.abandoned.list

Get list of orders that were left by customers before completing the order.

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
$CustomerId = "5" # String | Retrieves orders specified by customer id (optional)
$CustomerEmail = "jubari@hannsgroup.com" # String | Retrieves orders specified by customer email (optional)
$StoreId = "1" # String | Store Id (optional)
$CreatedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their creation date (optional)
$CreatedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their creation date (optional)
$ModifiedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their modification date (optional)
$ModifiedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their modification date (optional)
$SkipEmptyEmail = $true # Boolean | Filter empty emails (optional) (default to $false)
$ResponseFields = "{return_code,pagination,result{order{id,customer{email},created_at,totals{total},order_products}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "force_all" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "customer,totals,items")
$Exclude = "customer" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# order.abandoned.list
try {
    $Result = Invoke-OrderAbandonedList -Start $Start -Count $Count -PageCursor $PageCursor -CustomerId $CustomerId -CustomerEmail $CustomerEmail -StoreId $StoreId -CreatedFrom $CreatedFrom -CreatedTo $CreatedTo -ModifiedFrom $ModifiedFrom -ModifiedTo $ModifiedTo -SkipEmptyEmail $SkipEmptyEmail -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderAbandonedList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **CustomerId** | **String**| Retrieves orders specified by customer id | [optional] 
 **CustomerEmail** | **String**| Retrieves orders specified by customer email | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **CreatedFrom** | **String**| Retrieve entities from their creation date | [optional] 
 **CreatedTo** | **String**| Retrieve entities to their creation date | [optional] 
 **ModifiedFrom** | **String**| Retrieve entities from their modification date | [optional] 
 **ModifiedTo** | **String**| Retrieve entities to their modification date | [optional] 
 **SkipEmptyEmail** | **Boolean**| Filter empty emails | [optional] [default to $false]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;customer,totals,items&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseOrderAbandonedList**](ModelResponseOrderAbandonedList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderAdd"></a>
# **Invoke-OrderAdd**
> OrderAdd200Response Invoke-OrderAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderAdd] <PSCustomObject><br>

order.add

Add a new order to the cart.

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

$OrderAddNoteAttributesInner = Initialize-OrderAddNoteAttributesInner -Name "MyName" -Value "MyValue"

$OrderAddOrderItemInnerOrderItemOptionInner = Initialize-OrderAddOrderItemInnerOrderItemOptionInner -OrderItemOptionName "Color" -OrderItemOptionValue "green" -OrderItemOptionPrice 2.3
$OrderAddOrderItemInnerOrderItemPropertyInner = Initialize-OrderAddOrderItemInnerOrderItemPropertyInner -OrderItemPropertyName "Engraving" -OrderItemPropertyValue "lorem ipsum"
$OrderAddOrderItemInner = Initialize-OrderAddOrderItemInner -OrderItemId "125, where {x} - 1,2,3,... etc" -OrderItemName "Product 1, where {x} - 1,2,3,... etc" -OrderItemModel "sku_1, where {x} - 1,2,3,... etc" -OrderItemPrice 1.32, where {x} - 1,2,3,... etc -OrderItemQuantity 5, where {x} - 1,2,3,... etc -OrderItemWeight 5, where {x} - 1,2,3,... etc -OrderItemVariantId "52" -OrderItemTax 5.5 -OrderItemPriceIncludesTax $false -OrderItemParent 2 -OrderItemParentOptionName "Internal Memory Storage" -OrderItemAllowRefundItemsSeparately $true -OrderItemAllowShipItemsSeparately $true -OrderItemOption $OrderAddOrderItemInnerOrderItemOptionInner -OrderItemProperty $OrderAddOrderItemInnerOrderItemPropertyInner

$OrderAdd = Initialize-OrderAdd -Id "10" -OrderId "25" -StoreId "1" -ChannelId "1" -OrderStatus "Completed" -FulfillmentStatus "fulfilled" -FinancialStatus "paid" -CustomerEmail "jubari@hannsgroup.com" -CustomerFirstName "John" -CustomerLastName "Smith" -CustomerPhone "88008547457" -CustomerCountry "US" -CustomerBirthday "1990-12-03" -CustomerFax "5656598" -OrderPaymentMethod "PayPal" -TransactionId "d41d8cd98f00b204e9800998ecf8427e" -Currency "USD" -Date "2012-09-25 19:40:00" -DateModified "2014-05-05 05:05:00" -DateFinished "2014-06-05 05:05:00" -BillFirstName "Adam" -BillLastName "Smith" -BillAddress1 "Green str. 35" -BillAddress2 "Red str, 2" -BillCity "Chicago" -BillPostcode "12345" -BillState "IL" -BillCountry "US" -BillCompany "Apple" -BillPhone "8 800 5659 6896" -BillFax "545 45878" -ShippFirstName "John" -ShippLastName "Smith" -ShippAddress1 "Green str. 35" -ShippAddress2 "Green str. 35" -ShippCity "Chicago" -ShippPostcode "24545" -ShippState "IL" -ShippCountry "US" -ShippCompany "Apple" -ShippPhone "880086544564" -ShippFax "556868" -SubtotalPrice 563.23 -TaxPrice 5.5 -TotalPrice 23.56 -TotalPaid 23.56 -TotalWeight 23 -PricesIncTax $true -ShippingPrice 5.5 -ShippingTax 5.5 -Discount 5.5 -CouponDiscount 5.5 -GiftCertificateDiscount 5.5 -OrderShippingMethod "UPS Ground" -CarrierId "USPS" -WarehouseId "1" -Coupons "MyCoupons" -Tags "tag1,tag2" -Comment "This coole order" -AdminComment "Test admin comment" -AdminPrivateComment "Test admin private comment" -SendNotifications $true -SendAdminNotifications $true -ExternalSource "POS" -InventoryBehaviour "decrement_ignoring_policy" -CreateInvoice $true -NoteAttributes $OrderAddNoteAttributesInner -ClearCache $false -Origin "newsletter" -OrderItem $OrderAddOrderItemInner # OrderAdd | 

# order.add
try {
    $Result = Invoke-OrderAdd -OrderAdd $OrderAdd
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **OrderAdd** | [**OrderAdd**](OrderAdd.md)|  | 

### Return type

[**OrderAdd200Response**](OrderAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderCount"></a>
# **Invoke-OrderCount**
> OrderCount200Response Invoke-OrderCount<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderIds] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Ids] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerEmail] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderStatus] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderStatusIds] <String[]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EbayOrderStatus] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FinancialStatus] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FinancialStatusIds] <String[]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FulfillmentChannel] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FulfillmentStatus] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShippingMethod] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DeliveryMethod] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Tags] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShipNodeType] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTo] <String><br>

order.count

Count orders in store

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

$OrderIds = "24,25" # String | Counts orders specified by order ids (optional)
$Ids = "24,25" # String | Counts orders specified by ids (optional)
$CustomerId = "5" # String | Counts orders quantity specified by customer id (optional)
$StoreId = "1" # String | Counts orders quantity specified by store id (optional)
$CustomerEmail = "jubari@hannsgroup.com" # String | Counts orders quantity specified by customer email (optional)
$OrderStatus = "Completed" # String | Counts orders quantity specified by order status (optional)
$OrderStatusIds = "MyOrderStatusIds" # String[] | Retrieves orders specified by order statuses (optional)
$EbayOrderStatus = "Active" # String | Counts orders quantity specified by order status (optional)
$FinancialStatus = "paid" # String | Counts orders quantity specified by financial status (optional)
$FinancialStatusIds = "MyFinancialStatusIds" # String[] | Retrieves orders count specified by financial status ids (optional)
$FulfillmentChannel = "local" # String | Retrieves order with a fulfillment channel (optional)
$FulfillmentStatus = "fulfilled" # String | Create order with fulfillment status (optional)
$ShippingMethod = "flatrate_flatrate" # String | Retrieve entities according to shipping method (optional)
$DeliveryMethod = "local" # String | Retrieves order with delivery method (optional)
$Tags = "tag1,tag2" # String | Order tags (optional)
$ShipNodeType = "SellerFulfilled" # String | Retrieves order with ship node type (optional)
$CreatedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their creation date (optional)
$CreatedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their creation date (optional)
$ModifiedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their modification date (optional)
$ModifiedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their modification date (optional)

# order.count
try {
    $Result = Invoke-OrderCount -OrderIds $OrderIds -Ids $Ids -CustomerId $CustomerId -StoreId $StoreId -CustomerEmail $CustomerEmail -OrderStatus $OrderStatus -OrderStatusIds $OrderStatusIds -EbayOrderStatus $EbayOrderStatus -FinancialStatus $FinancialStatus -FinancialStatusIds $FinancialStatusIds -FulfillmentChannel $FulfillmentChannel -FulfillmentStatus $FulfillmentStatus -ShippingMethod $ShippingMethod -DeliveryMethod $DeliveryMethod -Tags $Tags -ShipNodeType $ShipNodeType -CreatedFrom $CreatedFrom -CreatedTo $CreatedTo -ModifiedFrom $ModifiedFrom -ModifiedTo $ModifiedTo
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderCount: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **OrderIds** | **String**| Counts orders specified by order ids | [optional] 
 **Ids** | **String**| Counts orders specified by ids | [optional] 
 **CustomerId** | **String**| Counts orders quantity specified by customer id | [optional] 
 **StoreId** | **String**| Counts orders quantity specified by store id | [optional] 
 **CustomerEmail** | **String**| Counts orders quantity specified by customer email | [optional] 
 **OrderStatus** | **String**| Counts orders quantity specified by order status | [optional] 
 **OrderStatusIds** | [**String[]**](String.md)| Retrieves orders specified by order statuses | [optional] 
 **EbayOrderStatus** | **String**| Counts orders quantity specified by order status | [optional] 
 **FinancialStatus** | **String**| Counts orders quantity specified by financial status | [optional] 
 **FinancialStatusIds** | [**String[]**](String.md)| Retrieves orders count specified by financial status ids | [optional] 
 **FulfillmentChannel** | **String**| Retrieves order with a fulfillment channel | [optional] 
 **FulfillmentStatus** | **String**| Create order with fulfillment status | [optional] 
 **ShippingMethod** | **String**| Retrieve entities according to shipping method | [optional] 
 **DeliveryMethod** | **String**| Retrieves order with delivery method | [optional] 
 **Tags** | **String**| Order tags | [optional] 
 **ShipNodeType** | **String**| Retrieves order with ship node type | [optional] 
 **CreatedFrom** | **String**| Retrieve entities from their creation date | [optional] 
 **CreatedTo** | **String**| Retrieve entities to their creation date | [optional] 
 **ModifiedFrom** | **String**| Retrieve entities from their modification date | [optional] 
 **ModifiedTo** | **String**| Retrieve entities to their modification date | [optional] 

### Return type

[**OrderCount200Response**](OrderCount200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderFinancialStatusList"></a>
# **Invoke-OrderFinancialStatusList**
> OrderFinancialStatusList200Response Invoke-OrderFinancialStatusList<br>

order.financial_status.list

Retrieve list of financial statuses

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


# order.financial_status.list
try {
    $Result = Invoke-OrderFinancialStatusList
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderFinancialStatusList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**OrderFinancialStatusList200Response**](OrderFinancialStatusList200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderFind"></a>
# **Invoke-OrderFind**
> OrderFind200Response Invoke-OrderFind<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerEmail] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderStatus] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FinancialStatus] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

order.find

This method is deprecated and won't be supported in the future. Please use ""order.list"" instead.

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
$CustomerId = "5" # String | Retrieves orders specified by customer id (optional)
$CustomerEmail = "jubari@hannsgroup.com" # String | Retrieves orders specified by customer email (optional)
$OrderStatus = "Completed" # String | Retrieves orders specified by order status (optional)
$FinancialStatus = "paid" # String | Retrieves orders specified by financial status (optional)
$CreatedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their creation date (optional)
$CreatedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their creation date (optional)
$ModifiedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their modification date (optional)
$ModifiedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their modification date (optional)
$Params = "order_id,totals,status" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "order_id,customer,totals,address,items,bundles,status")
$Exclude = "order_id,totals,status" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# order.find
try {
    $Result = Invoke-OrderFind -Start $Start -Count $Count -CustomerId $CustomerId -CustomerEmail $CustomerEmail -OrderStatus $OrderStatus -FinancialStatus $FinancialStatus -CreatedTo $CreatedTo -CreatedFrom $CreatedFrom -ModifiedTo $ModifiedTo -ModifiedFrom $ModifiedFrom -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderFind: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **CustomerId** | **String**| Retrieves orders specified by customer id | [optional] 
 **CustomerEmail** | **String**| Retrieves orders specified by customer email | [optional] 
 **OrderStatus** | **String**| Retrieves orders specified by order status | [optional] 
 **FinancialStatus** | **String**| Retrieves orders specified by financial status | [optional] 
 **CreatedTo** | **String**| Retrieve entities to their creation date | [optional] 
 **CreatedFrom** | **String**| Retrieve entities from their creation date | [optional] 
 **ModifiedTo** | **String**| Retrieve entities to their modification date | [optional] 
 **ModifiedFrom** | **String**| Retrieve entities from their modification date | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;order_id,customer,totals,address,items,bundles,status&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**OrderFind200Response**](OrderFind200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderFulfillmentStatusList"></a>
# **Invoke-OrderFulfillmentStatusList**
> OrderFulfillmentStatusList200Response Invoke-OrderFulfillmentStatusList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Action] <String><br>

order.fulfillment_status.list

Retrieve list of fulfillment statuses

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

$Action = "add" # String | Available statuses for the specified action. (optional)

# order.fulfillment_status.list
try {
    $Result = Invoke-OrderFulfillmentStatusList -Action $Action
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderFulfillmentStatusList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Action** | **String**| Available statuses for the specified action. | [optional] 

### Return type

[**OrderFulfillmentStatusList200Response**](OrderFulfillmentStatusList200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderInfo"></a>
# **Invoke-OrderInfo**
> OrderInfo200Response Invoke-OrderInfo<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EnableCache] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-UseLatestApiVersion] <System.Nullable[Boolean]><br>

order.info

Info about a specific order by ID

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

$Id = "10" # String | Retrieves order info specified by id (optional)
$OrderId = "25" # String | Retrieves order’s info specified by order id (optional)
$StoreId = "1" # String | Defines store id where the order should be found (optional)
$Params = "order_id,totals,status" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "order_id,customer,totals,address,items,bundles,status")
$ResponseFields = "{result{order_id,customer,totals,address,items,bundles,status}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Exclude = "order_id,totals,status" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)
$EnableCache = $true # Boolean | If the value is 'true' and order exist in our cache, we will return order.info response from cache (optional) (default to $false)
$UseLatestApiVersion = $true # Boolean | Use the latest platform API version (optional) (default to $false)

# order.info
try {
    $Result = Invoke-OrderInfo -Id $Id -OrderId $OrderId -StoreId $StoreId -Params $Params -ResponseFields $ResponseFields -Exclude $Exclude -EnableCache $EnableCache -UseLatestApiVersion $UseLatestApiVersion
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderInfo: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Retrieves order info specified by id | [optional] 
 **OrderId** | **String**| Retrieves order’s info specified by order id | [optional] 
 **StoreId** | **String**| Defines store id where the order should be found | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;order_id,customer,totals,address,items,bundles,status&quot;]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 
 **EnableCache** | **Boolean**| If the value is &#39;true&#39; and order exist in our cache, we will return order.info response from cache | [optional] [default to $false]
 **UseLatestApiVersion** | **Boolean**| Use the latest platform API version | [optional] [default to $false]

### Return type

[**OrderInfo200Response**](OrderInfo200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderList"></a>
# **Invoke-OrderList**
> ModelResponseOrderList Invoke-OrderList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Ids] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderIds] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SinceId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CustomerEmail] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-BasketId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CurrencyId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Phone] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderStatus] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderStatusIds] <String[]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EbayOrderStatus] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FinancialStatus] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FinancialStatusIds] <String[]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FulfillmentStatus] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ReturnStatus] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FulfillmentChannel] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShippingMethod] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SkipOrderIds] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-IsDeleted] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShippingCountryIso3] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DeliveryMethod] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShipNodeType] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Tags] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SortBy] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SortDirection] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-EnableCache] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-UseLatestApiVersion] <System.Nullable[Boolean]><br>

order.list

Get list of orders from store.

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
$PageCursor = "MyPageCursor" # String | Used to retrieve orders via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$Ids = "24,25" # String | Retrieves orders specified by ids (optional)
$OrderIds = "24,25" # String | Retrieves orders specified by order ids (optional)
$SinceId = "56" # String | Retrieve entities starting from the specified id. (optional)
$StoreId = "1" # String | Store Id (optional)
$CustomerId = "5" # String | Retrieves orders specified by customer id (optional)
$CustomerEmail = "jubari@hannsgroup.com" # String | Retrieves orders specified by customer email (optional)
$BasketId = "1" # String | Retrieves order’s info specified by basket id. (optional)
$CurrencyId = "usd" # String | Currency Id (optional)
$Phone = "56686868654" # String | Filter orders by customer's phone number (optional)
$OrderStatus = "Completed" # String | Retrieves orders specified by order status (optional)
$OrderStatusIds = "MyOrderStatusIds" # String[] | Retrieves orders specified by order statuses (optional)
$EbayOrderStatus = "Active" # String | Retrieves orders specified by order status (optional)
$FinancialStatus = "paid" # String | Retrieves orders specified by financial status (optional)
$FinancialStatusIds = "MyFinancialStatusIds" # String[] | Retrieves orders specified by financial status ids (optional)
$FulfillmentStatus = "fulfilled" # String | Create order with fulfillment status (optional)
$ReturnStatus = "RETURNED" # String | Retrieves orders specified by return status (optional)
$FulfillmentChannel = "local" # String | Retrieves order with a fulfillment channel (optional)
$ShippingMethod = "flatrate_flatrate" # String | Retrieve entities according to shipping method (optional)
$SkipOrderIds = "24,25" # String | Skipped orders by ids (optional)
$IsDeleted = $true # Boolean | Filter deleted orders (optional)
$ShippingCountryIso3 = "DEU" # String | Retrieve entities according to shipping country (optional)
$DeliveryMethod = "local" # String | Retrieves order with delivery method (optional)
$ShipNodeType = "SellerFulfilled" # String | Retrieves order with ship node type (optional)
$CreatedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their creation date (optional)
$CreatedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their creation date (optional)
$ModifiedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their modification date (optional)
$ModifiedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their modification date (optional)
$Tags = "tag1,tag2" # String | Order tags (optional)
$SortBy = "modified_at" # String | Set field to sort by (optional) (default to "order_id")
$SortDirection = "asc" # String | Set sorting direction (optional) (default to "asc")
$Params = "order_id,totals,status" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "order_id,customer,totals,address,items,bundles,status")
$ResponseFields = "{return_code,pagination,result{order{order_id,customer,totals,address,items,bundles,status}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Exclude = "order_id,totals,status" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)
$EnableCache = $true # Boolean | If the value is 'true', we will cache orders for a 15 minutes in order to increase speed and reduce requests throttling for some methods and shoping platforms (for example order.shipment.add) (optional) (default to $false)
$UseLatestApiVersion = $true # Boolean | Use the latest platform API version (optional) (default to $false)

# order.list
try {
    $Result = Invoke-OrderList -Start $Start -Count $Count -PageCursor $PageCursor -Ids $Ids -OrderIds $OrderIds -SinceId $SinceId -StoreId $StoreId -CustomerId $CustomerId -CustomerEmail $CustomerEmail -BasketId $BasketId -CurrencyId $CurrencyId -Phone $Phone -OrderStatus $OrderStatus -OrderStatusIds $OrderStatusIds -EbayOrderStatus $EbayOrderStatus -FinancialStatus $FinancialStatus -FinancialStatusIds $FinancialStatusIds -FulfillmentStatus $FulfillmentStatus -ReturnStatus $ReturnStatus -FulfillmentChannel $FulfillmentChannel -ShippingMethod $ShippingMethod -SkipOrderIds $SkipOrderIds -IsDeleted $IsDeleted -ShippingCountryIso3 $ShippingCountryIso3 -DeliveryMethod $DeliveryMethod -ShipNodeType $ShipNodeType -CreatedTo $CreatedTo -CreatedFrom $CreatedFrom -ModifiedTo $ModifiedTo -ModifiedFrom $ModifiedFrom -Tags $Tags -SortBy $SortBy -SortDirection $SortDirection -Params $Params -ResponseFields $ResponseFields -Exclude $Exclude -EnableCache $EnableCache -UseLatestApiVersion $UseLatestApiVersion
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve orders via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **Ids** | **String**| Retrieves orders specified by ids | [optional] 
 **OrderIds** | **String**| Retrieves orders specified by order ids | [optional] 
 **SinceId** | **String**| Retrieve entities starting from the specified id. | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **CustomerId** | **String**| Retrieves orders specified by customer id | [optional] 
 **CustomerEmail** | **String**| Retrieves orders specified by customer email | [optional] 
 **BasketId** | **String**| Retrieves order’s info specified by basket id. | [optional] 
 **CurrencyId** | **String**| Currency Id | [optional] 
 **Phone** | **String**| Filter orders by customer&#39;s phone number | [optional] 
 **OrderStatus** | **String**| Retrieves orders specified by order status | [optional] 
 **OrderStatusIds** | [**String[]**](String.md)| Retrieves orders specified by order statuses | [optional] 
 **EbayOrderStatus** | **String**| Retrieves orders specified by order status | [optional] 
 **FinancialStatus** | **String**| Retrieves orders specified by financial status | [optional] 
 **FinancialStatusIds** | [**String[]**](String.md)| Retrieves orders specified by financial status ids | [optional] 
 **FulfillmentStatus** | **String**| Create order with fulfillment status | [optional] 
 **ReturnStatus** | **String**| Retrieves orders specified by return status | [optional] 
 **FulfillmentChannel** | **String**| Retrieves order with a fulfillment channel | [optional] 
 **ShippingMethod** | **String**| Retrieve entities according to shipping method | [optional] 
 **SkipOrderIds** | **String**| Skipped orders by ids | [optional] 
 **IsDeleted** | **Boolean**| Filter deleted orders | [optional] 
 **ShippingCountryIso3** | **String**| Retrieve entities according to shipping country | [optional] 
 **DeliveryMethod** | **String**| Retrieves order with delivery method | [optional] 
 **ShipNodeType** | **String**| Retrieves order with ship node type | [optional] 
 **CreatedTo** | **String**| Retrieve entities to their creation date | [optional] 
 **CreatedFrom** | **String**| Retrieve entities from their creation date | [optional] 
 **ModifiedTo** | **String**| Retrieve entities to their modification date | [optional] 
 **ModifiedFrom** | **String**| Retrieve entities from their modification date | [optional] 
 **Tags** | **String**| Order tags | [optional] 
 **SortBy** | **String**| Set field to sort by | [optional] [default to &quot;order_id&quot;]
 **SortDirection** | **String**| Set sorting direction | [optional] [default to &quot;asc&quot;]
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;order_id,customer,totals,address,items,bundles,status&quot;]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 
 **EnableCache** | **Boolean**| If the value is &#39;true&#39;, we will cache orders for a 15 minutes in order to increase speed and reduce requests throttling for some methods and shoping platforms (for example order.shipment.add) | [optional] [default to $false]
 **UseLatestApiVersion** | **Boolean**| Use the latest platform API version | [optional] [default to $false]

### Return type

[**ModelResponseOrderList**](ModelResponseOrderList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderPreestimateShippingList"></a>
# **Invoke-OrderPreestimateShippingList**
> ModelResponseOrderPreestimateShippingList Invoke-OrderPreestimateShippingList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderPreestimateShippingList] <PSCustomObject><br>

order.preestimate_shipping.list

Retrieve list of order preestimated shipping methods

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

$OrderPreestimateShippingListOrderItemInnerOrderItemOptionInner = Initialize-OrderPreestimateShippingListOrderItemInnerOrderItemOptionInner -OrderItemOptionName "Color" -OrderItemOptionId "12" -OrderItemOptionValue "green" -OrderItemOptionValueId "13" -OrderItemOptionUsedInCombinations $false
$OrderPreestimateShippingListOrderItemInner = Initialize-OrderPreestimateShippingListOrderItemInner -OrderItemId "125, where {x} - 1,2,3,... etc" -OrderItemModel "sku_1, where {x} - 1,2,3,... etc" -OrderItemQuantity 5, where {x} - 1,2,3,... etc -OrderItemWeight 5, where {x} - 1,2,3,... etc -OrderItemVariantId "52" -OrderItemOption $OrderPreestimateShippingListOrderItemInnerOrderItemOptionInner

$OrderPreestimateShippingList = Initialize-OrderPreestimateShippingList -WarehouseId "1" -CustomerId "5" -CustomerEmail "jubari@hannsgroup.com" -StoreId "1" -ShippAddress1 "Green str. 35" -ShippCity "Chicago" -ShippPostcode "24545" -ShippState "IL" -ShippCountry "US" -Params "id,model,price,images" -Exclude "false" -OrderItem $OrderPreestimateShippingListOrderItemInner # OrderPreestimateShippingList | 

# order.preestimate_shipping.list
try {
    $Result = Invoke-OrderPreestimateShippingList -OrderPreestimateShippingList $OrderPreestimateShippingList
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderPreestimateShippingList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **OrderPreestimateShippingList** | [**OrderPreestimateShippingList**](OrderPreestimateShippingList.md)|  | 

### Return type

[**ModelResponseOrderPreestimateShippingList**](ModelResponseOrderPreestimateShippingList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderRefundAdd"></a>
# **Invoke-OrderRefundAdd**
> OrderRefundAdd200Response Invoke-OrderRefundAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderRefundAdd] <PSCustomObject><br>

order.refund.add

Add a refund to the order.

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

$OrderRefundAddItemsInner = Initialize-OrderRefundAddItemsInner -OrderProductId "MyOrderProductId" -Quantity 0 -Price 0
$OrderRefundAdd = Initialize-OrderRefundAdd -OrderId "25" -Items $OrderRefundAddItemsInner -TotalPrice 23.56 -ShippingPrice 5.5 -FeePrice 5.5 -Message "Received item is not like in the photo, get my money back." -ItemRestock $true -SendNotifications $true -Date "2012-09-25 19:40:00" -IsOnline $false # OrderRefundAdd | 

# order.refund.add
try {
    $Result = Invoke-OrderRefundAdd -OrderRefundAdd $OrderRefundAdd
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderRefundAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **OrderRefundAdd** | [**OrderRefundAdd**](OrderRefundAdd.md)|  | 

### Return type

[**OrderRefundAdd200Response**](OrderRefundAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderReturnAdd"></a>
# **Invoke-OrderReturnAdd**
> OrderReturnAdd200Response Invoke-OrderReturnAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderReturnAdd] <PSCustomObject><br>

order.return.add

Create new return request.

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

$OrderReturnAddOrderProductsInner = Initialize-OrderReturnAddOrderProductsInner -OrderProductId "125, where {x} - 1,2,3,... etc" -OrderProductQuantity 1, where {x} - 1,2,3,... etc -OrderProductReasonId "DEFECTIVE, where {x} - 1,2,3,... etc" -OrderProductActionId "REFUND, where {x} - 1,2,3,... etc" -OrderProductCustomerComment "I need a bigger size, where {x} - 1,2,3,... etc" -OrderProductHandlingStatus "123456" -OrderProductCondition "Broken, where {x} - 1,2,3,... etc" -OrderProductReason "123456" -OrderProductStatus "pending"
$OrderReturnAdd = Initialize-OrderReturnAdd -OrderId "25" -StoreId "1" -ReturnStatusId "RETURNED" -ReturnActionId "RETURNED" -ReturnReasonId "broken" -ReturnReason "broken" -ItemRestock $true -StaffNote "Test" -Comment "This coole order" -SendNotifications $true -RejectReason "ORDER_UNPAID" -OrderProducts $OrderReturnAddOrderProductsInner # OrderReturnAdd | 

# order.return.add
try {
    $Result = Invoke-OrderReturnAdd -OrderReturnAdd $OrderReturnAdd
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderReturnAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **OrderReturnAdd** | [**OrderReturnAdd**](OrderReturnAdd.md)|  | 

### Return type

[**OrderReturnAdd200Response**](OrderReturnAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderReturnDelete"></a>
# **Invoke-OrderReturnDelete**
> AttributeValueDelete200Response Invoke-OrderReturnDelete<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ReturnId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

order.return.delete

Delete return.

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

$ReturnId = "200000002" # String | Return ID
$OrderId = "25" # String | Defines the order id
$StoreId = "1" # String | Store Id (optional)

# order.return.delete
try {
    $Result = Invoke-OrderReturnDelete -ReturnId $ReturnId -OrderId $OrderId -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderReturnDelete: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ReturnId** | **String**| Return ID | 
 **OrderId** | **String**| Defines the order id | 
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**AttributeValueDelete200Response**](AttributeValueDelete200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderReturnUpdate"></a>
# **Invoke-OrderReturnUpdate**
> AccountConfigUpdate200Response Invoke-OrderReturnUpdate<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderReturnUpdate] <PSCustomObject><br>

order.return.update

Update order's shipment information.

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

$OrderReturnUpdateOrderProductsInner = Initialize-OrderReturnUpdateOrderProductsInner -OrderProductId "125, where {x} - 1,2,3,... etc" -OrderProductQuantity 1, where {x} - 1,2,3,... etc -OrderProductStatus "pending" -OrderProductActionId "REFUND, where {x} - 1,2,3,... etc"
$OrderReturnUpdate = Initialize-OrderReturnUpdate -ReturnId "200000002" -OrderId "25" -StoreId "1" -ItemRestock $true -ReturnStatusId "RETURNED" -StaffNote "Test" -Comment "This coole order" -SendNotifications $true -RejectReason "ORDER_UNPAID" -OrderProducts $OrderReturnUpdateOrderProductsInner # OrderReturnUpdate | 

# order.return.update
try {
    $Result = Invoke-OrderReturnUpdate -OrderReturnUpdate $OrderReturnUpdate
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderReturnUpdate: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **OrderReturnUpdate** | [**OrderReturnUpdate**](OrderReturnUpdate.md)|  | 

### Return type

[**AccountConfigUpdate200Response**](AccountConfigUpdate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderShipmentAdd"></a>
# **Invoke-OrderShipmentAdd**
> OrderShipmentAdd200Response Invoke-OrderShipmentAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderShipmentAdd] <PSCustomObject><br>

order.shipment.add

Add a shipment to the order.

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

$OrderShipmentAddItemsInner = Initialize-OrderShipmentAddItemsInner -OrderProductId "MyOrderProductId" -Quantity 0
$OrderShipmentAddTrackingNumbersInner = Initialize-OrderShipmentAddTrackingNumbersInner -CarrierId "MyCarrierId" -TrackingNumber "MyTrackingNumber"
$OrderShipmentAdd = Initialize-OrderShipmentAdd -OrderId "25" -WarehouseId "1" -StoreId "1" -ShipmentProvider "UPS" -ShippingMethod "flatrate_flatrate" -Items $OrderShipmentAddItemsInner -TrackingNumbers $OrderShipmentAddTrackingNumbersInner -TrackingLink "http://example.com?someParam=value" -IsShipped $true -SendNotifications $true -AdjustStock $true -EnableCache $true -CheckProcessStatus $false -TrackingProvider "Custom tracker" -UseLatestApiVersion $true # OrderShipmentAdd | 

# order.shipment.add
try {
    $Result = Invoke-OrderShipmentAdd -OrderShipmentAdd $OrderShipmentAdd
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderShipmentAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **OrderShipmentAdd** | [**OrderShipmentAdd**](OrderShipmentAdd.md)|  | 

### Return type

[**OrderShipmentAdd200Response**](OrderShipmentAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderShipmentAddBatch"></a>
# **Invoke-OrderShipmentAddBatch**
> CategoryAddBatch200Response Invoke-OrderShipmentAddBatch<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderShipmentAddBatch] <PSCustomObject><br>

order.shipment.add.batch

Add a shipments to the orders.

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

$OrderShipmentAddBatchPayloadInnerItemsInner = Initialize-OrderShipmentAddBatchPayloadInnerItemsInner -OrderProductId "MyOrderProductId" -Quantity 0
$OrderShipmentAddBatchPayloadInner = Initialize-OrderShipmentAddBatchPayloadInner -OrderId "MyOrderId" -StoreId "MyStoreId" -WarehouseId "MyWarehouseId" -CarrierId "MyCarrierId" -CarrierName "MyCarrierName" -TrackingNumber "MyTrackingNumber" -TrackingLink "MyTrackingLink" -ShipmentProvider "MyShipmentProvider" -Items $OrderShipmentAddBatchPayloadInnerItemsInner -SendNotifications $false

$OrderShipmentAddBatch = Initialize-OrderShipmentAddBatch -Payload $OrderShipmentAddBatchPayloadInner # OrderShipmentAddBatch | 

# order.shipment.add.batch
try {
    $Result = Invoke-OrderShipmentAddBatch -OrderShipmentAddBatch $OrderShipmentAddBatch
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderShipmentAddBatch: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **OrderShipmentAddBatch** | [**OrderShipmentAddBatch**](OrderShipmentAddBatch.md)|  | 

### Return type

[**CategoryAddBatch200Response**](CategoryAddBatch200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderShipmentDelete"></a>
# **Invoke-OrderShipmentDelete**
> OrderShipmentDelete200Response Invoke-OrderShipmentDelete<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ShipmentId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>

order.shipment.delete

Delete order's shipment.

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

$ShipmentId = "200000002" # String | Shipment id indicates the number of delivery
$OrderId = "25" # String | Defines the order for which the shipment will be deleted
$StoreId = "1" # String | Store Id (optional)

# order.shipment.delete
try {
    $Result = Invoke-OrderShipmentDelete -ShipmentId $ShipmentId -OrderId $OrderId -StoreId $StoreId
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderShipmentDelete: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ShipmentId** | **String**| Shipment id indicates the number of delivery | 
 **OrderId** | **String**| Defines the order for which the shipment will be deleted | 
 **StoreId** | **String**| Store Id | [optional] 

### Return type

[**OrderShipmentDelete200Response**](OrderShipmentDelete200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderShipmentInfo"></a>
# **Invoke-OrderShipmentInfo**
> OrderShipmentInfo200Response Invoke-OrderShipmentInfo<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Id] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

order.shipment.info

Get information of shipment.

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
$OrderId = "25" # String | Defines the order id
$Start = 0 # Int32 | This parameter sets the number from which you want to get entities (optional) (default to 0)
$StoreId = "1" # String | Store Id (optional)
$ResponseFields = "{result{id,order_id,shipment_provider,tracking_numbers{tracking_number},items{product_id,quantity}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,order_id,items,tracking_numbers")
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# order.shipment.info
try {
    $Result = Invoke-OrderShipmentInfo -Id $Id -OrderId $OrderId -Start $Start -StoreId $StoreId -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderShipmentInfo: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **Id** | **String**| Entity id | 
 **OrderId** | **String**| Defines the order id | 
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **StoreId** | **String**| Store Id | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,order_id,items,tracking_numbers&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**OrderShipmentInfo200Response**](OrderShipmentInfo200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderShipmentList"></a>
# **Invoke-OrderShipmentList**
> ModelResponseOrderShipmentList Invoke-OrderShipmentList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Start] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreatedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedFrom] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ModifiedTo] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

order.shipment.list

Get list of shipments by orders.

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

$OrderId = "25" # String | Retrieves shipments specified by order id
$Start = 0 # Int32 | This parameter sets the number from which you want to get entities (optional) (default to 0)
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$PageCursor = "MyPageCursor" # String | Used to retrieve entities via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$StoreId = "1" # String | Store Id (optional)
$CreatedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their creation date (optional)
$CreatedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their creation date (optional)
$ModifiedFrom = "2010-07-29 13:45:52" # String | Retrieve entities from their modification date (optional)
$ModifiedTo = "2100-08-29 13:45:52" # String | Retrieve entities to their modification date (optional)
$ResponseFields = "{status_code,pagination,result{shipment{id,order_id,shipment_provider,tracking_numbers{tracking_number},items{product_id,quantity}}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,order_id,items,tracking_numbers")
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# order.shipment.list
try {
    $Result = Invoke-OrderShipmentList -OrderId $OrderId -Start $Start -Count $Count -PageCursor $PageCursor -StoreId $StoreId -CreatedFrom $CreatedFrom -CreatedTo $CreatedTo -ModifiedFrom $ModifiedFrom -ModifiedTo $ModifiedTo -ResponseFields $ResponseFields -Params $Params -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderShipmentList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **OrderId** | **String**| Retrieves shipments specified by order id | 
 **Start** | **Int32**| This parameter sets the number from which you want to get entities | [optional] [default to 0]
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **CreatedFrom** | **String**| Retrieve entities from their creation date | [optional] 
 **CreatedTo** | **String**| Retrieve entities to their creation date | [optional] 
 **ModifiedFrom** | **String**| Retrieve entities from their modification date | [optional] 
 **ModifiedTo** | **String**| Retrieve entities to their modification date | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,order_id,items,tracking_numbers&quot;]
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseOrderShipmentList**](ModelResponseOrderShipmentList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderShipmentTrackingAdd"></a>
# **Invoke-OrderShipmentTrackingAdd**
> OrderShipmentTrackingAdd200Response Invoke-OrderShipmentTrackingAdd<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderShipmentTrackingAdd] <PSCustomObject><br>

order.shipment.tracking.add

Add order shipment's tracking info.

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

$OrderShipmentTrackingAdd = Initialize-OrderShipmentTrackingAdd -OrderId "25" -ShipmentId "200000002" -CarrierId "USPS" -StoreId "1" -TrackingProvider "Custom tracker" -TrackingNumber "1А6745" -TrackingLink "http://example.com?someParam=value" -SendNotifications $true # OrderShipmentTrackingAdd | 

# order.shipment.tracking.add
try {
    $Result = Invoke-OrderShipmentTrackingAdd -OrderShipmentTrackingAdd $OrderShipmentTrackingAdd
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderShipmentTrackingAdd: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **OrderShipmentTrackingAdd** | [**OrderShipmentTrackingAdd**](OrderShipmentTrackingAdd.md)|  | 

### Return type

[**OrderShipmentTrackingAdd200Response**](OrderShipmentTrackingAdd200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderShipmentUpdate"></a>
# **Invoke-OrderShipmentUpdate**
> AccountConfigUpdate200Response Invoke-OrderShipmentUpdate<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderShipmentUpdate] <PSCustomObject><br>

order.shipment.update

Update order's shipment information.

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

$OrderShipmentAddTrackingNumbersInner = Initialize-OrderShipmentAddTrackingNumbersInner -CarrierId "MyCarrierId" -TrackingNumber "MyTrackingNumber"
$OrderShipmentAddItemsInner = Initialize-OrderShipmentAddItemsInner -OrderProductId "MyOrderProductId" -Quantity 0
$OrderShipmentUpdate = Initialize-OrderShipmentUpdate -ShipmentId "200000002" -OrderId "25" -StoreId "1" -ShipmentProvider "UPS" -TrackingNumbers $OrderShipmentAddTrackingNumbersInner -TrackingLink "http://example.com?someParam=value" -IsShipped $true -DeliveredAt "2024-08-25T23:56:12+00:00" -Replace $false -SendNotifications $true -TrackingProvider "Custom tracker" -Items $OrderShipmentAddItemsInner # OrderShipmentUpdate | 

# order.shipment.update
try {
    $Result = Invoke-OrderShipmentUpdate -OrderShipmentUpdate $OrderShipmentUpdate
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderShipmentUpdate: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **OrderShipmentUpdate** | [**OrderShipmentUpdate**](OrderShipmentUpdate.md)|  | 

### Return type

[**AccountConfigUpdate200Response**](AccountConfigUpdate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderStatusList"></a>
# **Invoke-OrderStatusList**
> ModelResponseOrderStatusList Invoke-OrderStatusList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Action] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>

order.status.list

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

$StoreId = "1" # String | Store Id (optional)
$Action = "add" # String | Available statuses for the specified action. (optional)
$ResponseFields = "{return_code,return_message,result}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)

# order.status.list
try {
    $Result = Invoke-OrderStatusList -StoreId $StoreId -Action $Action -ResponseFields $ResponseFields
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderStatusList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **StoreId** | **String**| Store Id | [optional] 
 **Action** | **String**| Available statuses for the specified action. | [optional] 
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 

### Return type

[**ModelResponseOrderStatusList**](ModelResponseOrderStatusList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderTransactionList"></a>
# **Invoke-OrderTransactionList**
> ModelResponseOrderTransactionList Invoke-OrderTransactionList<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderIds] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Count] <System.Nullable[Int32]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-PageCursor] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Params] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-ResponseFields] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Exclude] <String><br>

order.transaction.list

Retrieve list of order transaction

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

$OrderIds = "24,25" # String | Retrieves order transactions specified by order ids
$Count = 20 # Int32 | This parameter sets the entity amount that has to be retrieved. Max allowed count=250 (optional) (default to 10)
$PageCursor = "MyPageCursor" # String | Used to retrieve entities via cursor-based pagination (it can't be used with any other filtering parameter) (optional)
$StoreId = "1" # String | Store Id (optional)
$Params = "id,model,price,images" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional) (default to "id,order_id,amount,description")
$ResponseFields = "{return_code,pagination,result{transactions_count,transactions{id,transaction_id,status,description,settlement_amount,gateway,card_brand,card_last_four}}}" # String | Set this parameter in order to choose which entity fields you want to retrieve (optional)
$Exclude = "false" # String | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter `params` equal force_all (optional)

# order.transaction.list
try {
    $Result = Invoke-OrderTransactionList -OrderIds $OrderIds -Count $Count -PageCursor $PageCursor -StoreId $StoreId -Params $Params -ResponseFields $ResponseFields -Exclude $Exclude
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderTransactionList: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **OrderIds** | **String**| Retrieves order transactions specified by order ids | 
 **Count** | **Int32**| This parameter sets the entity amount that has to be retrieved. Max allowed count&#x3D;250 | [optional] [default to 10]
 **PageCursor** | **String**| Used to retrieve entities via cursor-based pagination (it can&#39;t be used with any other filtering parameter) | [optional] 
 **StoreId** | **String**| Store Id | [optional] 
 **Params** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to &quot;id,order_id,amount,description&quot;]
 **ResponseFields** | **String**| Set this parameter in order to choose which entity fields you want to retrieve | [optional] 
 **Exclude** | **String**| Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 

### Return type

[**ModelResponseOrderTransactionList**](ModelResponseOrderTransactionList.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="Invoke-OrderUpdate"></a>
# **Invoke-OrderUpdate**
> AccountConfigUpdate200Response Invoke-OrderUpdate<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-StoreId] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderStatus] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FinancialStatus] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-FulfillmentStatus] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CancellationReason] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-OrderPaymentMethod] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Comment] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AdminComment] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-AdminPrivateComment] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-InvoiceAdminComment] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateModified] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DateFinished] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-SendNotifications] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-CreateInvoice] <System.Nullable[Boolean]><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Origin] <String><br>

order.update

Update existing order.

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

$OrderId = "25" # String | Defines the orders specified by order id
$StoreId = "1" # String | Defines store id where the order should be found (optional)
$OrderStatus = "Completed" # String | Defines new order's status (optional)
$FinancialStatus = "paid" # String | Update order financial status to specified (optional)
$FulfillmentStatus = "fulfilled" # String | Create order with fulfillment status (optional)
$CancellationReason = "ORDER_UNPAID" # String | Defines the cancellation reason when the order will be canceled (optional)
$OrderPaymentMethod = "PayPal" # String | Defines order payment method.<br/>Setting order_payment_method on Shopify will also change financial_status field value to 'paid' (optional)
$Comment = "This coole order" # String | Specifies order comment (optional)
$AdminComment = "Test admin comment" # String | Specifies admin's order comment (optional)
$AdminPrivateComment = "Test admin private comment" # String | Specifies private admin's order comment (optional)
$InvoiceAdminComment = "Test admin comment" # String | Specifies admin's order invoice comment (optional)
$DateModified = "2014-05-05 05:05:00" # String | Specifies order's  modification date (optional)
$DateFinished = "2014-06-05 05:05:00" # String | Specifies order's  finished date (optional)
$SendNotifications = $true # Boolean | Send notifications to customer after order was created (optional) (default to $false)
$CreateInvoice = $true # Boolean | Determines whether an invoice should be created if it has not already been created (optional)
$Origin = "newsletter" # String | The source of the order (optional)

# order.update
try {
    $Result = Invoke-OrderUpdate -OrderId $OrderId -StoreId $StoreId -OrderStatus $OrderStatus -FinancialStatus $FinancialStatus -FulfillmentStatus $FulfillmentStatus -CancellationReason $CancellationReason -OrderPaymentMethod $OrderPaymentMethod -Comment $Comment -AdminComment $AdminComment -AdminPrivateComment $AdminPrivateComment -InvoiceAdminComment $InvoiceAdminComment -DateModified $DateModified -DateFinished $DateFinished -SendNotifications $SendNotifications -CreateInvoice $CreateInvoice -Origin $Origin
} catch {
    Write-Host ("Exception occurred when calling Invoke-OrderUpdate: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **OrderId** | **String**| Defines the orders specified by order id | 
 **StoreId** | **String**| Defines store id where the order should be found | [optional] 
 **OrderStatus** | **String**| Defines new order&#39;s status | [optional] 
 **FinancialStatus** | **String**| Update order financial status to specified | [optional] 
 **FulfillmentStatus** | **String**| Create order with fulfillment status | [optional] 
 **CancellationReason** | **String**| Defines the cancellation reason when the order will be canceled | [optional] 
 **OrderPaymentMethod** | **String**| Defines order payment method.&lt;br/&gt;Setting order_payment_method on Shopify will also change financial_status field value to &#39;paid&#39; | [optional] 
 **Comment** | **String**| Specifies order comment | [optional] 
 **AdminComment** | **String**| Specifies admin&#39;s order comment | [optional] 
 **AdminPrivateComment** | **String**| Specifies private admin&#39;s order comment | [optional] 
 **InvoiceAdminComment** | **String**| Specifies admin&#39;s order invoice comment | [optional] 
 **DateModified** | **String**| Specifies order&#39;s  modification date | [optional] 
 **DateFinished** | **String**| Specifies order&#39;s  finished date | [optional] 
 **SendNotifications** | **Boolean**| Send notifications to customer after order was created | [optional] [default to $false]
 **CreateInvoice** | **Boolean**| Determines whether an invoice should be created if it has not already been created | [optional] 
 **Origin** | **String**| The source of the order | [optional] 

### Return type

[**AccountConfigUpdate200Response**](AccountConfigUpdate200Response.md) (PSCustomObject)

### Authorization

[StoreKeyAuth](../README.md#StoreKeyAuth), [ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

