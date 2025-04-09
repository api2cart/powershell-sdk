# ResponseProductListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProductsCount** | **Int32** |  | [optional] 
**Product** | [**Product[]**](Product.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseProductListResult = Initialize-PSOpenAPIToolsResponseProductListResult  -ProductsCount null `
 -Product null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseProductListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

