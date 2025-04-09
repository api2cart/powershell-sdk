# ModelReturn
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**OrderId** | **String** |  | [optional] 
**CustomerId** | **String** |  | [optional] 
**StoreId** | **String** |  | [optional] 
**CreatedAt** | **String** |  | [optional] 
**ModifiedAt** | **String** |  | [optional] 
**Status** | [**ReturnStatus**](ReturnStatus.md) |  | [optional] 
**OrderProducts** | [**ReturnOrderProduct[]**](ReturnOrderProduct.md) |  | [optional] 
**Comment** | **String** |  | [optional] 
**StaffNote** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ModelReturn = Initialize-PSOpenAPIToolsModelReturn  -Id null `
 -Name null `
 -OrderId null `
 -CustomerId null `
 -StoreId null `
 -CreatedAt null `
 -ModifiedAt null `
 -Status null `
 -OrderProducts null `
 -Comment null `
 -StaffNote null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ModelReturn | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

