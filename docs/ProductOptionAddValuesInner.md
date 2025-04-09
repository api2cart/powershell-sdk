# ProductOptionAddValuesInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Value** | **String** |  | 
**DisplayValue** | **String** |  | [optional] 
**IsDefault** | **Boolean** |  | [optional] [default to $false]

## Examples

- Prepare the resource
```powershell
$ProductOptionAddValuesInner = Initialize-PSOpenAPIToolsProductOptionAddValuesInner  -Value null `
 -DisplayValue null `
 -IsDefault null
```

- Convert the resource to JSON
```powershell
$ProductOptionAddValuesInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

