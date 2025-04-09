# CartWarehouse
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Description** | **String** |  | [optional] 
**Avail** | **Boolean** |  | [optional] 
**Address** | [**CustomerAddress**](CustomerAddress.md) |  | [optional] 
**CarriersIds** | **String[]** |  | [optional] 
**StoresIds** | **String[]** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CartWarehouse = Initialize-PSOpenAPIToolsCartWarehouse  -Id null `
 -Name null `
 -Description null `
 -Avail null `
 -Address null `
 -CarriersIds null `
 -StoresIds null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$CartWarehouse | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

