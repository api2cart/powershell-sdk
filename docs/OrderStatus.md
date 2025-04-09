# OrderStatus
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**History** | [**OrderStatusHistoryItem[]**](OrderStatusHistoryItem.md) |  | [optional] 
**RefundInfo** | [**OrderStatusRefund**](OrderStatusRefund.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderStatus = Initialize-PSOpenAPIToolsOrderStatus  -Id null `
 -Name null `
 -History null `
 -RefundInfo null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderStatus | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

