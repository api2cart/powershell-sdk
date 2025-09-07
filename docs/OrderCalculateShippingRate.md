# OrderCalculateShippingRate
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**PriceIncTax** | **Decimal** |  | [optional] 
**Tax** | **Decimal** |  | [optional] 
**TaxRate** | **Decimal** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderCalculateShippingRate = Initialize-PSOpenAPIToolsOrderCalculateShippingRate  -Code null `
 -Name null `
 -Price null `
 -PriceIncTax null `
 -Tax null `
 -TaxRate null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderCalculateShippingRate | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

