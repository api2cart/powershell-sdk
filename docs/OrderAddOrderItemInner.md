# OrderAddOrderItemInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderItemId** | **String** | Defines orders specified by order item id | 
**OrderItemName** | **String** | Defines orders specified by order item name | 
**OrderItemModel** | **String** | Defines orders specified by order item model | [optional] 
**OrderItemPrice** | **Decimal** | Defines orders specified by order item price | 
**OrderItemQuantity** | **Int32** | Defines orders specified by order item quantity | 
**OrderItemWeight** | **Decimal** | Defines orders specified by order item weight | [optional] 
**OrderItemVariantId** | **String** | Ordered product variant. Where x is order item ID | [optional] 
**OrderItemTax** | **Decimal** | Percentage of tax for product order | [optional] [default to 0]
**OrderItemPriceIncludesTax** | **Boolean** | Defines if item price includes tax | [optional] [default to $false]
**OrderItemParent** | **Int32** | Index of the parent grouped/bundle product | [optional] 
**OrderItemParentOptionName** | **String** | Option name of the parent grouped/bundle product | [optional] 
**OrderItemAllowRefundItemsSeparately** | **Boolean** | Indicates whether subitems of the grouped/bundle product can be refunded separately | [optional] 
**OrderItemAllowShipItemsSeparately** | **Boolean** | Indicates whether subitems of the grouped/bundle product can be shipped separately | [optional] 
**OrderItemOption** | [**OrderAddOrderItemInnerOrderItemOptionInner[]**](OrderAddOrderItemInnerOrderItemOptionInner.md) |  | [optional] 
**OrderItemProperty** | [**OrderAddOrderItemInnerOrderItemPropertyInner[]**](OrderAddOrderItemInnerOrderItemPropertyInner.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderAddOrderItemInner = Initialize-PSOpenAPIToolsOrderAddOrderItemInner  -OrderItemId 125, where {x} - 1,2,3,... etc `
 -OrderItemName Product 1, where {x} - 1,2,3,... etc `
 -OrderItemModel sku_1, where {x} - 1,2,3,... etc `
 -OrderItemPrice 1.32, where {x} - 1,2,3,... etc `
 -OrderItemQuantity 5, where {x} - 1,2,3,... etc `
 -OrderItemWeight 5, where {x} - 1,2,3,... etc `
 -OrderItemVariantId 52 `
 -OrderItemTax 5.5 `
 -OrderItemPriceIncludesTax null `
 -OrderItemParent 2 `
 -OrderItemParentOptionName Internal Memory Storage `
 -OrderItemAllowRefundItemsSeparately true `
 -OrderItemAllowShipItemsSeparately true `
 -OrderItemOption null `
 -OrderItemProperty null
```

- Convert the resource to JSON
```powershell
$OrderAddOrderItemInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

