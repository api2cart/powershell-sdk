# CategoryAddBatch
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Payload** | [**CategoryAddBatchPayloadInner[]**](CategoryAddBatchPayloadInner.md) | Contains an array of categories objects. The list of properties may vary depending on the specific platform. | 

## Examples

- Prepare the resource
```powershell
$CategoryAddBatch = Initialize-PSOpenAPIToolsCategoryAddBatch  -Payload null
```

- Convert the resource to JSON
```powershell
$CategoryAddBatch | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

