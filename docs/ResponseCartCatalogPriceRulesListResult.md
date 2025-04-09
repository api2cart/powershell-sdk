# ResponseCartCatalogPriceRulesListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CatalogPriceRulesCount** | **Int32** |  | [optional] 
**CatalogPriceRules** | [**CatalogPriceRule[]**](CatalogPriceRule.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseCartCatalogPriceRulesListResult = Initialize-PSOpenAPIToolsResponseCartCatalogPriceRulesListResult  -CatalogPriceRulesCount null `
 -CatalogPriceRules null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseCartCatalogPriceRulesListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

