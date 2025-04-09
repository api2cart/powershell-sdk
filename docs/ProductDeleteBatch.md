# ProductDeleteBatch
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Payload** | [**ProductDeleteBatchPayloadInner[]**](ProductDeleteBatchPayloadInner.md) | Contains an array of product deletion requests, each including the product ID. | 

## Examples

- Prepare the resource
```powershell
$ProductDeleteBatch = Initialize-PSOpenAPIToolsProductDeleteBatch  -Payload null
```

- Convert the resource to JSON
```powershell
$ProductDeleteBatch | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

