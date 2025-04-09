# ModelResponseCustomerAttributeList
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnCode** | **Int32** |  | [optional] 
**ReturnMessage** | **String** |  | [optional] 
**Pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**Result** | [**ResponseCustomerAttributeListResult**](ResponseCustomerAttributeListResult.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ModelResponseCustomerAttributeList = Initialize-PSOpenAPIToolsModelResponseCustomerAttributeList  -ReturnCode null `
 -ReturnMessage null `
 -Pagination null `
 -Result null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ModelResponseCustomerAttributeList | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

