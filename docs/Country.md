# Country
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code2** | **String** |  | [optional] 
**Code3** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Country = Initialize-PSOpenAPIToolsCountry  -Code2 null `
 -Code3 null `
 -Name null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Country | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

