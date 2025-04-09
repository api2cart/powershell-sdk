# ResponseOrderAbandonedListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Order** | [**OrderAbandoned[]**](OrderAbandoned.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseOrderAbandonedListResult = Initialize-PSOpenAPIToolsResponseOrderAbandonedListResult  -Order null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseOrderAbandonedListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

