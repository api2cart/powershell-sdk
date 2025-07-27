# ProductVariantUpdate
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **String** | Defines variant update specified by variant id | [optional] 
**ProductId** | **String** | Defines product&#39;s id where the variant has to be updated | [optional] 
**StoreId** | **String** | Defines store id where the variant should be found | [optional] 
**LangId** | **String** | Language id | [optional] 
**Options** | [**ProductVariantUpdateOptionsInner[]**](ProductVariantUpdateOptionsInner.md) | Defines variant&#39;s options list | [optional] 
**Name** | **String** | Defines variant&#39;s name that has to be updated | [optional] 
**Description** | **String** | Specifies variant&#39;s description | [optional] 
**ShortDescription** | **String** | Defines short description | [optional] 
**Model** | **String** | Specifies variant&#39;s model that has to be added | [optional] 
**Sku** | **String** | Defines new product&#39;s variant sku | [optional] 
**Visible** | **String** | Set visibility status | [optional] 
**Status** | **String** | Defines product variant&#39;s status | [optional] 
**BackorderStatus** | **String** | Set backorder status | [optional] 
**LowStockThreshold** | **Decimal** | Specify the quantity threshold below which the product is considered low in stock | [optional] 
**AvailableForSale** | **Boolean** | Specifies the set of visible/invisible product&#39;s variants for sale | [optional] [default to $true]
**Avail** | **Boolean** | Defines category&#39;s visibility status | [optional] [default to $true]
**IsDefault** | **Boolean** | Defines as a default variant | [optional] 
**IsFreeShipping** | **Boolean** | Specifies variant&#39;s free shipping flag that has to be added | [optional] 
**Taxable** | **Boolean** | Specifies whether a tax is charged | [optional] [default to $true]
**TaxClassId** | **String** | Defines tax classes where entity has to be added | [optional] 
**IsVirtual** | **Boolean** | Defines whether the product is virtual | [optional] [default to $false]
**ManageStock** | **Boolean** | Defines inventory tracking for product variant | [optional] 
**InStock** | **Boolean** | Set stock status | [optional] 
**WarehouseId** | **String** | This parameter is used for selecting a warehouse where you need to set/modify a product quantity. | [optional] 
**ReserveQuantity** | **Decimal** | This parameter allows to reserve/unreserve product variants quantity. | [optional] 
**Quantity** | **Decimal** | Defines new products&#39; variants quantity | [optional] 
**IncreaseQuantity** | **Decimal** | Defines the incremental changes in product quantity | [optional] [default to 0]
**ReduceQuantity** | **Decimal** | Defines the decrement changes in product quantity | [optional] [default to 0]
**Price** | **Decimal** | Defines new product&#39;s variant price | [optional] 
**SpecialPrice** | **Decimal** | Defines new product&#39;s variant special price | [optional] 
**RetailPrice** | **Decimal** | Defines new product&#39;s retail price | [optional] 
**OldPrice** | **Decimal** | Defines product&#39;s old price | [optional] 
**CostPrice** | **Decimal** | Defines new product&#39;s cost price | [optional] 
**FixedCostShippingPrice** | **Decimal** | Specifies fixed cost shipping price | [optional] 
**SpriceCreate** | **String** | Defines the date of special price creation | [optional] 
**SpriceExpire** | **String** | Defines the term of special price offer duration | [optional] 
**Weight** | **Decimal** | Weight | [optional] [default to 0]
**Barcode** | **String** | A barcode is a unique code composed of numbers used as a product identifier. | [optional] 
**Width** | **Decimal** | Defines product&#39;s width | [optional] 
**WeightUnit** | **String** | Weight Unit | [optional] 
**Height** | **Decimal** | Defines product&#39;s height | [optional] 
**Length** | **Decimal** | Defines product&#39;s length | [optional] 
**Gtin** | **String** | Global Trade Item Number. An GTIN is an identifier for trade items. | [optional] 
**Upc** | **String** | Universal Product Code. A UPC (UPC-A) is a commonly used identifer for many different products. | [optional] 
**Mpn** | **String** | Manufacturer Part Number. A MPN is an identifier of a particular part design or material used. | [optional] 
**Ean** | **String** | European Article Number. An EAN is a unique 8 or 13-digit identifier that many industries (such as book publishers) use to identify products. | [optional] 
**Isbn** | **String** | International Standard Book Number. An ISBN is a unique identifier for books. | [optional] 
**HarmonizedSystemCode** | **String** | Harmonized System Code. An HSC is a 6-digit identifier that allows participating countries to classify traded goods on a common basis for customs purposes | [optional] 
**CountryOfOrigin** | **String** | The country where the inventory item was made | [optional] 
**MetaTitle** | **String** | Defines unique meta title for each entity | [optional] 
**MetaDescription** | **String** | Defines unique meta description of a entity | [optional] 
**MetaKeywords** | **String** | Defines unique meta keywords for each entity | [optional] 
**Reindex** | **Boolean** | Is reindex required | [optional] [default to $true]
**ClearCache** | **Boolean** | Is cache clear required | [optional] [default to $true]

## Examples

- Prepare the resource
```powershell
$ProductVariantUpdate = Initialize-PSOpenAPIToolsProductVariantUpdate  -Id 10 `
 -ProductId 10 `
 -StoreId 1 `
 -LangId 3 `
 -Options null `
 -Name Bag Green L `
 -Description Product variant `
 -ShortDescription Short description. This is very short description `
 -Model bag_01 `
 -Sku bag_01 `
 -Visible catalog `
 -Status disabled `
 -BackorderStatus true `
 -LowStockThreshold 1 `
 -AvailableForSale false `
 -Avail false `
 -IsDefault true `
 -IsFreeShipping true `
 -Taxable false `
 -TaxClassId 9 `
 -IsVirtual false `
 -ManageStock false `
 -InStock true `
 -WarehouseId 1 `
 -ReserveQuantity 1 `
 -Quantity 6 `
 -IncreaseQuantity 4 `
 -ReduceQuantity 4 `
 -Price 99.9 `
 -SpecialPrice 56.9 `
 -RetailPrice 6.9 `
 -OldPrice 99.9 `
 -CostPrice 65.9 `
 -FixedCostShippingPrice 5.5 `
 -SpriceCreate 2018-08-25 23:56:12 `
 -SpriceExpire 2018-08-25 23:56:12 `
 -Weight 23.69 `
 -Barcode 9770317847001 `
 -Width 56.12 `
 -WeightUnit lb `
 -Height 56.12 `
 -Length 56.12 `
 -Gtin 12345678912345 `
 -Upc 9770317847001 `
 -Mpn 9770317847001 `
 -Ean 5901234123457 `
 -Isbn 9783161484100 `
 -HarmonizedSystemCode 123456 `
 -CountryOfOrigin 123456 `
 -MetaTitle category,test `
 -MetaDescription category,test `
 -MetaKeywords category,test `
 -Reindex false `
 -ClearCache false
```

- Convert the resource to JSON
```powershell
$ProductVariantUpdate | ConvertTo-JSON
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

