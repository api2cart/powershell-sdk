# OrderTotal
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SubtotalExTax** | **Decimal** |  | [optional] 
**WrappingExTax** | **Decimal** |  | [optional] 
**ShippingExTax** | **Decimal** |  | [optional] 
**TotalDiscount** | **Decimal** |  | [optional] 
**TotalTax** | **Decimal** |  | [optional] 
**Total** | **Decimal** |  | [optional] 
**TotalPaid** | **Decimal** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderTotal = Initialize-PSOpenAPIToolsOrderTotal  -SubtotalExTax null `
 -WrappingExTax null `
 -ShippingExTax null `
 -TotalDiscount null `
 -TotalTax null `
 -Total null `
 -TotalPaid null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderTotal | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

