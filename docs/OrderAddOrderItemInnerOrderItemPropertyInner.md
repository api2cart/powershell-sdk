# OrderAddOrderItemInnerOrderItemPropertyInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderItemPropertyName** | **String** | Ordered product property name. Where x is order item ID, y is order item property ID | [optional] 
**OrderItemPropertyValue** | **String** | Ordered product property value. Where x is order item ID, y - order item property ID | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderAddOrderItemInnerOrderItemPropertyInner = Initialize-PSOpenAPIToolsOrderAddOrderItemInnerOrderItemPropertyInner  -OrderItemPropertyName Engraving `
 -OrderItemPropertyValue lorem ipsum
```

- Convert the resource to JSON
```powershell
$OrderAddOrderItemInnerOrderItemPropertyInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

