# SpecialPrice
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Value** | **Decimal** |  | [optional] 
**Avail** | **Boolean** |  | [optional] 
**CreatedAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**ModifiedAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**ExpiredAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$SpecialPrice = Initialize-PSOpenAPIToolsSpecialPrice  -Value null `
 -Avail null `
 -CreatedAt null `
 -ModifiedAt null `
 -ExpiredAt null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$SpecialPrice | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

