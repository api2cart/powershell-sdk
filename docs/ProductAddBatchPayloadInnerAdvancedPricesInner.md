# ProductAddBatchPayloadInnerAdvancedPricesInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Value** | **Decimal** |  | 
**GroupId** | **Int32** |  | [optional] 
**Quantity** | **Decimal** |  | 
**StartTime** | **String** |  | [optional] 
**ExpireTime** | **String** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAddBatchPayloadInnerAdvancedPricesInner = Initialize-PSOpenAPIToolsProductAddBatchPayloadInnerAdvancedPricesInner  -Value null `
 -GroupId null `
 -Quantity null `
 -StartTime null `
 -ExpireTime null
```

- Convert the resource to JSON
```powershell
$ProductAddBatchPayloadInnerAdvancedPricesInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

