# BasketItem
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**ParentId** | **String** |  | [optional] 
**ProductId** | **String** |  | [optional] 
**VariantId** | **String** |  | [optional] 
**Sku** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**Tax** | **Decimal** |  | [optional] 
**Quantity** | **Decimal** |  | [optional] 
**WeightUnit** | **String** |  | [optional] 
**Weight** | **Decimal** |  | [optional] 
**Options** | [**BasketItemOption[]**](BasketItemOption.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$BasketItem = Initialize-PSOpenAPIToolsBasketItem  -Id null `
 -ParentId null `
 -ProductId null `
 -VariantId null `
 -Sku null `
 -Name null `
 -Price null `
 -Tax null `
 -Quantity null `
 -WeightUnit null `
 -Weight null `
 -Options null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$BasketItem | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

