# Basket
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Customer** | [**BaseCustomer**](BaseCustomer.md) |  | [optional] 
**BasketUrl** | **String** |  | [optional] 
**CreatedAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**ModifiedAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**Currency** | [**Currency**](Currency.md) |  | [optional] 
**BasketProducts** | [**BasketItem[]**](BasketItem.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Basket = Initialize-PSOpenAPIToolsBasket  -Id null `
 -Customer null `
 -BasketUrl null `
 -CreatedAt null `
 -ModifiedAt null `
 -Currency null `
 -BasketProducts null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Basket | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

