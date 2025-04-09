# OrderRefundAddItemsInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderProductId** | **String** |  | [optional] 
**Quantity** | **Int32** |  | [optional] 
**Price** | **Decimal** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderRefundAddItemsInner = Initialize-PSOpenAPIToolsOrderRefundAddItemsInner  -OrderProductId null `
 -Quantity null `
 -Price null
```

- Convert the resource to JSON
```powershell
$OrderRefundAddItemsInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

