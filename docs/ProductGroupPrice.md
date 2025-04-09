# ProductGroupPrice
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**GroupId** | **String** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**StoreId** | **String** |  | [optional] 
**Quantity** | **Decimal** |  | [optional] 
**StartTime** | **String** |  | [optional] 
**ExpireTime** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductGroupPrice = Initialize-PSOpenAPIToolsProductGroupPrice  -Id null `
 -GroupId null `
 -Price null `
 -StoreId null `
 -Quantity null `
 -StartTime null `
 -ExpireTime null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ProductGroupPrice | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

