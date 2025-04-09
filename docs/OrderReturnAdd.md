# OrderReturnAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderId** | **String** | Defines the order id | [optional] 
**StoreId** | **String** | Store Id | [optional] 
**ReturnStatusId** | **String** | Defines return request status | 
**ReturnActionId** | **String** | Defines return request action | 
**ReturnReasonId** | **String** | Defines return request reason | 
**ReturnReason** | **String** | Defines return request reason | [optional] 
**ItemRestock** | **Boolean** | Boolean, whether or not to add the line items back to the store inventory. | [optional] [default to $false]
**StaffNote** | **String** | Specifies staff note | [optional] 
**Comment** | **String** | Specifies return comment | [optional] 
**SendNotifications** | **Boolean** | Send notifications to customer after order was created | [optional] [default to $false]
**RejectReason** | **String** | Defines return reject reason | [optional] 
**OrderProducts** | [**OrderReturnAddOrderProductsInner[]**](OrderReturnAddOrderProductsInner.md) |  | 

## Examples

- Prepare the resource
```powershell
$OrderReturnAdd = Initialize-PSOpenAPIToolsOrderReturnAdd  -OrderId 25 `
 -StoreId 1 `
 -ReturnStatusId RETURNED `
 -ReturnActionId RETURNED `
 -ReturnReasonId broken `
 -ReturnReason broken `
 -ItemRestock true `
 -StaffNote Test `
 -Comment This coole order `
 -SendNotifications true `
 -RejectReason ORDER_UNPAID `
 -OrderProducts null
```

- Convert the resource to JSON
```powershell
$OrderReturnAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

