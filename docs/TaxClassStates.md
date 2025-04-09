# TaxClassStates
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Tax** | **Decimal** |  | [optional] 
**TaxType** | **Int32** |  | [optional] 
**Name** | **String** |  | [optional] 
**Code** | **String** |  | [optional] 
**ZipCodes** | [**TaxClassZipCodes[]**](TaxClassZipCodes.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$TaxClassStates = Initialize-PSOpenAPIToolsTaxClassStates  -Id null `
 -Tax null `
 -TaxType null `
 -Name null `
 -Code null `
 -ZipCodes null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$TaxClassStates | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

