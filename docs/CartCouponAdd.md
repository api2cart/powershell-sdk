# CartCouponAdd
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code** | **String** | Coupon code | 
**ActionType** | **String** | Coupon discount type | 
**ActionApplyTo** | **String** | Defines where discount should be applied | 
**ActionScope** | **String** | Specify how discount should be applied. If scope&#x3D;matching_items, then discount will be applied to each of the items that match action conditions. Scope order means that discount will be applied once. | 
**ActionAmount** | **Decimal** | Defines the discount amount value. | 
**Codes** | **String[]** | Entity codes | [optional] 
**Name** | **String** | Coupon name | [optional] 
**DateStart** | **String** | Date start | [optional] [default to "now"]
**DateEnd** | **String** | Defines when discount code will be expired. | [optional] 
**UsageLimit** | **Int32** | Usage limit for coupon. | [optional] 
**UsageLimitPerCustomer** | **Int32** | Usage limit per customer. | [optional] 
**ActionConditionEntity** | **String** | Defines entity for action condition. | [optional] 
**ActionConditionKey** | **String** | Defines entity attribute code for action condition. | [optional] 
**ActionConditionOperator** | **String** | Defines condition operator. | [optional] 
**ActionConditionValue** | **String** | Defines condition attribute value/s. Can be comma separated string. | [optional] 
**IncludeTax** | **Boolean** | Indicates whether to apply a discount for taxes. | [optional] [default to $false]
**StoreId** | **String** | Store Id | [optional] 
**FreeCashOnDelivery** | **Boolean** | Defines whether the coupon provides free cash on delivery | [optional] 
**CustomerId** | **String** | Retrieves orders specified by customer id | [optional] 

## Examples

- Prepare the resource
```powershell
$CartCouponAdd = Initialize-PSOpenAPIToolsCartCouponAdd  -Code 000_BIG_SALE_000 `
 -ActionType percent `
 -ActionApplyTo order_total `
 -ActionScope matching_items `
 -ActionAmount 15.5 `
 -Codes codes[0]&#x3D;000_BIG_SALE_000&amp;codes[1]&#x3D;000_BIG_SALE_001&amp;codes[2]&#x3D;000_BIG_SALE_002 `
 -Name Sale! -30% `
 -DateStart 2019-12-29 06:44:30 `
 -DateEnd 2020-01-05 01:00:00 `
 -UsageLimit 99 `
 -UsageLimitPerCustomer 1 `
 -ActionConditionEntity order `
 -ActionConditionKey product_id `
 -ActionConditionOperator ONE_OF `
 -ActionConditionValue 17834222,45466663 `
 -IncludeTax true `
 -StoreId 1 `
 -FreeCashOnDelivery true `
 -CustomerId 5
```

- Convert the resource to JSON
```powershell
$CartCouponAdd | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

