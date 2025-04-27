# OrderShipmentTrackingAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderId** | **String** | Defines the order id | [optional] 
**ShipmentId** | **String** | Shipment id indicates the number of delivery | 
**CarrierId** | **String** | Defines tracking carrier id | [optional] 
**StoreId** | **String** | Store Id | [optional] 
**TrackingProvider** | **String** | Defines name of the company which provides shipment tracking | [optional] 
**TrackingNumber** | **String** | Defines tracking number | 
**TrackingLink** | **String** | Defines custom tracking link | [optional] 
**SendNotifications** | **Boolean** | Send notifications to customer after tracking was created | [optional] [default to $false]

## Examples

- Prepare the resource
```powershell
$OrderShipmentTrackingAdd = Initialize-PSOpenAPIToolsOrderShipmentTrackingAdd  -OrderId 25 `
 -ShipmentId 200000002 `
 -CarrierId USPS `
 -StoreId 1 `
 -TrackingProvider Custom tracker `
 -TrackingNumber 1А6745 `
 -TrackingLink http://example.com?someParam&#x3D;value `
 -SendNotifications true
```

- Convert the resource to JSON
```powershell
$OrderShipmentTrackingAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

