# ProductVariantUpdateBatchPayloadInner
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** |  | 
**ProductId** | **String** |  | 
**Name** | **String** |  | [optional] 
**Description** | **String** |  | [optional] 
**ShortDescription** | **String** |  | [optional] 
**Sku** | **String** |  | [optional] 
**Upc** | **String** |  | [optional] 
**Mpn** | **String** |  | [optional] 
**Gtin** | **String** |  | [optional] 
**Isbn** | **String** |  | [optional] 
**Status** | **String** |  | [optional] 
**Price** | **Decimal** |  | [optional] 
**SpecialPrice** | **Decimal** |  | [optional] 
**CostPrice** | **Decimal** |  | [optional] 
**RetailPrice** | **Decimal** |  | [optional] 
**AdvancedPrices** | [**ProductUpdateBatchPayloadInnerAdvancedPricesInner[]**](ProductUpdateBatchPayloadInnerAdvancedPricesInner.md) | If an empty array is passed, all entries will be deleted when the &#39;nested_items_update_behaviour&#39; parameter is set to &#39;replace&#39;. | [optional] 
**Quantity** | **Decimal** |  | [optional] 
**ReserveQuantity** | **Decimal** |  | [optional] 
**IncreaseQuantity** | **Decimal** |  | [optional] 
**ReduceQuantity** | **Decimal** |  | [optional] 
**WarehouseId** | **String** |  | [optional] 
**ManufacturerId** | **String** |  | [optional] 
**Weight** | **Decimal** |  | [optional] 
**Height** | **Decimal** |  | [optional] 
**Length** | **Decimal** |  | [optional] 
**Width** | **Decimal** |  | [optional] 
**StoreId** | **String** |  | [optional] 
**LangId** | **String** |  | [optional] 
**TaxClassId** | **String** |  | [optional] 
**BackorderStatus** | **String** |  | [optional] 
**Visible** | **String** |  | [optional] 
**IsDefault** | **Boolean** |  | [optional] 
**InStock** | **Boolean** |  | [optional] 
**IsVirtual** | **Boolean** |  | [optional] 
**Downloadable** | **Boolean** |  | [optional] 
**ManageStock** | **Boolean** |  | [optional] 
**IsFreeShipping** | **Boolean** |  | [optional] 
**SeoUrl** | **String** |  | [optional] 
**MetaTitle** | **String** |  | [optional] 
**MetaDescription** | **String** |  | [optional] 
**MetaKeywords** | **String[]** |  | [optional] 
**CategoriesIds** | **String[]** | If an empty array is passed, all entries will be deleted when the &#39;nested_items_update_behaviour&#39; parameter is set to &#39;replace&#39;. | [optional] 
**StoresIds** | **String[]** |  | [optional] 
**Images** | [**ProductAddBatchPayloadInnerImagesInner[]**](ProductAddBatchPayloadInnerImagesInner.md) | The passed items will completely replace the original items | [optional] 
**ProductImagesIds** | **String[]** |  | [optional] 
**RelatedProductsIds** | **String[]** | If an empty array is passed, all entries will be deleted when the &#39;nested_items_update_behaviour&#39; parameter is set to &#39;replace&#39;. | [optional] 
**UpSellProductsIds** | **String[]** | If an empty array is passed, all entries will be deleted when the &#39;nested_items_update_behaviour&#39; parameter is set to &#39;replace&#39;. | [optional] 
**CrossSellProductsIds** | **String[]** | If an empty array is passed, all entries will be deleted when the &#39;nested_items_update_behaviour&#39; parameter is set to &#39;replace&#39;. | [optional] 

## Examples

- Prepare the resource
```powershell
$ProductVariantUpdateBatchPayloadInner = Initialize-PSOpenAPIToolsProductVariantUpdateBatchPayloadInner  -Id null `
 -ProductId null `
 -Name null `
 -Description null `
 -ShortDescription null `
 -Sku null `
 -Upc null `
 -Mpn null `
 -Gtin null `
 -Isbn null `
 -Status null `
 -Price null `
 -SpecialPrice null `
 -CostPrice null `
 -RetailPrice null `
 -AdvancedPrices null `
 -Quantity null `
 -ReserveQuantity null `
 -IncreaseQuantity null `
 -ReduceQuantity null `
 -WarehouseId null `
 -ManufacturerId null `
 -Weight null `
 -Height null `
 -Length null `
 -Width null `
 -StoreId null `
 -LangId null `
 -TaxClassId null `
 -BackorderStatus null `
 -Visible null `
 -IsDefault null `
 -InStock null `
 -IsVirtual null `
 -Downloadable null `
 -ManageStock null `
 -IsFreeShipping null `
 -SeoUrl null `
 -MetaTitle null `
 -MetaDescription null `
 -MetaKeywords null `
 -CategoriesIds null `
 -StoresIds null `
 -Images null `
 -ProductImagesIds null `
 -RelatedProductsIds null `
 -UpSellProductsIds null `
 -CrossSellProductsIds null
```

- Convert the resource to JSON
```powershell
$ProductVariantUpdateBatchPayloadInner | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

