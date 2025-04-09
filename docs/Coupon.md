# Coupon
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Code** | **String** |  | [optional] 
**Codes** | [**CouponCode[]**](CouponCode.md) |  | [optional] 
**Name** | **String** |  | [optional] 
**Description** | **String** |  | [optional] 
**Actions** | [**CouponAction[]**](CouponAction.md) |  | [optional] 
**DateStart** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**DateEnd** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**Avail** | **Boolean** |  | [optional] 
**Priority** | **Int32** |  | [optional] 
**UsedTimes** | **Int32** |  | [optional] 
**UsageLimit** | **Int32** |  | [optional] 
**UsageLimitPerCustomer** | **Int32** |  | [optional] 
**LogicOperator** | **String** |  | [optional] 
**Conditions** | [**CouponCondition[]**](CouponCondition.md) |  | [optional] 
**UsageHistory** | [**CouponHistory[]**](CouponHistory.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Coupon = Initialize-PSOpenAPIToolsCoupon  -Id null `
 -Code null `
 -Codes null `
 -Name null `
 -Description null `
 -Actions null `
 -DateStart null `
 -DateEnd null `
 -Avail null `
 -Priority null `
 -UsedTimes null `
 -UsageLimit null `
 -UsageLimitPerCustomer null `
 -LogicOperator null `
 -Conditions null `
 -UsageHistory null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Coupon | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

