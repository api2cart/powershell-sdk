# Child
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**ParentId** | **String** |  | [optional] 
**Sku** | **String** |  | [optional] 
**Upc** | **String** |  | [optional] 
**Ean** | **String** |  | [optional] 
**Mpn** | **String** |  | [optional] 
**Gtin** | **String** |  | [optional] 
**Isbn** | **String** |  | [optional] 
**Url** | **String** |  | [optional] 
**SeoUrl** | **String** |  | [optional] 
**SortOrder** | **Int32** |  | [optional] 
**CreatedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**ModifiedTime** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**Name** | **String** |  | [optional] 
**ShortDescription** | **String** |  | [optional] 
**FullDescription** | **String** |  | [optional] 
**Images** | [**Image[]**](Image.md) |  | [optional] 
**Combination** | [**ProductChildItemCombination[]**](ProductChildItemCombination.md) |  | [optional] 
**DefaultPrice** | **Decimal** |  | [optional] 
**CostPrice** | **Decimal** |  | [optional] 
**ListPrice** | **Decimal** |  | [optional] 
**WholesalePrice** | **Decimal** |  | [optional] 
**AdvancedPrice** | [**ProductAdvancedPrice[]**](ProductAdvancedPrice.md) |  | [optional] 
**TaxClassId** | **String** |  | [optional] 
**AvailForSale** | **Boolean** |  | [optional] 
**AllowBackorders** | **Boolean** |  | [optional] 
**InStock** | **Boolean** |  | [optional] 
**ManageStock** | **Boolean** |  | [optional] 
**InventoryLevel** | **Decimal** |  | [optional] 
**Inventory** | [**ProductInventory[]**](ProductInventory.md) |  | [optional] 
**MinQuantity** | **Decimal** |  | [optional] 
**DefaultQtyInPack** | **Decimal** |  | [optional] 
**IsQtyInPackFixed** | **Boolean** |  | [optional] 
**WeightUnit** | **String** |  | [optional] 
**Weight** | **Decimal** |  | [optional] 
**DimensionsUnit** | **String** |  | [optional] 
**Width** | **Decimal** |  | [optional] 
**Height** | **Decimal** |  | [optional] 
**Length** | **Decimal** |  | [optional] 
**MetaTitle** | **String** |  | [optional] 
**MetaDescription** | **String** |  | [optional] 
**MetaKeywords** | **String** |  | [optional] 
**Discounts** | [**Discount[]**](Discount.md) |  | [optional] 
**IsVirtual** | **Boolean** |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Child = Initialize-PSOpenAPIToolsChild  -Id null `
 -ParentId null `
 -Sku null `
 -Upc null `
 -Ean null `
 -Mpn null `
 -Gtin null `
 -Isbn null `
 -Url null `
 -SeoUrl null `
 -SortOrder null `
 -CreatedTime null `
 -ModifiedTime null `
 -Name null `
 -ShortDescription null `
 -FullDescription null `
 -Images null `
 -Combination null `
 -DefaultPrice null `
 -CostPrice null `
 -ListPrice null `
 -WholesalePrice null `
 -AdvancedPrice null `
 -TaxClassId null `
 -AvailForSale null `
 -AllowBackorders null `
 -InStock null `
 -ManageStock null `
 -InventoryLevel null `
 -Inventory null `
 -MinQuantity null `
 -DefaultQtyInPack null `
 -IsQtyInPackFixed null `
 -WeightUnit null `
 -Weight null `
 -DimensionsUnit null `
 -Width null `
 -Height null `
 -Length null `
 -MetaTitle null `
 -MetaDescription null `
 -MetaKeywords null `
 -Discounts null `
 -IsVirtual null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Child | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

