# CatalogPriceRule
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Gid** | **String** |  | [optional] 
**Type** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Description** | **String** |  | [optional] 
**ShortDescription** | **String** |  | [optional] 
**Avail** | **Boolean** |  | [optional] 
**Actions** | [**CatalogPriceRuleAction[]**](CatalogPriceRuleAction.md) |  | [optional] 
**CreatedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**DateStart** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**DateEnd** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**UsageCount** | **Decimal** |  | [optional] 
**Conditions** | [**CouponCondition[]**](CouponCondition.md) |  | [optional] 
**UsesPerOrderLimit** | **Int32** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CatalogPriceRule = Initialize-PSOpenAPIToolsCatalogPriceRule  -Id null `
 -Gid null `
 -Type null `
 -Name null `
 -Description null `
 -ShortDescription null `
 -Avail null `
 -Actions null `
 -CreatedTime null `
 -DateStart null `
 -DateEnd null `
 -UsageCount null `
 -Conditions null `
 -UsesPerOrderLimit null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$CatalogPriceRule | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

