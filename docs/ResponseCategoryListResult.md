# ResponseCategoryListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CategoriesCount** | **Int32** |  | [optional] 
**Category** | [**Category[]**](Category.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseCategoryListResult = Initialize-PSOpenAPIToolsResponseCategoryListResult  -CategoriesCount null `
 -Category null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseCategoryListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

