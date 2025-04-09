# CartShippingZone2
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Enabled** | **Boolean** |  | [optional] 
**Countries** | [**Country[]**](Country.md) |  | [optional] 
**ShippingMethods** | [**CartShippingMethod[]**](CartShippingMethod.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CartShippingZone2 = Initialize-PSOpenAPIToolsCartShippingZone2  -Id null `
 -Name null `
 -Enabled null `
 -Countries null `
 -ShippingMethods null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$CartShippingZone2 | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

