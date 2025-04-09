# OrderReturnUpdate
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnId** | **String** | Return ID | 
**OrderId** | **String** | Defines the order id | [optional] 
**StoreId** | **String** | Store Id | [optional] 
**ItemRestock** | **Boolean** | Boolean, whether or not to add the line items back to the store inventory. | [optional] [default to $false]
**ReturnStatusId** | **String** | Defines return request status | [optional] 
**StaffNote** | **String** | Specifies staff note | [optional] 
**Comment** | **String** | Specifies return comment | [optional] 
**SendNotifications** | **Boolean** | Send notifications to customer after order was created | [optional] [default to $false]
**RejectReason** | **String** | Defines return reject reason | [optional] 
**OrderProducts** | [**OrderReturnUpdateOrderProductsInner[]**](OrderReturnUpdateOrderProductsInner.md) |  | 

## Examples

- Prepare the resource
```powershell
$OrderReturnUpdate = Initialize-PSOpenAPIToolsOrderReturnUpdate  -ReturnId 200000002 `
 -OrderId 25 `
 -StoreId 1 `
 -ItemRestock true `
 -ReturnStatusId RETURNED `
 -StaffNote Test `
 -Comment This coole order `
 -SendNotifications true `
 -RejectReason ORDER_UNPAID `
 -OrderProducts null
```

- Convert the resource to JSON
```powershell
$OrderReturnUpdate | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

