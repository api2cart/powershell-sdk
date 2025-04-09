# CartShippingMethodRate
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**MinWeight** | **String** |  | [optional] 
**MaxWeight** | **String** |  | [optional] 
**MinOrderAmount** | **String** |  | [optional] 
**MaxOrderAmount** | **String** |  | [optional] 
**MinItemsCount** | **String** |  | [optional] 
**MaxItemsCount** | **String** |  | [optional] 
**Price** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CartShippingMethodRate = Initialize-PSOpenAPIToolsCartShippingMethodRate  -MinWeight null `
 -MaxWeight null `
 -MinOrderAmount null `
 -MaxOrderAmount null `
 -MinItemsCount null `
 -MaxItemsCount null `
 -Price null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$CartShippingMethodRate | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

