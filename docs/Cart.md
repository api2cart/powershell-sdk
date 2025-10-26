# Cart
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **String** |  | [optional] 
**Url** | **String** |  | [optional] 
**Version** | **String** |  | [optional] 
**BridgeVersion** | **String** |  | [optional] 
**DefaultRoundingPrecision** | **Int32** |  | [optional] 
**DbPrefix** | **String** |  | [optional] 
**StoresInfo** | [**CartStoreInfo[]**](CartStoreInfo.md) |  | [optional] 
**Warehouses** | [**CartWarehouse[]**](CartWarehouse.md) |  | [optional] 
**ShippingZones** | [**CartShippingZone[]**](CartShippingZone.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Cart = Initialize-PSOpenAPIToolsCart  -Name null `
 -Url null `
 -Version null `
 -BridgeVersion null `
 -DefaultRoundingPrecision null `
 -DbPrefix null `
 -StoresInfo null `
 -Warehouses null `
 -ShippingZones null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Cart | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

