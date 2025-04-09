# OrderRefundAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderId** | **String** | Defines the order for which the refund will be created. | [optional] 
**Items** | [**OrderRefundAddItemsInner[]**](OrderRefundAddItemsInner.md) | Defines items in the order that will be refunded | [optional] 
**TotalPrice** | **Decimal** | Defines order refund amount. | [optional] 
**ShippingPrice** | **Decimal** | Defines refund shipping amount. | [optional] 
**FeePrice** | **Decimal** | Specifies refund&#39;s fee price | [optional] 
**Message** | **String** | Refund reason, or some else message which assigned to refund. | [optional] 
**ItemRestock** | **Boolean** | Boolean, whether or not to add the line items back to the store inventory. | [optional] [default to $false]
**SendNotifications** | **Boolean** | Send notifications to customer after refund was created | [optional] [default to $false]
**Date** | **String** | Specifies an order creation date in format Y-m-d H:i:s | [optional] 
**IsOnline** | **Boolean** | Indicates whether refund type is online | [optional] [default to $false]

## Examples

- Prepare the resource
```powershell
$OrderRefundAdd = Initialize-PSOpenAPIToolsOrderRefundAdd  -OrderId 25 `
 -Items null `
 -TotalPrice 23.56 `
 -ShippingPrice 5.5 `
 -FeePrice 5.5 `
 -Message Received item is not like in the photo, get my money back. `
 -ItemRestock true `
 -SendNotifications true `
 -Date 2012-09-25 19:40:00 `
 -IsOnline false
```

- Convert the resource to JSON
```powershell
$OrderRefundAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

