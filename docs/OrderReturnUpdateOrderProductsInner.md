# OrderReturnUpdateOrderProductsInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderProductId** | **String** | Defines which products from the order should be returned | 
**OrderProductQuantity** | **Int32** | Defines how many product units from the order should be returned | 
**OrderProductStatus** | **String** | Defines product return status | [optional] 
**OrderProductActionId** | **String** | Defines the ID of the return action | 

## Examples

- Prepare the resource
```powershell
$OrderReturnUpdateOrderProductsInner = Initialize-PSOpenAPIToolsOrderReturnUpdateOrderProductsInner  -OrderProductId 125, where {x} - 1,2,3,... etc `
 -OrderProductQuantity 1, where {x} - 1,2,3,... etc `
 -OrderProductStatus pending `
 -OrderProductActionId REFUND, where {x} - 1,2,3,... etc
```

- Convert the resource to JSON
```powershell
$OrderReturnUpdateOrderProductsInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

