# OrderCalculateOrderItemInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderItemId** | **String** | Defines orders specified by order item id | 
**OrderItemQuantity** | **Int32** | Defines orders specified by order item quantity | 
**OrderItemVariantId** | **String** | Ordered product variant. Where x is order item ID | [optional] 
**OrderItemParent** | **Int32** | Index of the parent grouped/bundle product | [optional] 
**OrderItemParentOptionName** | **String** | Option name of the parent grouped/bundle product | [optional] 
**OrderItemOption** | [**OrderCalculateOrderItemInnerOrderItemOptionInner[]**](OrderCalculateOrderItemInnerOrderItemOptionInner.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderCalculateOrderItemInner = Initialize-PSOpenAPIToolsOrderCalculateOrderItemInner  -OrderItemId 125, where {x} - 1,2,3,... etc `
 -OrderItemQuantity 5, where {x} - 1,2,3,... etc `
 -OrderItemVariantId 52 `
 -OrderItemParent 2 `
 -OrderItemParentOptionName Internal Memory Storage `
 -OrderItemOption null
```

- Convert the resource to JSON
```powershell
$OrderCalculateOrderItemInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

