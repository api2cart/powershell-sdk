# ResponseTaxClassInfoResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Avail** | **Boolean** |  | [optional] 
**Tax** | **Decimal** |  | [optional] 
**TaxType** | **Int32** |  | [optional] 
**CreatedAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**ModifiedAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**TaxRates** | [**TaxClassRate[]**](TaxClassRate.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseTaxClassInfoResult = Initialize-PSOpenAPIToolsResponseTaxClassInfoResult  -Id null `
 -Name null `
 -Avail null `
 -Tax null `
 -TaxType null `
 -CreatedAt null `
 -ModifiedAt null `
 -TaxRates null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseTaxClassInfoResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

