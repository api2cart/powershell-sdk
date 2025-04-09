# BatchJobResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**JobId** | **Int32** |  | [optional] 
**JobName** | **String** |  | [optional] 
**ItemsProcessed** | **Int32** |  | [optional] 
**ItemsSucceed** | **Int32** |  | [optional] 
**Items** | [**BatchJobResultItem[]**](BatchJobResultItem.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$BatchJobResult = Initialize-PSOpenAPIToolsBatchJobResult  -JobId null `
 -JobName null `
 -ItemsProcessed null `
 -ItemsSucceed null `
 -Items null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$BatchJobResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

