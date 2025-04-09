# ProductUpdateBatchPayloadInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | 
**Name** | **String** |  | [optional] 
**Description** | **String** |  | [optional] 
**ShortDescription** | **String** |  | [optional] 
**Sku** | **String** |  | [optional] 
**Model** | **String** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**SpecialPrice** | **Decimal** |  | [optional] 
**SpriceCreate** | **String** |  | [optional] 
**SpriceExpire** | **String** |  | [optional] 
**CostPrice** | **Decimal** |  | [optional] 
**OldPrice** | **Decimal** |  | [optional] 
**FixedCostShippingPrice** | **Decimal** |  | [optional] 
**AdvancedPrices** | [**ProductUpdateBatchPayloadInnerAdvancedPricesInner[]**](ProductUpdateBatchPayloadInnerAdvancedPricesInner.md) | If an empty array is passed, all entries will be deleted when the &#39;nested_items_update_behaviour&#39; parameter is set to &#39;replace&#39;. | [optional] 
**Quantity** | **Decimal** |  | [optional] 
**IncreaseQuantity** | **Decimal** |  | [optional] 
**ReduceQuantity** | **Decimal** |  | [optional] 
**ReserveQuantity** | **Decimal** |  | [optional] 
**StoreId** | **String** |  | [optional] 
**LangId** | **String** |  | [optional] 
**Status** | **String** |  | [optional] 
**Type** | **String** |  | [optional] 
**Condition** | **String** |  | [optional] 
**Visible** | **String** |  | [optional] 
**AvailableForView** | **Boolean** |  | [optional] 
**AvailableForSale** | **Boolean** |  | [optional] 
**AvailFrom** | **String** |  | [optional] 
**Weight** | **Decimal** |  | [optional] 
**Length** | **Decimal** |  | [optional] 
**Width** | **Decimal** |  | [optional] 
**Height** | **Decimal** |  | [optional] 
**DimensionsUnit** | **String** |  | [optional] 
**WeightUnit** | **String** |  | [optional] 
**ManageStock** | **Boolean** |  | [optional] 
**InStock** | **Boolean** |  | [optional] 
**BackorderStatus** | **String** |  | [optional] 
**IsFreeShipping** | **Boolean** |  | [optional] 
**IsVirtual** | **Boolean** |  | [optional] 
**Taxable** | **Boolean** |  | [optional] 
**Downloadable** | **Boolean** |  | [optional] 
**WarehouseId** | **String** |  | [optional] 
**TaxClassId** | **String** |  | [optional] 
**CategoriesIds** | **String[]** |  | [optional] 
**MetaTitle** | **String** |  | [optional] 
**MetaDescription** | **String** |  | [optional] 
**MetaKeywords** | **String[]** |  | [optional] 
**Url** | **String** |  | [optional] 
**SeoUrl** | **String** |  | [optional] 
**Manufacturer** | **String** |  | [optional] 
**ManufacturerId** | **String** |  | [optional] 
**Mpn** | **String** |  | [optional] 
**Gtin** | **String** |  | [optional] 
**Upc** | **String** |  | [optional] 
**Isbn** | **String** |  | [optional] 
**Ean** | **String** |  | [optional] 
**Barcode** | **String** |  | [optional] 
**Images** | [**ProductUpdateBatchPayloadInnerImagesInner[]**](ProductUpdateBatchPayloadInnerImagesInner.md) | Property &#39;nested_items_update_behaviour&#39; does not apply. Specified items will be added to existing product images | [optional] 
**RelatedProductsIds** | **String[]** | If an empty array is passed, all entries will be deleted when the &#39;nested_items_update_behaviour&#39; parameter is set to &#39;replace&#39;. | [optional] 
**UpSellProductsIds** | **String[]** | If an empty array is passed, all entries will be deleted when the &#39;nested_items_update_behaviour&#39; parameter is set to &#39;replace&#39;. | [optional] 
**CrossSellProductsIds** | **String[]** | If an empty array is passed, all entries will be deleted when the &#39;nested_items_update_behaviour&#39; parameter is set to &#39;replace&#39;. | [optional] 
**Tags** | **String[]** |  | [optional] 
**SearchKeywords** | **String[]** |  | [optional] 
**HarmonizedSystemCode** | **String** |  | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductUpdateBatchPayloadInner = Initialize-PSOpenAPIToolsProductUpdateBatchPayloadInner  -Id null `
 -Name null `
 -Description null `
 -ShortDescription null `
 -Sku null `
 -Model null `
 -Price null `
 -SpecialPrice null `
 -SpriceCreate null `
 -SpriceExpire null `
 -CostPrice null `
 -OldPrice null `
 -FixedCostShippingPrice null `
 -AdvancedPrices null `
 -Quantity null `
 -IncreaseQuantity null `
 -ReduceQuantity null `
 -ReserveQuantity null `
 -StoreId null `
 -LangId null `
 -Status null `
 -Type null `
 -Condition null `
 -Visible null `
 -AvailableForView null `
 -AvailableForSale null `
 -AvailFrom null `
 -Weight null `
 -Length null `
 -Width null `
 -Height null `
 -DimensionsUnit null `
 -WeightUnit null `
 -ManageStock null `
 -InStock null `
 -BackorderStatus null `
 -IsFreeShipping null `
 -IsVirtual null `
 -Taxable null `
 -Downloadable null `
 -WarehouseId null `
 -TaxClassId null `
 -CategoriesIds null `
 -MetaTitle null `
 -MetaDescription null `
 -MetaKeywords null `
 -Url null `
 -SeoUrl null `
 -Manufacturer null `
 -ManufacturerId null `
 -Mpn null `
 -Gtin null `
 -Upc null `
 -Isbn null `
 -Ean null `
 -Barcode null `
 -Images null `
 -RelatedProductsIds null `
 -UpSellProductsIds null `
 -CrossSellProductsIds null `
 -Tags null `
 -SearchKeywords null `
 -HarmonizedSystemCode null
```

- Convert the resource to JSON
```powershell
$ProductUpdateBatchPayloadInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

