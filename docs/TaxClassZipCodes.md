# TaxClassZipCodes
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**IsRange** | **Boolean** |  | [optional] 
**Range** | **String[]** |  | [optional] 
**Fields** | [**TaxClassZipCodesRange[]**](TaxClassZipCodesRange.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$TaxClassZipCodes = Initialize-PSOpenAPIToolsTaxClassZipCodes  -IsRange null `
 -Range null `
 -Fields null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$TaxClassZipCodes | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

