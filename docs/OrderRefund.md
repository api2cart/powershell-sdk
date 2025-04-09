# OrderRefund
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Shipping** | **Decimal** |  | [optional] 
**Fee** | **Decimal** |  | [optional] 
**Tax** | **Decimal** |  | [optional] 
**Total** | **Decimal** |  | [optional] 
**ModifiedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**Comment** | **String** |  | [optional] 
**Items** | [**OrderStatusRefundItem[]**](OrderStatusRefundItem.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderRefund = Initialize-PSOpenAPIToolsOrderRefund  -Id null `
 -Shipping null `
 -Fee null `
 -Tax null `
 -Total null `
 -ModifiedTime null `
 -Comment null `
 -Items null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderRefund | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

