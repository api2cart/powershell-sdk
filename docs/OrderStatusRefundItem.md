# OrderStatusRefundItem
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProductId** | **String** |  | [optional] 
**VariantId** | **String** |  | [optional] 
**OrderProductId** | **String** |  | [optional] 
**Qty** | **Decimal** |  | [optional] 
**Refund** | **Decimal** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderStatusRefundItem = Initialize-PSOpenAPIToolsOrderStatusRefundItem  -ProductId null `
 -VariantId null `
 -OrderProductId null `
 -Qty null `
 -Refund null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderStatusRefundItem | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

