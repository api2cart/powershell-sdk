# OrderTotals
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Total** | **Decimal** |  | [optional] 
**Subtotal** | **Decimal** |  | [optional] 
**Shipping** | **Decimal** |  | [optional] 
**Tax** | **Decimal** |  | [optional] 
**Discount** | **Decimal** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderTotals = Initialize-PSOpenAPIToolsOrderTotals  -Total null `
 -Subtotal null `
 -Shipping null `
 -Tax null `
 -Discount null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderTotals | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

