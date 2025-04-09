# OrderPreestimateShippingListOrderItemInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderItemId** | **String** | Defines orders specified by order item id | 
**OrderItemModel** | **String** | Defines orders specified by order item model | [optional] 
**OrderItemQuantity** | **Int32** | Defines orders specified by order item quantity | 
**OrderItemWeight** | **Decimal** | Defines orders specified by order item weight | [optional] 
**OrderItemVariantId** | **String** | Ordered product variant. Where x is order item ID | [optional] 
**OrderItemOption** | [**OrderPreestimateShippingListOrderItemInnerOrderItemOptionInner[]**](OrderPreestimateShippingListOrderItemInnerOrderItemOptionInner.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderPreestimateShippingListOrderItemInner = Initialize-PSOpenAPIToolsOrderPreestimateShippingListOrderItemInner  -OrderItemId 125, where {x} - 1,2,3,... etc `
 -OrderItemModel sku_1, where {x} - 1,2,3,... etc `
 -OrderItemQuantity 5, where {x} - 1,2,3,... etc `
 -OrderItemWeight 5, where {x} - 1,2,3,... etc `
 -OrderItemVariantId 52 `
 -OrderItemOption null
```

- Convert the resource to JSON
```powershell
$OrderPreestimateShippingListOrderItemInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

