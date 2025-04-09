# ProductTierPrice
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Qty** | **Decimal** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductTierPrice = Initialize-PSOpenAPIToolsProductTierPrice  -Qty null `
 -Price null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ProductTierPrice | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

