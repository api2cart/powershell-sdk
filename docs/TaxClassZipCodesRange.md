# TaxClassZipCodesRange
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**VarFrom** | **String** |  | [optional] 
**To** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$TaxClassZipCodesRange = Initialize-PSOpenAPIToolsTaxClassZipCodesRange  -VarFrom null `
 -To null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$TaxClassZipCodesRange | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

