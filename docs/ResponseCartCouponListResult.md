# ResponseCartCouponListResult
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CouponCount** | **Int32** |  | [optional] 
**Coupon** | [**Coupon[]**](Coupon.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ResponseCartCouponListResult = Initialize-PSOpenAPIToolsResponseCartCouponListResult  -CouponCount null `
 -Coupon null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$ResponseCartCouponListResult | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

