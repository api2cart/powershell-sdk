# OrderCalculateBundle
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProductId** | **String** |  | [optional] 
**Sku** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Quantity** | **Int32** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**PriceIncTax** | **Decimal** |  | [optional] 
**TaxRate** | **Decimal** |  | [optional] 
**UnitDiscount** | **Decimal** |  | [optional] 
**Weight** | **Decimal** |  | [optional] 
**WeightUnit** | **String** |  | [optional] 
**Barcode** | **String** |  | [optional] 
**VariantId** | **String** |  | [optional] 
**Options** | [**OrderItemOption[]**](OrderItemOption.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderCalculateBundle = Initialize-PSOpenAPIToolsOrderCalculateBundle  -ProductId null `
 -Sku null `
 -Name null `
 -Quantity null `
 -Price null `
 -PriceIncTax null `
 -TaxRate null `
 -UnitDiscount null `
 -Weight null `
 -WeightUnit null `
 -Barcode null `
 -VariantId null `
 -Options null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderCalculateBundle | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

