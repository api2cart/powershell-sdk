# ProductGroupItem
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ChildItemId** | **String** |  | [optional] 
**ProductId** | **String** |  | [optional] 
**DefaultQtyInPack** | **String** |  | [optional] 
**IsQtyInPackFixed** | **Boolean** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductGroupItem = Initialize-PSOpenAPIToolsProductGroupItem  -ChildItemId null `
 -ProductId null `
 -DefaultQtyInPack null `
 -IsQtyInPackFixed null `
 -Price null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ProductGroupItem | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

