# TaxClassRate
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Tax** | **Decimal** |  | [optional] 
**TaxType** | **Int32** |  | [optional] 
**TaxBasedOn** | **String** |  | [optional] 
**Countries** | [**TaxClassCountries[]**](TaxClassCountries.md) |  | [optional] 
**Cities** | **String[]** |  | [optional] 
**Address** | **String[]** |  | [optional] 
**ZipCodes** | [**TaxClassZipCodes[]**](TaxClassZipCodes.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$TaxClassRate = Initialize-PSOpenAPIToolsTaxClassRate  -Id null `
 -Name null `
 -Tax null `
 -TaxType null `
 -TaxBasedOn null `
 -Countries null `
 -Cities null `
 -Address null `
 -ZipCodes null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$TaxClassRate | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

