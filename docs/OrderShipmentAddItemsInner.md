# OrderShipmentAddItemsInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderProductId** | **String** |  | [optional] 
**Quantity** | **Decimal** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderShipmentAddItemsInner = Initialize-PSOpenAPIToolsOrderShipmentAddItemsInner  -OrderProductId null `
 -Quantity null
```

- Convert the resource to JSON
```powershell
$OrderShipmentAddItemsInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

