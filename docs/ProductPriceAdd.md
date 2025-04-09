# ProductPriceAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProductId** | **String** | Defines the product to which the price has to be added | [optional] 
**GroupPrices** | [**ProductAddGroupPricesInner[]**](ProductAddGroupPricesInner.md) | Defines product&#39;s group prices | [optional] 
**StoreId** | **String** | Store Id | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductPriceAdd = Initialize-PSOpenAPIToolsProductPriceAdd  -ProductId 10 `
 -GroupPrices null `
 -StoreId 1
```

- Convert the resource to JSON
```powershell
$ProductPriceAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

