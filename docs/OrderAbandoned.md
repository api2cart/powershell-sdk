# OrderAbandoned
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Customer** | [**BaseCustomer**](BaseCustomer.md) |  | [optional] 
**BasketId** | **String** |  | [optional] 
**BasketUrl** | **String** |  | [optional] 
**CreatedAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**ModifiedAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**Currency** | [**Currency**](Currency.md) |  | [optional] 
**Totals** | [**OrderTotals**](OrderTotals.md) |  | [optional] 
**OrderProducts** | [**OrderItem[]**](OrderItem.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$OrderAbandoned = Initialize-PSOpenAPIToolsOrderAbandoned  -Id null `
 -Customer null `
 -BasketId null `
 -BasketUrl null `
 -CreatedAt null `
 -ModifiedAt null `
 -Currency null `
 -Totals null `
 -OrderProducts null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$OrderAbandoned | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

