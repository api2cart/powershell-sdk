# ResponseCustomerGroupListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**GroupCount** | **Int32** |  | [optional] 
**Group** | [**CustomerGroup[]**](CustomerGroup.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseCustomerGroupListResult = Initialize-PSOpenAPIToolsResponseCustomerGroupListResult  -GroupCount null `
 -Group null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseCustomerGroupListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

