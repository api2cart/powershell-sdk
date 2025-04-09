# CartStoreInfo
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**StoreId** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Language** | **String** |  | [optional] 
**StoreLanguages** | [**Language[]**](Language.md) |  | [optional] 
**Currency** | [**Currency**](Currency.md) |  | [optional] 
**StoreCurrencies** | [**Currency[]**](Currency.md) |  | [optional] 
**Timezone** | **String** |  | [optional] 
**Country** | **String** |  | [optional] 
**RootCategoryId** | **String** |  | [optional] 
**MultiStoreUrl** | **String** |  | [optional] 
**Active** | **Boolean** |  | [optional] 
**WeightUnit** | **String** |  | [optional] 
**DimensionUnit** | **String** |  | [optional] 
**PricesIncludeTax** | **Boolean** |  | [optional] 
**CarrierInfo** | [**Carrier[]**](Carrier.md) |  | [optional] 
**StoreOwnerInfo** | [**Info**](Info.md) |  | [optional] 
**DefaultWarehouseId** | **String** |  | [optional] 
**Channels** | [**CartChannel[]**](CartChannel.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$CartStoreInfo = Initialize-PSOpenAPIToolsCartStoreInfo  -StoreId null `
 -Name null `
 -Language null `
 -StoreLanguages null `
 -Currency null `
 -StoreCurrencies null `
 -Timezone null `
 -Country null `
 -RootCategoryId null `
 -MultiStoreUrl null `
 -Active null `
 -WeightUnit null `
 -DimensionUnit null `
 -PricesIncludeTax null `
 -CarrierInfo null `
 -StoreOwnerInfo null `
 -DefaultWarehouseId null `
 -Channels null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$CartStoreInfo | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

