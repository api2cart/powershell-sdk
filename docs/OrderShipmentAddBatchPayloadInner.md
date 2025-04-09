# OrderShipmentAddBatchPayloadInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderId** | **String** |  | 
**StoreId** | **String** |  | [optional] 
**WarehouseId** | **String** |  | [optional] 
**CarrierId** | **String** |  | [optional] 
**CarrierName** | **String** |  | [optional] 
**TrackingNumber** | **String** |  | 
**TrackingLink** | **String** |  | [optional] 
**ShipmentProvider** | **String** |  | [optional] 
**Items** | [**OrderShipmentAddBatchPayloadInnerItemsInner[]**](OrderShipmentAddBatchPayloadInnerItemsInner.md) |  | [optional] 
**SendNotifications** | **Boolean** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderShipmentAddBatchPayloadInner = Initialize-PSOpenAPIToolsOrderShipmentAddBatchPayloadInner  -OrderId null `
 -StoreId null `
 -WarehouseId null `
 -CarrierId null `
 -CarrierName null `
 -TrackingNumber null `
 -TrackingLink null `
 -ShipmentProvider null `
 -Items null `
 -SendNotifications null
```

- Convert the resource to JSON
```powershell
$OrderShipmentAddBatchPayloadInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

