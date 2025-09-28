# ProductAddBatchPayloadInnerSalesTax
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TaxPercent** | **Decimal** |  | [optional] 
**Taxable** | **Boolean** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAddBatchPayloadInnerSalesTax = Initialize-PSOpenAPIToolsProductAddBatchPayloadInnerSalesTax  -TaxPercent null `
 -Taxable null
```

- Convert the resource to JSON
```powershell
$ProductAddBatchPayloadInnerSalesTax | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

