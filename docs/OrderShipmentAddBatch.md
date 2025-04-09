# OrderShipmentAddBatch
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Payload** | [**OrderShipmentAddBatchPayloadInner[]**](OrderShipmentAddBatchPayloadInner.md) | Contains an array of order shipment objects. The list of properties may vary depending on the specific platform. | 

## Examples

- Prepare the resource
```powershell
$OrderShipmentAddBatch = Initialize-PSOpenAPIToolsOrderShipmentAddBatch  -Payload null
```

- Convert the resource to JSON
```powershell
$OrderShipmentAddBatch | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

