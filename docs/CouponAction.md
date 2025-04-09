# CouponAction
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Scope** | **String** |  | [optional] 
**ApplyTo** | **String** |  | [optional] 
**Amount** | **Decimal** |  | [optional] 
**CurrencyCode** | **String** |  | [optional] 
**IncludeTax** | **Boolean** |  | [optional] 
**Type** | **String** |  | [optional] 
**DiscountedQuantity** | **Decimal** |  | [optional] 
**DiscountQuantityStep** | **Int32** |  | [optional] 
**LogicOperator** | **String** |  | [optional] 
**Conditions** | [**CouponCondition[]**](CouponCondition.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CouponAction = Initialize-PSOpenAPIToolsCouponAction  -Scope null `
 -ApplyTo null `
 -Amount null `
 -CurrencyCode null `
 -IncludeTax null `
 -Type null `
 -DiscountedQuantity null `
 -DiscountQuantityStep null `
 -LogicOperator null `
 -Conditions null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$CouponAction | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

