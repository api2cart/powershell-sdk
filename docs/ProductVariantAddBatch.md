# ProductVariantAddBatch
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ClearCache** | **Boolean** |  | [optional] [default to $false]
**Reindex** | **Boolean** |  | [optional] [default to $false]
**Payload** | [**ProductVariantAddBatchPayloadInner[]**](ProductVariantAddBatchPayloadInner.md) | Contains an array of product variants objects. The list of properties may vary depending on the specific platform. | 

## Examples

- Prepare the resource
```powershell
$ProductVariantAddBatch = Initialize-PSOpenAPIToolsProductVariantAddBatch  -ClearCache null `
 -Reindex null `
 -Payload null
```

- Convert the resource to JSON
```powershell
$ProductVariantAddBatch | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

