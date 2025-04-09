# OrderStatusRefund
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Shipping** | **Decimal** |  | [optional] 
**Fee** | **Decimal** |  | [optional] 
**Tax** | **Decimal** |  | [optional] 
**TotalRefunded** | **Decimal** |  | [optional] 
**Time** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**Comment** | **String** |  | [optional] 
**RefundedItems** | [**OrderStatusRefundItem[]**](OrderStatusRefundItem.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderStatusRefund = Initialize-PSOpenAPIToolsOrderStatusRefund  -Shipping null `
 -Fee null `
 -Tax null `
 -TotalRefunded null `
 -Time null `
 -Comment null `
 -RefundedItems null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderStatusRefund | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

