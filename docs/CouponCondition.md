# CouponCondition
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Entity** | **String** |  | [optional] 
**MatchItems** | **String** |  | [optional] 
**Key** | **String** |  | [optional] 
**Operator** | **String** |  | [optional] 
**Value** | **String** |  | [optional] 
**LogicOperator** | **String** |  | [optional] 
**SubConditions** | [**CouponCondition[]**](CouponCondition.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CouponCondition = Initialize-PSOpenAPIToolsCouponCondition  -Id null `
 -Entity null `
 -MatchItems null `
 -Key null `
 -Operator null `
 -Value null `
 -LogicOperator null `
 -SubConditions null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$CouponCondition | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

