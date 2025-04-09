# OrderPreestimateShipping
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**MethodCode** | **String** |  | [optional] 
**MethodName** | **String** |  | [optional] 
**CarrierCode** | **String** |  | [optional] 
**CarrierName** | **String** |  | [optional] 
**Description** | **String** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**PriceIncTax** | **Decimal** |  | [optional] 
**DeliveryTime** | **String** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderPreestimateShipping = Initialize-PSOpenAPIToolsOrderPreestimateShipping  -MethodCode null `
 -MethodName null `
 -CarrierCode null `
 -CarrierName null `
 -Description null `
 -Price null `
 -PriceIncTax null `
 -DeliveryTime null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderPreestimateShipping | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

