# OrderShipmentUpdate
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ShipmentId** | **String** | Shipment id indicates the number of delivery | 
**OrderId** | **String** | Defines the order that will be updated | [optional] 
**StoreId** | **String** | Store Id | [optional] 
**ShipmentProvider** | **String** | Defines company name that provide tracking of shipment | [optional] 
**TrackingNumbers** | [**OrderShipmentAddTrackingNumbersInner[]**](OrderShipmentAddTrackingNumbersInner.md) | Defines shipment&#39;s tracking numbers that have to be added&lt;/br&gt; How set tracking numbers to appropriate carrier:&lt;ul&gt;&lt;li&gt;tracking_numbers[]&#x3D;a2c.demo1,a2c.demo2 - set default carrier&lt;/li&gt;&lt;li&gt;tracking_numbers[&lt;b&gt;carrier_id&lt;/b&gt;]&#x3D;a2c.demo - set appropriate carrier&lt;/li&gt;&lt;/ul&gt;To get the list of carriers IDs that are available in your store, use the &lt;a href &#x3D; &quot;&quot;https://api2cart.com/docs/#/cart/CartInfo&quot;&quot;&gt;cart.info&lt;/a &gt; method | [optional] 
**TrackingLink** | **String** | Defines custom tracking link | [optional] 
**IsShipped** | **Boolean** | Defines shipment&#39;s status | [optional] [default to $true]
**DeliveredAt** | **String** | Defines the date of delivery | [optional] 
**Replace** | **Boolean** | Allows rewrite tracking numbers | [optional] [default to $true]
**SendNotifications** | **Boolean** | Send notifications to customer after order was created | [optional] [default to $false]
**TrackingProvider** | **String** | Defines name of the company which provides shipment tracking | [optional] 
**Items** | [**OrderShipmentAddItemsInner[]**](OrderShipmentAddItemsInner.md) | Defines items in the order that will be shipped | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderShipmentUpdate = Initialize-PSOpenAPIToolsOrderShipmentUpdate  -ShipmentId 200000002 `
 -OrderId 25 `
 -StoreId 1 `
 -ShipmentProvider UPS `
 -TrackingNumbers null `
 -TrackingLink http://example.com?someParam&#x3D;value `
 -IsShipped true `
 -DeliveredAt 2024-08-25T23:56:12+00:00 `
 -Replace false `
 -SendNotifications true `
 -TrackingProvider Custom tracker `
 -Items null
```

- Convert the resource to JSON
```powershell
$OrderShipmentUpdate | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

