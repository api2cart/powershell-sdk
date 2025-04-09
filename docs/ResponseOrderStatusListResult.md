# ResponseOrderStatusListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CartOrderStatuses** | [**Status[]**](Status.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseOrderStatusListResult = Initialize-PSOpenAPIToolsResponseOrderStatusListResult  -CartOrderStatuses null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseOrderStatusListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

