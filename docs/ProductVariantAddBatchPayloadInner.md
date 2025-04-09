# ProductVariantAddBatchPayloadInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProductId** | **String** |  | 
**Combination** | [**ProductVariantAddBatchPayloadInnerCombinationInner[]**](ProductVariantAddBatchPayloadInnerCombinationInner.md) | A unique combination that contains an array of options and their values, which form a variation. | 
**Name** | **String** |  | [optional] 
**Description** | **String** |  | [optional] 
**ShortDescription** | **String** |  | [optional] 
**Sku** | **String** |  | 
**Model** | **String** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**OldPrice** | **Decimal** |  | [optional] 
**CostPrice** | **Decimal** |  | [optional] 
**SpecialPrice** | **Decimal** |  | [optional] 
**SpriceCreate** | **String** |  | [optional] 
**SpriceExpire** | **String** |  | [optional] 
**AdvancedPrices** | [**ProductUpdateBatchPayloadInnerAdvancedPricesInner[]**](ProductUpdateBatchPayloadInnerAdvancedPricesInner.md) |  | [optional] 
**MetaTitle** | **Decimal** |  | [optional] 
**MetaDescription** | **Decimal** |  | [optional] 
**MetaKeywords** | **String[]** |  | [optional] 
**CategoriesIds** | **String[]** |  | [optional] 
**StoresIds** | **String[]** |  | [optional] 
**Weight** | **Decimal** |  | [optional] 
**Width** | **Decimal** |  | [optional] 
**Height** | **Decimal** |  | [optional] 
**Length** | **Decimal** |  | [optional] 
**WeightUnit** | **String** |  | [optional] 
**WarehouseId** | **String** |  | [optional] 
**Quantity** | **Decimal** |  | [optional] 
**ManageStock** | **Boolean** |  | [optional] 
**InStock** | **Boolean** |  | [optional] 
**StoreId** | **String** |  | [optional] 
**LangId** | **String** |  | [optional] 
**TaxClassId** | **String** |  | [optional] 
**BackorderStatus** | **String** |  | [optional] 
**Status** | **String** |  | [optional] 
**Visible** | **String** |  | [optional] 
**IsVirtual** | **Boolean** |  | [optional] 
**Downloadable** | **Boolean** |  | [optional] 
**IsDefault** | **Boolean** |  | [optional] 
**Upc** | **String** |  | [optional] 
**Isbn** | **String** |  | [optional] 
**Mpn** | **String** |  | [optional] 
**Ean** | **String** |  | [optional] 
**Barcode** | **String** |  | [optional] 
**AvailableForSale** | **Boolean** |  | [optional] 
**IsFreeShipping** | **Boolean** |  | [optional] 
**Taxable** | **Boolean** |  | [optional] 
**SeoUrl** | **String** |  | [optional] 
**ManufacturerId** | **String** |  | [optional] 
**HarmonizedSystemCode** | **String** |  | [optional] 
**MarketplaceItemProperties** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**Images** | [**ProductAddBatchPayloadInnerImagesInner[]**](ProductAddBatchPayloadInnerImagesInner.md) |  | [optional] 
**ProductImagesIds** | **String[]** |  | [optional] 
**RelatedProductsIds** | **String[]** |  | [optional] 
**UpSellProductsIds** | **String[]** |  | [optional] 
**CrossSellProductsIds** | **String[]** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductVariantAddBatchPayloadInner = Initialize-PSOpenAPIToolsProductVariantAddBatchPayloadInner  -ProductId null `
 -Combination null `
 -Name null `
 -Description null `
 -ShortDescription null `
 -Sku null `
 -Model null `
 -Price null `
 -OldPrice null `
 -CostPrice null `
 -SpecialPrice null `
 -SpriceCreate null `
 -SpriceExpire null `
 -AdvancedPrices null `
 -MetaTitle null `
 -MetaDescription null `
 -MetaKeywords null `
 -CategoriesIds null `
 -StoresIds null `
 -Weight null `
 -Width null `
 -Height null `
 -Length null `
 -WeightUnit null `
 -WarehouseId null `
 -Quantity null `
 -ManageStock null `
 -InStock null `
 -StoreId null `
 -LangId null `
 -TaxClassId null `
 -BackorderStatus null `
 -Status null `
 -Visible null `
 -IsVirtual null `
 -Downloadable null `
 -IsDefault null `
 -Upc null `
 -Isbn null `
 -Mpn null `
 -Ean null `
 -Barcode null `
 -AvailableForSale null `
 -IsFreeShipping null `
 -Taxable null `
 -SeoUrl null `
 -ManufacturerId null `
 -HarmonizedSystemCode null `
 -MarketplaceItemProperties null `
 -Images null `
 -ProductImagesIds null `
 -RelatedProductsIds null `
 -UpSellProductsIds null `
 -CrossSellProductsIds null
```

- Convert the resource to JSON
```powershell
$ProductVariantAddBatchPayloadInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

