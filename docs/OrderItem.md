# OrderItem
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProductId** | **String** |  | [optional] 
**OrderProductId** | **String** |  | [optional] 
**Model** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**PriceIncTax** | **Decimal** |  | [optional] 
**Quantity** | **Decimal** |  | [optional] 
**DiscountAmount** | **Decimal** |  | [optional] 
**TotalPrice** | **Decimal** |  | [optional] 
**TaxPercent** | **Decimal** |  | [optional] 
**TaxValue** | **Decimal** |  | [optional] 
**TaxValueAfterDiscount** | **Decimal** |  | [optional] 
**Options** | [**OrderItemOption[]**](OrderItemOption.md) |  | [optional] 
**VariantId** | **String** |  | [optional] 
**WeightUnit** | **String** |  | [optional] 
**Weight** | **Decimal** |  | [optional] 
**Barcode** | **String** |  | [optional] 
**ParentOrderProductId** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderItem = Initialize-PSOpenAPIToolsOrderItem  -ProductId null `
 -OrderProductId null `
 -Model null `
 -Name null `
 -Price null `
 -PriceIncTax null `
 -Quantity null `
 -DiscountAmount null `
 -TotalPrice null `
 -TaxPercent null `
 -TaxValue null `
 -TaxValueAfterDiscount null `
 -Options null `
 -VariantId null `
 -WeightUnit null `
 -Weight null `
 -Barcode null `
 -ParentOrderProductId null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderItem | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

