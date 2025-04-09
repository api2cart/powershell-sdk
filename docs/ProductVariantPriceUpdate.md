# ProductVariantPriceUpdate
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** | Defines the variant where the price has to be updated | [optional] 
**ProductId** | **String** | Product id | [optional] 
**GroupPrices** | [**ProductPriceUpdateGroupPricesInner[]**](ProductPriceUpdateGroupPricesInner.md) | Defines variants&#39;s group prices | 

## Examples

- Prepare the resource
```powershell
$ProductVariantPriceUpdate = Initialize-PSOpenAPIToolsProductVariantPriceUpdate  -Id 10 `
 -ProductId 10 `
 -GroupPrices null
```

- Convert the resource to JSON
```powershell
$ProductVariantPriceUpdate | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

