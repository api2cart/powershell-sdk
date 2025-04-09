# ResponseCustomerWishlistListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TotalCount** | **Int32** |  | [optional] 
**WishLists** | [**CustomerWishList[]**](CustomerWishList.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseCustomerWishlistListResult = Initialize-PSOpenAPIToolsResponseCustomerWishlistListResult  -TotalCount null `
 -WishLists null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseCustomerWishlistListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

