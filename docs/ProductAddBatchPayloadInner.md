# ProductAddBatchPayloadInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **String** |  | [optional] 
**Description** | **String** |  | [optional] 
**ShortDescription** | **String** |  | [optional] 
**Sku** | **String** |  | [optional] 
**Model** | **String** |  | [optional] 
**Asin** | **String** |  | [optional] 
**Upc** | **String** |  | [optional] 
**Ean** | **String** |  | [optional] 
**Gtin** | **String** |  | [optional] 
**Mpn** | **String** |  | [optional] 
**Barcode** | **String** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**OldPrice** | **Decimal** |  | [optional] 
**CostPrice** | **Decimal** |  | [optional] 
**SpecialPrice** | **Decimal** |  | [optional] 
**SpriceCreate** | **String** |  | [optional] 
**SpriceExpire** | **String** |  | [optional] 
**AdvancedPrices** | [**ProductAddBatchPayloadInnerAdvancedPricesInner[]**](ProductAddBatchPayloadInnerAdvancedPricesInner.md) |  | [optional] 
**FixedCostShippingPrice** | **Decimal** |  | [optional] 
**Quantity** | **Decimal** |  | [optional] 
**ManageStock** | **Boolean** |  | [optional] 
**ProductType** | **String** |  | [optional] 
**MarketplaceItemProperties** | [**SystemCollectionsHashtable**](.md) |  | [optional] 
**IsFreeShipping** | **Boolean** |  | [optional] 
**Taxable** | **Boolean** |  | [optional] 
**Status** | **String** |  | [optional] 
**Condition** | **String** |  | [optional] 
**Visible** | **String** |  | [optional] 
**AvailableForView** | **Boolean** |  | [optional] 
**AvailableForSale** | **Boolean** |  | [optional] 
**IsVirtual** | **Boolean** |  | [optional] 
**InStock** | **Boolean** |  | [optional] 
**Type** | **String** |  | [optional] 
**Downloadable** | **Boolean** |  | [optional] 
**Weight** | **Decimal** |  | [optional] 
**Length** | **Decimal** |  | [optional] 
**Width** | **Decimal** |  | [optional] 
**Height** | **Decimal** |  | [optional] 
**WeightUnit** | **String** |  | [optional] 
**DimensionsUnit** | **String** |  | [optional] 
**StoreId** | **String** |  | [optional] 
**LangId** | **String** |  | [optional] 
**CategoryId** | **String** |  | [optional] 
**WarehouseId** | **String** |  | [optional] 
**CategoriesIds** | **String[]** |  | [optional] 
**RelatedProductsIds** | **String[]** |  | [optional] 
**UpSellProductsIds** | **String[]** |  | [optional] 
**CrossSellProductsIds** | **String[]** |  | [optional] 
**StoresIds** | **String[]** |  | [optional] 
**TaxClassId** | **String** |  | [optional] 
**MetaTitle** | **String** |  | [optional] 
**MetaDescription** | **String** |  | [optional] 
**MetaKeywords** | **String[]** |  | [optional] 
**SearchKeywords** | **String[]** |  | [optional] 
**HarmonizedSystemCode** | **String** |  | [optional] 
**Url** | **String** |  | [optional] 
**SeoUrl** | **String** |  | [optional] 
**Manufacturer** | **String** |  | [optional] 
**ManufacturerId** | **String** |  | [optional] 
**BackorderStatus** | **String** |  | [optional] 
**Images** | [**ProductAddBatchPayloadInnerImagesInner[]**](ProductAddBatchPayloadInnerImagesInner.md) |  | [optional] 
**Tags** | **String[]** |  | [optional] 
**Files** | [**ProductAddFilesInner[]**](ProductAddFilesInner.md) |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductAddBatchPayloadInner = Initialize-PSOpenAPIToolsProductAddBatchPayloadInner  -Name null `
 -Description null `
 -ShortDescription null `
 -Sku null `
 -Model null `
 -Asin null `
 -Upc null `
 -Ean null `
 -Gtin null `
 -Mpn null `
 -Barcode null `
 -Price null `
 -OldPrice null `
 -CostPrice null `
 -SpecialPrice null `
 -SpriceCreate null `
 -SpriceExpire null `
 -AdvancedPrices null `
 -FixedCostShippingPrice null `
 -Quantity null `
 -ManageStock null `
 -ProductType null `
 -MarketplaceItemProperties null `
 -IsFreeShipping null `
 -Taxable null `
 -Status null `
 -Condition null `
 -Visible null `
 -AvailableForView null `
 -AvailableForSale null `
 -IsVirtual null `
 -InStock null `
 -Type null `
 -Downloadable null `
 -Weight null `
 -Length null `
 -Width null `
 -Height null `
 -WeightUnit null `
 -DimensionsUnit null `
 -StoreId null `
 -LangId null `
 -CategoryId null `
 -WarehouseId null `
 -CategoriesIds null `
 -RelatedProductsIds null `
 -UpSellProductsIds null `
 -CrossSellProductsIds null `
 -StoresIds null `
 -TaxClassId null `
 -MetaTitle null `
 -MetaDescription null `
 -MetaKeywords null `
 -SearchKeywords null `
 -HarmonizedSystemCode null `
 -Url null `
 -SeoUrl null `
 -Manufacturer null `
 -ManufacturerId null `
 -BackorderStatus null `
 -Images null `
 -Tags null `
 -Files null
```

- Convert the resource to JSON
```powershell
$ProductAddBatchPayloadInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

