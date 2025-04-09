# ProductTaxAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProductId** | **String** | Defines products specified by product id | [optional] 
**Name** | **String** | Defines tax class name where tax has to be added | 
**TaxRates** | [**ProductTaxAddTaxRatesInner[]**](ProductTaxAddTaxRatesInner.md) | Defines tax rates of specified tax classes | 

## Examples

- Prepare the resource
```powershell
$ProductTaxAdd = Initialize-PSOpenAPIToolsProductTaxAdd  -ProductId 10 `
 -Name ECO-Tax `
 -TaxRates null
```

- Convert the resource to JSON
```powershell
$ProductTaxAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

