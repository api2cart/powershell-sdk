# OrderReturnAddOrderProductsInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderProductId** | **String** | Defines which products from the order should be returned | 
**OrderProductQuantity** | **Int32** | Defines how many product units from the order should be returned | 
**OrderProductReasonId** | **String** | Defines the ID of the return reason | 
**OrderProductActionId** | **String** | Defines the ID of the return action | 
**OrderProductCustomerComment** | **String** | Defines the customer&#39;s comment for return | [optional] 
**OrderProductHandlingStatus** | **String** | Defines handling status | [optional] 
**OrderProductCondition** | **String** | Defines the product condition | [optional] 
**OrderProductReason** | **String** | Defines return reason | [optional] 
**OrderProductStatus** | **String** | Defines product return status | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderReturnAddOrderProductsInner = Initialize-PSOpenAPIToolsOrderReturnAddOrderProductsInner  -OrderProductId 125, where {x} - 1,2,3,... etc `
 -OrderProductQuantity 1, where {x} - 1,2,3,... etc `
 -OrderProductReasonId DEFECTIVE, where {x} - 1,2,3,... etc `
 -OrderProductActionId REFUND, where {x} - 1,2,3,... etc `
 -OrderProductCustomerComment I need a bigger size, where {x} - 1,2,3,... etc `
 -OrderProductHandlingStatus 123456 `
 -OrderProductCondition Broken, where {x} - 1,2,3,... etc `
 -OrderProductReason 123456 `
 -OrderProductStatus pending
```

- Convert the resource to JSON
```powershell
$OrderReturnAddOrderProductsInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

