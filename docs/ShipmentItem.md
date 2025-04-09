# ShipmentItem
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderProductId** | **String** |  | [optional] 
**ProductId** | **String** |  | [optional] 
**VariantId** | **String** |  | [optional] 
**Model** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**Quantity** | **Decimal** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ShipmentItem = Initialize-PSOpenAPIToolsShipmentItem  -OrderProductId null `
 -ProductId null `
 -VariantId null `
 -Model null `
 -Name null `
 -Price null `
 -Quantity null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ShipmentItem | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

