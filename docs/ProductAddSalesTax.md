# ProductAddSalesTax
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TaxPercent** | **Decimal** |  | [optional] 
**TaxState** | **String** |  | [optional] 
**ShippingIncInTax** | **Boolean** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAddSalesTax = Initialize-PSOpenAPIToolsProductAddSalesTax  -TaxPercent null `
 -TaxState null `
 -ShippingIncInTax null
```

- Convert the resource to JSON
```powershell
$ProductAddSalesTax | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

