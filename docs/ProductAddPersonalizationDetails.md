# ProductAddPersonalizationDetails
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**IsPersonalizable** | **Boolean** |  | 
**PersonalizationIsRequired** | **Boolean** |  | [optional] 
**PersonalizationCharCountMax** | **Int32** |  | [optional] 
**PersonalizationInstructions** | **String** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAddPersonalizationDetails = Initialize-PSOpenAPIToolsProductAddPersonalizationDetails  -IsPersonalizable null `
 -PersonalizationIsRequired null `
 -PersonalizationCharCountMax null `
 -PersonalizationInstructions null
```

- Convert the resource to JSON
```powershell
$ProductAddPersonalizationDetails | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

