# CustomerWishListItem
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**ProductId** | **String** |  | [optional] 
**ChildId** | **String** |  | [optional] 
**CreatedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CustomerWishListItem = Initialize-PSOpenAPIToolsCustomerWishListItem  -Id null `
 -ProductId null `
 -ChildId null `
 -CreatedTime null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$CustomerWishListItem | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

