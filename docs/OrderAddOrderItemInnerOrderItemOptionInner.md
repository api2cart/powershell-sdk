# OrderAddOrderItemInnerOrderItemOptionInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderItemOptionName** | **String** | Ordered Product Option Name. Where x is order item ID, y is order item option ID | [optional] 
**OrderItemOptionValue** | **String** | Ordered product option value Where x is order item ID, y - order item option ID | [optional] 
**OrderItemOptionPrice** | **Decimal** | Ordered product option price Where x is order item ID, y - order item option ID | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderAddOrderItemInnerOrderItemOptionInner = Initialize-PSOpenAPIToolsOrderAddOrderItemInnerOrderItemOptionInner  -OrderItemOptionName Color `
 -OrderItemOptionValue green `
 -OrderItemOptionPrice 2.3
```

- Convert the resource to JSON
```powershell
$OrderAddOrderItemInnerOrderItemOptionInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

