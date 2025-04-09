# ProductPriceUpdate
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProductId** | **String** | Defines the product where the price has to be updated | [optional] 
**GroupPrices** | [**ProductPriceUpdateGroupPricesInner[]**](ProductPriceUpdateGroupPricesInner.md) | Defines product&#39;s group prices | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductPriceUpdate = Initialize-PSOpenAPIToolsProductPriceUpdate  -ProductId 10 `
 -GroupPrices null
```

- Convert the resource to JSON
```powershell
$ProductPriceUpdate | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

