# ProductVariantAddAttributesInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeName** | **String** |  | [optional] 
**AttributeValue** | **String** |  | [optional] 
**AttributePrice** | **Decimal** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductVariantAddAttributesInner = Initialize-PSOpenAPIToolsProductVariantAddAttributesInner  -AttributeName null `
 -AttributeValue null `
 -AttributePrice null
```

- Convert the resource to JSON
```powershell
$ProductVariantAddAttributesInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

