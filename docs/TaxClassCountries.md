# TaxClassCountries
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Code** | **String** |  | [optional] 
**Tax** | **Decimal** |  | [optional] 
**TaxType** | **Int32** |  | [optional] 
**States** | [**TaxClassStates[]**](TaxClassStates.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$TaxClassCountries = Initialize-PSOpenAPIToolsTaxClassCountries  -Id null `
 -Name null `
 -Code null `
 -Tax null `
 -TaxType null `
 -States null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$TaxClassCountries | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

