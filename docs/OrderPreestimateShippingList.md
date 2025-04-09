# OrderPreestimateShippingList
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**StoreId** | **String** | Store Id | [optional] 
**WarehouseId** | **String** | This parameter is used for selecting a warehouse where you need to set/modify a product quantity. | [optional] 
**CustomerEmail** | **String** | Retrieves orders specified by customer email | [optional] 
**CustomerId** | **String** | Retrieves orders specified by customer id | [optional] 
**ShippAddress1** | **String** | Specifies first shipping address | [optional] 
**ShippCity** | **String** | Specifies shipping city | [optional] 
**ShippPostcode** | **String** | Specifies shipping postcode | [optional] 
**ShippState** | **String** | Specifies shipping state code | [optional] 
**ShippCountry** | **String** | Specifies shipping country code | 
**Params** | **String** | Set this parameter in order to choose which entity fields you want to retrieve | [optional] [default to "force_all"]
**Exclude** | **String** | Set this parameter in order to choose which entity fields you want to ignore. Works only if parameter &#x60;params&#x60; equal force_all | [optional] 
**OrderItem** | [**OrderPreestimateShippingListOrderItemInner[]**](OrderPreestimateShippingListOrderItemInner.md) |  | 

## Examples

- Prepare the resource
```powershell
$OrderPreestimateShippingList = Initialize-PSOpenAPIToolsOrderPreestimateShippingList  -StoreId 1 `
 -WarehouseId 1 `
 -CustomerEmail jubari@hannsgroup.com `
 -CustomerId 5 `
 -ShippAddress1 Green str. 35 `
 -ShippCity Chicago `
 -ShippPostcode 24545 `
 -ShippState IL `
 -ShippCountry US `
 -Params id,model,price,images `
 -Exclude false `
 -OrderItem null
```

- Convert the resource to JSON
```powershell
$OrderPreestimateShippingList | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

