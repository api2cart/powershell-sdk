# ProductOption
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**ProductOptionId** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Description** | **String** |  | [optional] 
**SortOrder** | **Int32** |  | [optional] 
**Type** | **String** |  | [optional] 
**Required** | **Boolean** |  | [optional] 
**Available** | **Boolean** |  | [optional] 
**UsedInCombination** | **Boolean** |  | [optional] 
**OptionItems** | [**ProductOptionItem[]**](ProductOptionItem.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductOption = Initialize-PSOpenAPIToolsProductOption  -Id null `
 -ProductOptionId null `
 -Name null `
 -Description null `
 -SortOrder null `
 -Type null `
 -Required null `
 -Available null `
 -UsedInCombination null `
 -OptionItems null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ProductOption | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

