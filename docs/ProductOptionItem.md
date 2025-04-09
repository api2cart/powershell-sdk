# ProductOptionItem
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**ProductOptionItemId** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**SortOrder** | **Int32** |  | [optional] 
**Price** | **String** |  | [optional] 
**Weight** | **String** |  | [optional] 
**Quantity** | **Int32** |  | [optional] 
**TypePrice** | **String** |  | [optional] 
**Sku** | **String** |  | [optional] 
**IsDefault** | **Boolean** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductOptionItem = Initialize-PSOpenAPIToolsProductOptionItem  -Id null `
 -ProductOptionItemId null `
 -Name null `
 -SortOrder null `
 -Price null `
 -Weight null `
 -Quantity null `
 -TypePrice null `
 -Sku null `
 -IsDefault null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ProductOptionItem | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

