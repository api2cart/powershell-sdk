# BatchJobResultItem
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **Int32** |  | [optional] 
**Status** | **String** |  | [optional] 
**EntityId** | **String** |  | [optional] 
**Errors** | **String[]** |  | [optional] 
**Warnings** | **String[]** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$BatchJobResultItem = Initialize-PSOpenAPIToolsBatchJobResultItem  -Id null `
 -Status null `
 -EntityId null `
 -Errors null `
 -Warnings null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$BatchJobResultItem | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

