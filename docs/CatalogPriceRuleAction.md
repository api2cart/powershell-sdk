# CatalogPriceRuleAction
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Scope** | **String** |  | [optional] 
**ApplyTo** | **String** |  | [optional] 
**Type** | **String** |  | [optional] 
**Quantity** | **Decimal** |  | [optional] 
**Value** | **Decimal** |  | [optional] 
**CurrencyCode** | **String** |  | [optional] 
**IncludeTax** | **Boolean** |  | [optional] 
**Conditions** | [**CouponCondition[]**](CouponCondition.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CatalogPriceRuleAction = Initialize-PSOpenAPIToolsCatalogPriceRuleAction  -Scope null `
 -ApplyTo null `
 -Type null `
 -Quantity null `
 -Value null `
 -CurrencyCode null `
 -IncludeTax null `
 -Conditions null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$CatalogPriceRuleAction | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

