# OrderPreestimateShippingListOrderItemInnerOrderItemOptionInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderItemOptionName** | **String** | Ordered Product Option Name. Where x is order item ID, y is order item option ID | [optional] 
**OrderItemOptionId** | **String** | Product Option ID. Where x is order item ID, y is order item option ID | [optional] 
**OrderItemOptionValue** | **String** | Ordered product option value Where x is order item ID, y - order item option ID | [optional] 
**OrderItemOptionValueId** | **String** | Product option value ID, where x is order item ID, y - order item option ID | [optional] 
**OrderItemOptionUsedInCombinations** | **Boolean** | Product option used in combinations flag, where x is order item ID, y - order item option ID | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderPreestimateShippingListOrderItemInnerOrderItemOptionInner = Initialize-PSOpenAPIToolsOrderPreestimateShippingListOrderItemInnerOrderItemOptionInner  -OrderItemOptionName Color `
 -OrderItemOptionId 12 `
 -OrderItemOptionValue green `
 -OrderItemOptionValueId 13 `
 -OrderItemOptionUsedInCombinations null
```

- Convert the resource to JSON
```powershell
$OrderPreestimateShippingListOrderItemInnerOrderItemOptionInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

