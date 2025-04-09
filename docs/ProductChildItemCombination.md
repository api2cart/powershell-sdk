# ProductChildItemCombination
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OptionId** | **String** |  | [optional] 
**OptionValueId** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductChildItemCombination = Initialize-PSOpenAPIToolsProductChildItemCombination  -OptionId null `
 -OptionValueId null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ProductChildItemCombination | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

