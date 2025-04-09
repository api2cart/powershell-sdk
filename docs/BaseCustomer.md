# BaseCustomer
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Email** | **String** |  | [optional] 
**FirstName** | **String** |  | [optional] 
**LastName** | **String** |  | [optional] 
**Phone** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$BaseCustomer = Initialize-PSOpenAPIToolsBaseCustomer  -Id null `
 -Email null `
 -FirstName null `
 -LastName null `
 -Phone null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$BaseCustomer | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

