# Product
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | [optional] 
**Type** | **String** |  | [optional] 
**UModel** | **String** |  | [optional] 
**USku** | **String** |  | [optional] 
**Name** | **String** |  | [optional] 
**Description** | **String** |  | [optional] 
**ShortDescription** | **String** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**AdvancedPrice** | [**ProductAdvancedPrice[]**](ProductAdvancedPrice.md) |  | [optional] 
**CostPrice** | **Decimal** |  | [optional] 
**Quantity** | **Decimal** |  | [optional] 
**Inventory** | [**ProductInventory[]**](ProductInventory.md) |  | [optional] 
**GroupItems** | [**ProductGroupItem[]**](ProductGroupItem.md) |  | [optional] 
**UBrandId** | **String** |  | [optional] 
**UBrand** | **String** |  | [optional] 
**CategoriesIds** | **String[]** |  | [optional] 
**StoresIds** | **String[]** |  | [optional] 
**Url** | **String** |  | [optional] 
**SeoUrl** | **String** |  | [optional] 
**MetaTitle** | **String** |  | [optional] 
**MetaKeywords** | **String** |  | [optional] 
**MetaDescription** | **String** |  | [optional] 
**AvailSale** | **Boolean** |  | [optional] 
**AvailView** | **Boolean** |  | [optional] 
**IsVirtual** | **Boolean** |  | [optional] 
**IsDownloadable** | **Boolean** |  | [optional] 
**Weight** | **Decimal** |  | [optional] 
**WeightUnit** | **String** |  | [optional] 
**SortOrder** | **Int32** |  | [optional] 
**InStock** | **Boolean** |  | [optional] 
**Backorders** | **String** |  | [optional] 
**ManageStock** | **String** |  | [optional] 
**IsStockManaged** | **Boolean** |  | [optional] 
**CreateAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**ModifiedAt** | [**A2CDateTime**](A2CDateTime.md) |  | [optional] 
**TaxClassId** | **String** |  | [optional] 
**SpecialPrice** | [**SpecialPrice**](SpecialPrice.md) |  | [optional] 
**TierPrice** | [**ProductTierPrice[]**](ProductTierPrice.md) |  | [optional] 
**GroupPrice** | [**ProductGroupPrice[]**](ProductGroupPrice.md) |  | [optional] 
**Images** | [**Image[]**](Image.md) |  | [optional] 
**ProductOptions** | [**ProductOption[]**](ProductOption.md) |  | [optional] 
**UUpc** | **String** |  | [optional] 
**UMpn** | **String** |  | [optional] 
**UGtin** | **String** |  | [optional] 
**UIsbn** | **String** |  | [optional] 
**UEan** | **String** |  | [optional] 
**RelatedProductsIds** | **String[]** |  | [optional] 
**UpSellProductsIds** | **String[]** |  | [optional] 
**CrossSellProductsIds** | **String[]** |  | [optional] 
**DimensionsUnit** | **String** |  | [optional] 
**Width** | **Decimal** |  | [optional] 
**Height** | **Decimal** |  | [optional] 
**Length** | **Decimal** |  | [optional] 
**Discounts** | [**Discount[]**](Discount.md) |  | [optional] 
**AdditionalFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**CustomFields** | [**SystemCollectionsHashtable**](.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$Product = Initialize-PSOpenAPIToolsProduct  -Id null `
 -Type null `
 -UModel null `
 -USku null `
 -Name null `
 -Description null `
 -ShortDescription null `
 -Price null `
 -AdvancedPrice null `
 -CostPrice null `
 -Quantity null `
 -Inventory null `
 -GroupItems null `
 -UBrandId null `
 -UBrand null `
 -CategoriesIds null `
 -StoresIds null `
 -Url null `
 -SeoUrl null `
 -MetaTitle null `
 -MetaKeywords null `
 -MetaDescription null `
 -AvailSale null `
 -AvailView null `
 -IsVirtual null `
 -IsDownloadable null `
 -Weight null `
 -WeightUnit null `
 -SortOrder null `
 -InStock null `
 -Backorders null `
 -ManageStock null `
 -IsStockManaged null `
 -CreateAt null `
 -ModifiedAt null `
 -TaxClassId null `
 -SpecialPrice null `
 -TierPrice null `
 -GroupPrice null `
 -Images null `
 -ProductOptions null `
 -UUpc null `
 -UMpn null `
 -UGtin null `
 -UIsbn null `
 -UEan null `
 -RelatedProductsIds null `
 -UpSellProductsIds null `
 -CrossSellProductsIds null `
 -DimensionsUnit null `
 -Width null `
 -Height null `
 -Length null `
 -Discounts null `
 -AdditionalFields null `
 -CustomFields null
```

- Convert the resource to JSON
```powershell
$Product | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

