# ProductVariantPriceAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** | Defines the variant to which the price has to be added | [optional] 
**ProductId** | **String** | Product id | [optional] 
**GroupPrices** | [**ProductAddGroupPricesInner[]**](ProductAddGroupPricesInner.md) | Defines variants&#39;s group prices | 
**StoreId** | **String** | Store Id | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductVariantPriceAdd = Initialize-PSOpenAPIToolsProductVariantPriceAdd  -Id 10 `
 -ProductId 10 `
 -GroupPrices null `
 -StoreId 1
```

- Convert the resource to JSON
```powershell
$ProductVariantPriceAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

