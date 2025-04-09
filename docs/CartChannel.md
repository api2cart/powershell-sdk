# CartChannel
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Platform** | **String** |  | [optional] 
**IsEnabled** | **Boolean** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CartChannel = Initialize-PSOpenAPIToolsCartChannel  -Id null `
 -Name null `
 -Platform null `
 -IsEnabled null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$CartChannel | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

