# ResponseCartScriptListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TotalCount** | **Int32** |  | [optional] 
**Scripts** | [**Script[]**](Script.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseCartScriptListResult = Initialize-PSOpenAPIToolsResponseCartScriptListResult  -TotalCount null `
 -Scripts null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseCartScriptListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

