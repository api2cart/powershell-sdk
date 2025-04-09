# OrderShipmentAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderId** | **String** | Defines the order for which the shipment will be created | [optional] 
**StoreId** | **String** | Store Id | [optional] 
**WarehouseId** | **String** | This parameter is used for selecting a warehouse where you need to set/modify a product quantity. | [optional] 
**ShipmentProvider** | **String** | Defines company name that provide tracking of shipment | [optional] 
**ShippingMethod** | **String** | Define shipping method | [optional] 
**Items** | [**OrderShipmentAddItemsInner[]**](OrderShipmentAddItemsInner.md) | Defines items in the order that will be shipped | [optional] 
**SendNotifications** | **Boolean** | Send notifications to customer after shipment was created | [optional] [default to $false]
**TrackingNumbers** | [**OrderShipmentAddTrackingNumbersInner[]**](OrderShipmentAddTrackingNumbersInner.md) | Defines shipment&#39;s tracking numbers that have to be added&lt;/br&gt; How set tracking numbers to appropriate carrier:&lt;ul&gt;&lt;li&gt;tracking_numbers[]&#x3D;a2c.demo1,a2c.demo2 - set default carrier&lt;/li&gt;&lt;li&gt;tracking_numbers[&lt;b&gt;carrier_id&lt;/b&gt;]&#x3D;a2c.demo - set appropriate carrier&lt;/li&gt;&lt;/ul&gt;To get the list of carriers IDs that are available in your store, use the &lt;a href &#x3D; &quot;&quot;https://api2cart.com/docs/#/cart/CartInfo&quot;&quot;&gt;cart.info&lt;/a &gt; method | [optional] 
**AdjustStock** | **Boolean** | This parameter is used for adjust stock. | [optional] [default to $false]
**EnableCache** | **Boolean** | If the value is &#39;true&#39; and order exist in our cache, we will use order.info from cache to prepare shipment items. | [optional] [default to $false]
**TrackingLink** | **String** | Defines custom tracking link | [optional] 
**IsShipped** | **Boolean** | Defines shipment&#39;s status | [optional] [default to $true]
**CheckProcessStatus** | **Boolean** | Disable or enable check process status. Please note that the response will be slower due to additional requests to the store. | [optional] [default to $false]
**UseLatestApiVersion** | **Boolean** | Use the latest platform API version | [optional] [default to $false]

## Examples

- Prepare the resource
```powershell
$OrderShipmentAdd = Initialize-PSOpenAPIToolsOrderShipmentAdd  -OrderId 25 `
 -StoreId 1 `
 -WarehouseId 1 `
 -ShipmentProvider UPS `
 -ShippingMethod flatrate_flatrate `
 -Items null `
 -SendNotifications true `
 -TrackingNumbers null `
 -AdjustStock true `
 -EnableCache true `
 -TrackingLink http://example.com?someParam&#x3D;value `
 -IsShipped true `
 -CheckProcessStatus false `
 -UseLatestApiVersion true
```

- Convert the resource to JSON
```powershell
$OrderShipmentAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

