# Shipment
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**OrderId** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**WarehouseId** | **String** |  | [optional] 
**ShipmentProvider** | **String** |  | [optional] 
**TrackingNumbers** | [**ShipmentTrackingNumber[]**](ShipmentTrackingNumber.md) |  | [optional] 
**CreatedAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**ModifiedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**Items** | [**ShipmentItem[]**](ShipmentItem.md) |  | [optional] 
**IsShipped** | **Boolean** |  | [optional] 
**DeliveredAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Shipment = Initialize-PSOpenAPIToolsShipment  -Id null `
 -OrderId null `
 -Name null `
 -WarehouseId null `
 -ShipmentProvider null `
 -TrackingNumbers null `
 -CreatedAt null `
 -ModifiedTime null `
 -Items null `
 -IsShipped null `
 -DeliveredAt null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Shipment | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

