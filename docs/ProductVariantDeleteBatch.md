# ProductVariantDeleteBatch
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ClearCache** | **Boolean** |  | [optional] [default to $false]
**Reindex** | **Boolean** |  | [optional] [default to $false]
**Payload** | [**ProductVariantDeleteBatchPayloadInner[]**](ProductVariantDeleteBatchPayloadInner.md) | Contains an array of product variant deletion requests, each including the product ID and variant ID. The list of properties may vary depending on the specific platform. | 

## Examples

- Prepare the resource
```powershell
$ProductVariantDeleteBatch = Initialize-PSOpenAPIToolsProductVariantDeleteBatch  -ClearCache null `
 -Reindex null `
 -Payload null
```

- Convert the resource to JSON
```powershell
$ProductVariantDeleteBatch | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

