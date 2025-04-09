# ModelResponseCustomerWishlistList
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnCode** | **Int32** |  | [optional] 
**ReturnMessage** | **String** |  | [optional] 
**Pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**Result** | [**ResponseCustomerWishlistListResult**](ResponseCustomerWishlistListResult.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ModelResponseCustomerWishlistList = Initialize-PSOpenAPIToolsModelResponseCustomerWishlistList  -ReturnCode null `
 -ReturnMessage null `
 -Pagination null `
 -Result null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ModelResponseCustomerWishlistList | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

