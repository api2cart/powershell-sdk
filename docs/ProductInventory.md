# ProductInventory
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**WarehouseId** | **String** |  | [optional] 
**Quantity** | **Decimal** |  | [optional] 
**InStock** | **Boolean** |  | [optional] 
**Priority** | **Int32** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductInventory = Initialize-PSOpenAPIToolsProductInventory  -WarehouseId null `
 -Quantity null `
 -InStock null `
 -Priority null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ProductInventory | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

